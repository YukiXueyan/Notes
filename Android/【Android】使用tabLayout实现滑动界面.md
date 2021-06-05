## 界面效果



## 代码实现

### 新建 OrdersPagerAdapter

`OrdersPagerAdapter`是用来定义要切换的fragment的顺序和创建出要显示的是哪一个fragment

```java

public class OrdersPagerAdapter extends FragmentStateAdapter {

    public OrdersPagerAdapter(@NonNull FragmentActivity fragmentActivity) {
        super(fragmentActivity);
    }


    @NonNull
    @Override
    public Fragment createFragment(int position) {
        switch (position){
            case 0:
                return new firstFragment();
            case 1:
                return new secondFragment();

        }
        return new firstFragment();//默认进入界面是展示的fragment
    }

    @Override
    public int getItemCount() {
        return 2;//返回fragment数量
    }

}

```



### 在activity中创建tabLayout进行切换

```java
        viewPager2 = findViewById(R.id.viewPager); //在xml中定义 androidx.viewpager2.widget.ViewPager2
        viewPager2.setAdapter(new OrdersPagerAdapter(this)); //将OrdersPagerAdapter加入viewPager2进行初始化

        TabLayout tabLayout = findViewById(R.id.tabLayout);//在xml中定义com.google.android.material.tabs.TabLayout
        TabLayoutMediator tabLayoutMediator = new TabLayoutMediator(
                tabLayout, viewPager2, new TabLayoutMediator.TabConfigurationStrategy() {
            @Override
            public void onConfigureTab(@NonNull TabLayout.Tab tab, int position) {
                switch (position){
                    case 0:
                        tab.setText("1");
                        tab.setIcon(R.drawable.ic_baseline_add_photo_alternate_24);//图标
                        break;
                    case 1:
                        tab.setText("2");
                        tab.setIcon(R.drawable.ic_baseline_folder_24);//图标
                        break;

                }
            }
        }
        );
        tabLayoutMediator.attach();

        viewPager2.registerOnPageChangeCallback(new ViewPager2.OnPageChangeCallback() {
            @Override
            public void onPageSelected(int position) {
                super.onPageSelected(position);
            }
        });
```

