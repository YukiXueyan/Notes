【Android】使用recyclerView+adapter实现滑动布局，并添加点击和长按事件

本文基于《第一行代码（第三版）》，记录一下使用kotlin语言建立recyclerView+adapter的滑动布局，并在adapter中设定监听器，已达到在Activity中使用adapter时自主设定点击和长按事件。

## 新建fruit类、fruit的布局

1. fruit类

   ```kotlin
   class Fruit(val name:String, val bitmap: Bitmap)
   ```

   

2. 自定义布局

   ```xml
   <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
       android:layout_width="match_parent"
       android:layout_height="60dp">
   
       <ImageView
           android:id="@+id/fruitImage"
           android:layout_width="40dp"
           android:layout_height="40dp"
           android:layout_gravity="center_vertical"
           android:layout_marginLeft="10dp"/>
   
       <TextView
           android:id="@+id/fruitName"
           android:layout_width="wrap_content"
           android:layout_height="wrap_content"
           android:layout_gravity="center_vertical"
           android:layout_marginLeft="10dp" />
   
   </LinearLayout>
   
   ```

## 定义adapter适配器及监听接口

```kotlin
package com.example.adaptertest


import android.view.LayoutInflater
import android.view.View
import android.view.ViewGroup
import android.widget.ImageView
import android.widget.TextView
import androidx.recyclerview.widget.RecyclerView

class FruitAdapter(val fruitsList: List<Fruit>):
    RecyclerView.Adapter<FruitAdapter.ViewHolder>(){
    inner class ViewHolder(view: View) : RecyclerView.ViewHolder(view){
        val fruitView = view
        val fruitImage : ImageView = view.findViewById(R.id.fruitImage)
        val fruitName : TextView = view.findViewById(R.id.fruitName)
    }
    //此处设置监听器
    interface OnItemClickListener {
        fun onItemClick(view: View?, position: Int) //点击监听
        fun onItemLongClick(view: View?, position: Int)//长按监听
    }
    //调用监听器
    private var onItemClickListener: OnItemClickListener? = null

    fun setOnItemClickListener(onItemClickListener: OnItemClickListener?) {
        this.onItemClickListener = onItemClickListener
    }
    
    override fun onCreateViewHolder(parent: ViewGroup, viewType: Int): ViewHolder {
        val view = LayoutInflater.from(parent.context).inflate(R.layout.fruit_item, parent, false)
        val viewHolder = ViewHolder(view)
//        viewHolder.fruitImage.setOnClickListener {}

        return ViewHolder(view)

    }

    override fun onBindViewHolder(holder: ViewHolder, position: Int) {
        val fruit = fruitsList[position]
        holder.fruitImage.setImageBitmap(fruit.imgBitmap)
        holder.fruitName.text = fruit.name
        
        //设置监听器
        if (onItemClickListener != null) {
            holder.fruitView.setOnClickListener {
                val layoutPos = holder.layoutPosition
                onItemClickListener!!.onItemClick(holder.fruitView, layoutPos)
            }
            holder.fruitView.setOnLongClickListener {
                val layoutPos = holder.layoutPosition
                onItemClickListener!!.onItemLongClick(holder.fruitView, layoutPos)
                false
            }
        }
    }

    override fun getItemCount() = fruitsList.size
}
```

## 在Activity里使用recyclerView

```kotlin

class MainActivity : AppCompatActivity() {

    private val fruitList = ArrayList<Fruit>()

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)
        initFruits() // 初始化水果数据
        val layoutManager = LinearLayoutManager(this)
        recyclerView.layoutManager = layoutManager
        val adapter = FruitAdapter(fruitList)
        recyclerView.adapter = adapter

        adapter.setOnItemClickListener(object : FruitAdapter.OnItemClickListener{
            override fun onItemClick(view: View?, position: Int) {
                //定义点击事件
                Toast.makeText(this@MainActivity,"点击事件", Toast.LENGTH_SHORT).show()
            }
            override fun onItemLongClick(view: View?, position: Int) {
                //定义长按事件
                Toast.makeText(this@MainActivity,"长按事件", Toast.LENGTH_SHORT).show()
                //删除示例
                fruitList.removeAt(position)
                adapter.notifyDataSetChanged()
            }

        })
    }

    private fun initFruits() {
        repeat(2) {
            fruitList.add(Fruit("Apple", R.drawable.apple_pic))
            fruitList.add(Fruit("Banana", R.drawable.banana_pic))
            fruitList.add(Fruit("Orange", R.drawable.orange_pic))
            fruitList.add(Fruit("Watermelon", R.drawable.watermelon_pic))
            fruitList.add(Fruit("Pear", R.drawable.pear_pic))
            fruitList.add(Fruit("Grape", R.drawable.grape_pic))
            fruitList.add(Fruit("Pineapple", R.drawable.pineapple_pic))
            fruitList.add(Fruit("Strawberry", R.drawable.strawberry_pic))
            fruitList.add(Fruit("Cherry", R.drawable.cherry_pic))
            fruitList.add(Fruit("Mango", R.drawable.mango_pic))
        }
    }


}
```

## 改变recyclerView的布局为横向排布或网格排布

