## react的特点

- 声明式的设计
- 高效，采用虚拟DOM来实现DOM的渲染，最大限度的减少DOM的操作。
- 灵活，跟其他库灵活搭配使用。
- 使用JSX，俗称JS里面写HTML，JavaScript语法的扩展。
- 组件化，模块化。代码容易复用
- 单向数据流。没有实现数据的双向绑定

## 创建react项目

方法1：

通过script引入使用，仅用于学习调试使用

`<script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script><script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>`

方法2：

通过react的脚手架，创建项目进行开发，部署

1. 安装脚手架[Create React App](https://react.docschina.org/docs/create-a-new-react-app.html#create-react-app)。`cnpm install -g create-react-app`

2. 创建项目`create-react-app 01reactapp`(项目名称可以自定义)

## JSX

### 优点

- 执行更快，有代码优化，采用虚拟DOM

- 类型更安全

- 编写模板更加简单快速

### 使用

- 必须要有根节点

- 正常的HTML元素要小写，大写的是组件

- **HTML的样式类名要写className而不是class，因为class在js中是关键字**

### JSX表达式

- 由HTML元素构成
- 中间如果需要插入变量用`{}`
- `{}`中间可以使用表达式
- `{}`中间表达式中可以使用JSX对象
- 属性和 html 内容一样都是用来插入内容

### JSX_style

- class，style中，**不可以存在多个class属性**

- style样式中，如果存在多个单词的属性组合，第二个单词开始，**首字母大写**。或者用引号引起来，否则会报错（border-bottom要写为borderBottom）

- 如果多个类共存，则需要使用数组和{}结合引用

  ```react
  let element2 = (
      <div>
          <h1 className={"abc "+classStr}>helloworld</h1>
      </div>
  )
  
  
  let classStr2 = ['abc2','redBg2'].join(" ")
  let element3 = (
      <div>
          {/* 这里写注释 */}
          <h1 className={classStr2} style={exampleStyle}>helloworld</h1>
      </div>
  )
  
  ```

  

- 注释必须在括号的表达式内书写，否则报错：`{/* 这里写注释 */}`



## react 元素渲染

`let h1 = <h1>helloworld</h1>;`

使用JSX的写法，可以创建JS元素对象

注意：JSX元素对象，或者组件对象，必须只有1个根元素（根节点）

```react
//example

//实现页面时刻的显示

function clock(){
    let time = new Date().toLocaleTimeString()
    let element = (
        <div>
            <h1>现在的时间是{time} </h1>
            <h2>这是副标题</h2>
        </div>
    )
    let root = document.querySelector('#root');
    ReactDOM.render(element,root)
}

clock()

setInterval(clock,1000)

//声明式组件渲染
function Clock(props){
    return (
                <div>
                    <h1>现在的时间是{props.date.toLocaleTimeString()} </h1>
                    <h2>这是函数式组件开发</h2>
                </div>
    )
}

function run(){
    ReactDOM.render(
        <Clock date={new Date()} />,
        document.querySelector('#root')
    )
}

setInterval(run,1000)
```



## React 组件

函数式组件与类组件的区别和使用，函数式比较简单，一般用于静态没有交互事件内容的组件页面。类组件，一般又称为动态组件，那么一般会有交互或者数据修改的操作

1. 函数式组件

   ```react
   //函数式组件
   function Childcom(props){
       console.log(props)
   
       let title = <h2>我是副标题</h2>
       let weather = props.weather
       //条件判断 
       let isGo = weather=='下雨' ?"不出门":"出门"
   
       return (
           <div>
               <h1>函数式组件helloworld</h1>
               {title}
   
               <div>
                   是否出门？
                   <span>{isGo}</span>
               </div>
           </div>
       )
   }
   
   ```

   

2. 类组件

   ```react
   //类组件定义
   class HelloWorld extends React.Component{
       render(){
           console.log(this)
           return (
               <div>
                   <h1>类组件定义HELLOWORLD</h1>
                   <h1>hello:{this.props.name}</h1>
                   <Childcom weather={this.props.weather} />
               </div>
           )
       }
   
   
   }
   
   ```

   

3. 复合组件(组件中又有其他的组件，复合组件中既可以有类组件又可以有函数组件)

   ```react
   import React from 'react';
   import ReactDOM from 'react-dom';
   import './04style.css';
   //函数式组件
   function Childcom(props){
       console.log(props)
   
       let title = <h2>我是副标题</h2>
       let weather = props.weather
       //条件判断 
       let isGo = weather=='下雨' ?"不出门":"出门"
   
       return (
           <div>
               <h1>函数式组件helloworld</h1>
               {title}
   
               <div>
                   是否出门？
                   <span>{isGo}</span>
               </div>
           </div>
       )
   }
   
   //类组件定义
   class HelloWorld extends React.Component{
       render(){
           console.log(this)
   //返回的都是JSX对象
           return (
               <div>
                   <h1>类组件定义HELLOWORLD</h1>
                   <h1>hello:{this.props.name}</h1>
                   <Childcom weather={this.props.weather} />
               </div>
           )
       }
   
   
   }
   
   
   // ReactDOM.render(
   //     <Childcom weather="出太阳" />,
   //     document.querySelector('#root')
   // )
   
   ReactDOM.render(
       <HelloWorld name="老陈" weather="下雨" />,
       document.querySelector('#root')
   )
   
   ```




## React State

state就是数据，被view渲染出来。

构造函数初始化数据，将需要改变的数据初始化到state中。

- 当需要改变数据时，可以在组件的render()中写改变方法。但是不是自动更新，所以不太推荐

  ```react
  import React from 'react';
  import ReactDOM from 'react-dom';
  
  
  class Clock extends React.Component{
      constructor(props){
          super(props)
          //状态（数据）--》view
          //构造函数初始化数据，将需要改变的数据初始化到state中
          this.state = {
              time:new Date().toLocaleTimeString()
          }
          //console.log(this.state.time)
      }
  
      render(){
          //console.log("这是渲染函数")
          this.state.time = new Date().toLocaleTimeString();
          return (
              <div>
                  <h1>当前时间：{this.state.time}</h1>
              </div>
          )
      }
  }
  ReactDOM.render(
      <Clock />,
      document.querySelector('#root')
  )
  //每一秒钟重新渲染
  setInterval(()=>{
      ReactDOM.render(
      <Clock />,
      document.querySelector('#root')
  )
  },1000)
  ```

  

- 使用生命周期函数

  ```react
  import React from 'react';
  import ReactDOM from 'react-dom';
  
  
  class Clock extends React.Component{
      constructor(props){
          super(props)
          //状态（数据）--》view
          //构造函数初始化数据，将需要改变的数据初始化到state中
          this.state = {
              time:new Date().toLocaleTimeString()
          }
          //console.log(this.state.time)
      }
  
      render(){
          //console.log("这是渲染函数")
          //this.state.time = new Date().toLocaleTimeString();
          return (
              <div>
                  <h1>当前时间：{this.state.time}</h1>
              </div>
          )
      }
  
      //生命周期函数,组件渲染完成时的函数
      componentDidMount(){
          setInterval(()=>{
              console.log(this.state.time)
              //this.state.time = new Date().toLocaleTimeString(); //错误的方式
              //切勿直接修改state数据，直接state重新渲染内容，需要使用setState
              //通过this.setState修改完数据后，并不会立即修改DOM里面的内容,react会在，
              //这个函数内容所有设置状态改变后，统一对比虚拟DOM对象，然后在统一修改，提升性能。
              //小程序也是也是借鉴REACT状态管理操作
              this.setState({
                  time:new Date().toLocaleTimeString()
              })
              
          },1000)
      }
  
  }
  ReactDOM.render(
      <Clock />,
      document.querySelector('#root')
  )
  ```

  

- 案例 点击切换

  ```react
  import React from 'react';
  import ReactDOM from 'react-dom';
  import './Tab.css'
  
  
  class Tab extends React.Component{
      constructor(props){
          super(props)
  
          //设置状态、数据
          this.state = {
              c1:'content active',
              c2:"content"
          }
  
          this.clickEvent = this.clickEvent.bind(this)
      }
      clickEvent(e){
          console.log('clickEvent')
          console.log(e.target.dataset.index)
          let index = e.target.dataset.index;
          console.log(this)
          if(index=='1'){
              this.setState({
                  c1:'content active'
                 
              })
              this.setState({
                  c2:"content"
              })
          }else{
              this.setState({
                  c1:'content',
                  c2:"content active"
              })
          }
      }
  
      render(){
          return (
              <div>
                  <button data-index="1" onClick={this.clickEvent}>内容一</button>
                  <button data-index="2" onClick={this.clickEvent}>内容二</button>
                  <div className={this.state.c1}>
                      <h1>内容1</h1>
                  </div>
                  <div className={this.state.c2}>
                      <h1>内容2</h1>
                  </div>
              </div>
          )
      }
  }
  
  
  
  ReactDOM.render(
      <Tab />,
      document.querySelector('#root')
  )
  
  ```



## props

父组件传递给子组件数据，是单向流动的，不能让子组件传递数据给父组件。

props的传值可以是任意的类型。

props可以设置默认值。

注意：props可以传递函数，props可以传递父元素的函数，就可以去修改父元素的state,从而达到传递数据给父元素。



- 父传子 数据：

  ```react
  import React from 'react';
  import ReactDOM from 'react-dom';
  import './01props.css'
  
  
  //在父元素中使用state去控制子元素props的从而达到父元素数据传递给子元素
  
  class ParentCom extends React.Component{
      constructor(props){
          super(props)
          this.state = {
              isActive:true
          }
          this.changeShow = this.changeShow.bind(this)
      }
  
      render(){
          return (
              <div>
                  <button onClick={this.changeShow}>控制子元素显示</button>
                  <ChildCom isActive={this.state.isActive} />
              </div>
          )
      }
  
      changeShow(){
          this.setState({
              isActive:!this.state.isActive
          })
      }
  }
  
  class ChildCom extends React.Component{
      constructor(props){
          super(props)
      }
      render(){
          let strClass = null;
          if(this.props.isActive){
              strClass = ' active'
          }else{
              strClass = ""
          }
          strClass = this.props.isActive?" active":"";
  
          return (
              <div className={"content"+strClass}>
                  <h1>我是子元素</h1>
              </div>
          )
      }
  }
  
  
  ReactDOM.render(
      <ParentCom />,
      document.querySelector("#root")
  )
  ```



- 子传父

  调用父元素的函数从而操作父元素的数据，从而实现数据从子元素传递至父元素

  ```react
  import React from 'react';
  import ReactDOM from 'react-dom';
  
  class ParentCom extends React.Component{
      constructor(props){
          super(props);
          this.state = {
              childData:null
          }
      }
  
      render(){
          return (
              <div>
                  <h1>子元素传递给父元素的数据：{this.state.childData}</h1>
                  <childCom setChildData={this.setChildData} />
              </div>
          )
      }
  
      setChildData = (data) =>{
          this.setState({
              childData:data
          })
      }
  }
  
  class ChildCom extends React.Component{
      constructor(props){
          super(props)
          this.state = {
              msg:"Hello World"
          }
      }
      render(){
          return (
              <div>
                  <button onClick = {this.sendData}>传递helloworld</button>
                  <button onClick = {()=>{this.props.setChildData("直接调用props")}}>直接传递helloworld</button>
  
              </div>
              )
      }
      sendData=()=>{
          this.props.setChildData(this.state.msg)
      }
  }
  
  ```



## React 事件

- 驼峰命名法

- {} 传入一个函数 ` onClick = {this.sendData}`

- 事件对象：React返回的事件对象是代理的原生的事件对象，如果想要查看事件对象的具体值，必须之间输出事件对象的属性

- 原生，阻止默认行为时，可以直接返回return false；

  React中，阻止默认必须e.preventDefault();



```react
import React from 'react';
import ReactDOM from 'react-dom';

class ParentCom extends React.Component{
    constructor(props){
        super(props)
    }
    render(){
        
        return (
            <div >
                <form action="http://www.baidu.com">
                    <div className="child" >
                        <h1>helloworld</h1>
                        <button onClick={this.parentEvent}>提交</button>
                    </div>

                </form>
                
                {/* 使用ES6箭头函数传递多个参数 */}
                <button  onClick={(e)=>{this.parentEvent1('msg:helloworld',e)}}>提交</button>
                {/* //不使用ES6箭头函数传递多个参数的方式 */}
                <button  onClick={function(e){this.parentEvent1('不使用es6,msg:helloworld',e)}.bind(this)}>提交</button>
            
            </div>
        )
    }
    parentEvent=(e)=>{
        console.log(e.preventDefault)
        e.preventDefault()
        //e.preventDefault()
        //return false;
    }
    parentEvent1 = (msg,e)=>{
        console.log(msg)
        console.log(e)
        
    }
}


ReactDOM.render(
    <ParentCom></ParentCom>,
    document.querySelector("#root")
)
```



## React 条件渲染

React中条件渲染即和JavaScript中，条件运算，如if...else...三元运算符等。

-  直接通过条件运算返回要渲染的JSX对象

- 通过条件运算得出jsx对象，在将JSX对象渲染到模板中。



eg1:

```react
import React from 'react';
import ReactDOM from 'react-dom';

function UserGreet(props){
    return (<h1>欢迎登陆</h1>)
}

function UserLogin(props){
    return (<h1>请先登录</h1>)
}


class ParentCom extends React.Component{
    constructor(props){
        super(props)
        this.state = {
            isLogin:true
        }
    }
    render(){
        if(this.state.isLogin){
            return (<UserGreet></UserGreet>)
        }else{
            return (<UserLogin></UserLogin>)
        }
    }
}


ReactDOM.render(
    <ParentCom></ParentCom>,
    document.querySelector('#root')
)
```



eg2:

```react
import React from 'react';
import ReactDOM from 'react-dom';

function UserGreet(props){
    return (<h1>欢迎登陆</h1>)
}

function UserLogin(props){
    return (<h1>请先登录</h1>)
}


class ParentCom extends React.Component{
    constructor(props){
        super(props)
        this.state = {
            isLogin:false
        }
    }
    render(){
        let element = null;
        if(this.state.isLogin){
            element = <UserGreet></UserGreet>;
        }else{
            element = (<UserLogin></UserLogin>);
        }

        

        return (
            <div>
                <h1>这是头部</h1>
                {element}
                <h1>这是三元运算符的操作</h1>
                {this.state.isLogin?<UserGreet></UserGreet>:<UserLogin></UserLogin>}
                <h1>这是尾部</h1>
            </div>
        )
    }
}


ReactDOM.render(
    <ParentCom></ParentCom>,
    document.querySelector('#root')
)
```





## React 列表渲染

将列表内容拼装成数组放置到模板中。将数据拼装成数组的JSX对象。

使用数组的map方法，对每一项数据按照JSX的形式进行加工，最终得到1个每一项都是JSX对象的数组，在将数组渲染到模板中。

Key值需要放置到每一项中。

```react
import React from 'react';
import ReactDOM from 'react-dom';

class Welcome extends React.Component{
    constructor(props){
        super(props)
        this.state = {
            list:[
                {
                    title:"第一节 React事件",
                    content:"事件内容"
                },
                {
                    title:"第二节 React数据传递",
                    content:"数据传递内容",
                },
                {
                    title:"第三节 条件渲染",
                    content:"条件渲染内容",
                }
            ]
        }
    }

    render(){
        let listArr = [];
        for(let i=0;i<this.state.list.length;i++){
            let item = (
                <li>
                    <h3>{this.state.list[i].title}</h3>
                    <p>{this.state.list[i].content}</p>
                </li>
            )
            listArr.push(item)
        }
        return (
            <div>
                <h1>
                    今天课程内容
                </h1>

                <ul>
                    {listArr}
                    <li>
                        <h3>这是标题</h3>
                        <p>内容</p>
                    </li>
                </ul>

            </div>
        )
    }
}


ReactDOM.render(
    <Welcome></Welcome>,
    document.querySelector('#root')
)
```



复杂写法：

```react
import React from 'react';
import ReactDOM from 'react-dom';

function ListItem(props){
    return (
        <li>
            <h3>{props.index+1}:listItem:{props.data.title}</h3>
            <p>{props.data.content}</p>
        </li>
    )
}


class ListItem2 extends React.Component{
    constructor(props){
        super(props)
    }
    render(){
        return (
            <li onClick={(event)=>{this.clickEvent(
                this.props.index,
                this.props.data.title,
                event
                )}}>
                <h3>{this.props.index+1}:listItem:{this.props.data.title}</h3>
                <p>{this.props.data.content}</p>
            </li>
        )
    }
    clickEvent=(index,title,event)=>{
        alert((index+1)+"-"+title)
    }
}



class Welcome extends React.Component{
    constructor(props){
        super(props)
        this.state = {
            list:[
                {
                    title:"第一节 React事件",
                    content:"事件内容"
                },
                {
                    title:"第二节 React数据传递",
                    content:"数据传递内容",
                },
                {
                    title:"第三节 条件渲染",
                    content:"条件渲染内容",
                }
            ]
        }
    }

    render(){
        let listArr = this.state.list.map((item,index)=>{
            return (
                <ListItem2 key={index} data={item} index={index}></ListItem2>
                
            )
        })
        
        return (
            <div>
                <h1>
                    今天课程内容
                </h1>

                <ul>
                    {listArr}
                    <li>
                        <h3>这是标题</h3>
                        <p>内容</p>
                    </li>
                </ul>

                <h1>复杂没有用组件完成列表</h1>
                <ul>
                {
                    this.state.list.map((item,index)=>{
                        return (
                            <li key={index} onClick={(event)=>{this.clickFn(index,item.title,event)}}>
                                <h3>{index+1}-复杂-{item.title}</h3>
                                <p>{item.content}</p>
                            </li>
                        )
                    })
                }
                </ul>

            </div>
        )
    }

    clickFn=(index,title,event)=>{
        alert((index+1)+"-clickFn-"+title)
    }
}


ReactDOM.render(
    <Welcome></Welcome>,
    document.querySelector('#root')
)
```



## for循环



## 生命周期

生命周期即是组件从实例化到渲染到最终从页面中销毁，整个过程就是生命周期，在这生命周期中，我们有许多可以调用的事件，也俗称为钩子函数

 

生命周期的3个状态：

Mounting:将组件插入到DOM中

Updating:将数据更新到DOM中

Unmounting:将组件移除DOM中

 

 

生命周期中的钩子函数（方法，事件）

 

CompontWillMount :组件将要渲染，AJAX，添加动画前的类

CompontDidMount:组件渲染完毕,添加动画

compontWillReceiveProps:组件将要接受props数据，查看接收props的数据什么

ShouldComponentUpdate：组件接收到新的state或者props,判断是否更新。返回布尔值

CompontWillUpdate:组件将要更新

ComponentDidUpdate:组件已经更新

ComponentwillUnmount:组件将要卸载





## React插槽

组件中写入内容，这些内容可以被识别和控制。React需要自己开发支持插槽功能。

原理：

组件中写入的HTML，可以传入到props中。

 

组件中的HTML内容直接全部插入

 

组件中根据HTML内容的不同，插入的位置不同。

 

## React 路由

根据不同的路径，显示不同的组件（内容）；React使用的库react-router-dom;

 

安装

  Cnpm install react-router-dom --save  

 

 

ReactRouter三大组件：

Router：所有路由组件的根组件（底层组件），包裹路由规则的最外层容器。

属性：basename->设置跟此路由根路径，router可以在1个组件中写多个。

Route:路由规则匹配组件，显示当前规则对应的组件

Link:路由跳转的组件

 

 

注意：如果要精确匹配，那么可以在route上设置exact属性。

 

 

Router使用案例



 

Link组件可以设置to属性来进行页面的跳转，to属性可以直接写路径的字符串，也可以通过1个对象，进行路径的设置，如

 

 

Link的replace属性：点击链接后，将新地址替换成历史访问记录的原地址。

 

动态路由实现：



## 重定向组件

如果访问某个组件时，如果有重定向组件，那么就会修改页面路径，使得页面内容显示为所定向路径的内容

 

用例：



 

## Switch组件

让switch组件内容的route只匹配1个，只要匹配到了，剩余的路由规则将不再匹配



 

## Redux 

解决React数据管理（状态管理），用于中大型，数据比较庞大，组件之间数据交互多的情况下使用。如果你不知道是否需要使用Redux，那么你就不需要用它！

\* 解决组件的数据通信。

\* 解决数据和交互较多的应用

 

Redux只是一种状态管理的解决方案！

 

 

Store:数据仓库，保存数据的地方。

State:state是1个对象，数据仓库里的所有数据都放到1个state里。

Action:1个动作，触发数据改变的方法。

Dispatch:将动作触发成方法

Reducer:是1个函数，通过获取动作，改变数据，生成1个新state。从而改变页面

 

安装

  Cnpm install redux --save  

 

​    

 

## React-redux

安装

  cnpm install react-redux --save  

 

概念：

Provider组件：自动的将store里的state和组件进行关联。

MapStatetoProps：这个函数用于将store的state映射到组件的里props

mapdispatchToProps:将store中的dispatch映射到组件的props里，实现了方法的共享。

Connect方法：将组件和数据（方法）进行连接

 

使用：

初始化数据，实例化store


  function reducer(state={num:0},action){    switch(action.type){      case "add":        state.num++;        break;      default:        break;    }    return {...state}  }     const store = createStore(reducer)     

 

数据的获取，数据的修改

要state映射到到组件的props中，将修改数据的方法映射到组件的props中

​     

 

 