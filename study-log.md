# 学习日记

[TOC]



## 24/10/16

- 京东商品综合案例完成了点击小图切换到大图的作用
- 背诵拼写了第三单元的单词

## 24/10/17

- 京东商城实现了对商品信息的动态渲染
- 京东商城实现了放大镜效果，但是有bug初始大图不能显示
- 背诵第四单元单词

## 24/10/18

- 学习了解了一下函数防抖，但是不是很清楚
- 写了一个表单的小案例，在这个过程中
- 学会了一些未了解的选择器如focus,placeholder,checked,disabled,～（选择后面的一个兄弟）
- 建议表单用form而不是div
- select标签的属性-mutiple
- 建议每一个表格都用div进行包装，以至于后续好css添加样式
- 浮动元素造成的父亲元素高度坍塌添加伪类选择器：after

## 24/10/19

- 学习了正则表达式的基础写法

- 学习了并跟写了五子棋案例

- 修复了前面的京东案例放大镜的bug(url路径写错导致)

- 完成了京东案例的点击左右按钮切换大图的功能

- 完成了京东案例点击左右按钮border颜色随着切换的功能

- 学习了浏览器的http的简单工作原理

- 软件postman的基础使用

- 了解了事件循环的基本原理，三种进程

  - 浏览器进程


  - 网络进程


  - 渲染进程
    - 渲染主线程做的事包括js html css图片等的渲染

- 了解了下异步的编程的进行步骤(promise还没深入学习)

## 24/10/19

- 京东商城案例几乎完成，只有价格添加改变上还没做
- 简单了解了一下vue

## 24/10/21

- 复习了一下数组的各种方法

  - splice()

  - join()——数组转为字符串可控制以什么元素来连接数组

  - shift()——删除数组首位的元素

  - unshift()——在数组首位添加元素

  - delete arr[index]——数组也是对象，可以用delete方法删除

  - splice

    - splice(2,0,'lemon')——在第二个位置添加元素lemon
    
    - splice(0,1)——删除第一个元素
  - concat——连接多个数组并且生成一个新的数组
  - concat——连接多个数组并且生成一个新的数组
  - slice
    - slice(1)——从第一个位置开始剪切数组到最后一个
    - slice(a,b)——从第a个元素开始剪切到b-1个元素
  - sort()
  - sort()
  - ...剩余参数
- 初步接触vue
  - el——element用于指定当前vue实例位于哪个容器服务，值通常为css选择器字符串
  - data——data中用于存储数据，数据供el指定的容器去使用，值我们暂时先写成一个对象
  - 插值表达式{{}}
  - 指令语法——v-bind 可省略为 :
  - 单向双向数据绑定
  - 数据只能从data流向页面——v:bind
- 数据能在data和页面之间互流动——v-model只能绑定在表单元素上
  - data 和el的另外的写法
  - data 和el的另外的写法
- const  v = new Vue(),v.$mount("绑定的容器")
- data可以写为一个函数，但是不要写箭头函数（this）
## 2 4/10/22
- CommonJS——社区模块化
  - 只能运行在node环境下
  - module.exports =(对象、对象集合（函数）)——导出
  - require——导入
- ES Module——官方标准
  - export ——导出


  - import——导入

- 继续推进vue的学习


  - 数据代理——数据代理，通过一个对象代理对另一个对象中属性的操作


- Object.defineProperty（对象名，属性名，function(){}）


  - // value: 18,


  - // enumerable: true//控制属性是否可以枚举，默认值为false


  - // writable:true//控制属性是否可以被修改，默认值为false


  - // configurable: true//控制属性是否可以被删除，默认值为false


  - //delete person.age


- get——当有人读取对象中的这个属性名的时候，get函数就被我们调用，返回值就是属性的值


- set——当有人修改对象的这个属性的时候，set函数就会被调用，且会接受受到修改的具体值


  - 事件处理——使用vue来绑定事件
  - 事件处理——使用vue来绑定事件
- <button @click='showInfo(参数,$event)'>点击</button>，用$符号表示事件对象
  - 事件修饰符
  - 事件修饰符


- prevent 阻止默认事件


-   stop 阻止事件冒泡


-   once 事件只会触发一次


-   capture 事件的捕获模式


-   self 只有event.target是当前操作的元素的时候才触发事件


-   passive 时间的默认行为立即执行，无需等待事件的回调执行完毕

  - 键盘事件

  - 键盘事件

  -    回车键enter


-           删除delete  


-           退出esc


-           空格space


-          换行tab

-          上up


-           下down


-           左left


-           右right


-           切换大小写caps-lock，写成小写，单词中间- 


-           tab特殊必须配合keydown使用触发事件


-           ctrl alt shift meta键 为系统修饰键


-           配合keyup 都要加上别的按键，松开后触发


-       配合keydown正常触发

​      
​      

- 背诵第五单元单词

##  24/10/23

- 学习了vue的计算属性

  - computed

    - 内置set和get函数，
- get有什么作用？当有人读取fullName时候，get就会被调用，且返回值就作为fullName的值
  - 什么时候调用：
  - 什么时候调用：


  - 1 初次读取fullName时候被调用


  - 2 所依赖的数据发生变化时被调用


  - 即 firstName和lastName有发生改变的时候，get也会被调用


  - get函数做了缓存


  - 区别methods就会有缓存，用computed就会更方便一点


  - get中的this，此处的this是vue实例vm


  - set什么时候被调用？


  - 当fullName被修改的时候被调用


- 初步接触到vue的监视属性


  - watch

- freecamp完成了第一个练习

- 复习跟写了尚优选项目

- 背诵第六单元单词

## 24/10/24

- freecamp练习

- 了解了axios库的基础使用


  - axios({})

- 今天并没有很多的学习有点累

## 24/10/25

- 学习了axios的使用，post和get的区别，查询错误，url的组成，responsehead和requesthead
- vue的watch和complete的区别和使用
- 完成freecamp的游戏案例（备注：190多步数纯英文，受不了啦）
- watch的深度监视deep
- watch的简写方式，不用immediate和deep时候使用，二者默认都为false
- vue绑定class和绑定style的方式

## 24/10/26

- 抄写了三位数字随机抽奖的案例，并自己仿写了一个随机抽人的程序

- 学习了promise对象的基本概念——处理异步问题


  - unsettled未决阶段——挂起状态pending


  - settled已决阶段——完成状态/失败状态


  - then()


  - new promise((resolve,reject)={ 具体执行的内容}).then( (data)=>{成功了后续},(reason)=>{失败了返回原因}    )

- 学习了Vue的条件渲染


  - v-show
- v-show显示和隐藏用true和false值，原理只是给display添加了一个none属性，适合于需要频繁改变
  - v-if
  - v-if
- v-if和v-else-if 和v-else，倘若在每个条件中间有其他的元素那么会打断后面便不再进行判断了，用此条件的话，元素是整个都delete，而不是简单的display：none
  - template组件包裹，不会影响数据的结构
  - template组件包裹，不会影响数据的结构

- 学习了基本的列表渲染


  - v-for类似原生javasricpt的for of 和for in


  - :key属性的基本原理


  - key唯一的标识类似于身份证号、


  - 使用index作为key会出现的一些问题

##  24/10/27
- 跟写了一个图片拖动验证的三件套案例
- 学了了列表过滤（filter是生成一个新的数组哦）分别用computed和watch实现了
- 了解了一下Vue检测数据改变的原理（不是很清楚感觉有点复杂）
## 24/10/28
- 学习了v.set()方法
- 今日很疲惫
## 24/10/29
- 学习了Vue修改数组中的某个元素能够使用的常见api


  -  1.使用这些API:push()、pop()、shift()、unshift()、splice()、sort()、reverse()


  - 2.Vue.set() 或 vm.$set()

- 做了一个表单收集的小案例


  - trim
- 能够再收集的数据后去掉输入的前后的空格 
  - number
  - number
- 添加一个修饰符number表示这个输入的是数字而不是字符
  - lazy
  - lazy
- 当输入东西的时候失去焦点的瞬间再进行vue的收集而不是持续的收集
  - 当表单类型为radio时，我们给他添加一个value进行数据传递
  - 当表单类型为radio时，我们给他添加一个value进行数据传递

- 学习了过滤器


  - 语法：


- 1 用于插值表达式{{ xxxxx    |    过滤器名}}


- 2用于标签 v-bind:xxxx='xxxxxx    |    过滤器名字'


  - Vue.filter——全局配置一个过滤器
  - Vue.filter——全局配置一个过滤器


  - filters:{}——局部配置的过滤器


  - 过滤器可以进行一个串联过滤

- 学习了部分简单的内置指令

  - v-text——建议还是使用插值表达式


  - v-html——能够解析出来html标签


  - v-cloak——没有值，能够在网页加载过慢的时候，让这个标签进行隐藏，加载完成后这个指令消失，能够通过css选择器display:none


  - v-once——没有值，可以让这个属性被渲染一次后便视为静态内容不再更新

  - v-pre——没有值，可以让这个属性不再被Vue给读取，可以利用它跳过那些没有指令语法和插值语法的地方的节点


  - v-once和v-pre能够提高性能，加快编译

- 自定义指令——配置项：directives

## 24/10/30

- 学习了Vue的生命周期

  - beforeCreate()
  - created()
  - created()
  - beforeMount()
  - mounted()
  - beforeUpdate()
  - updated()
  - beforeDestroy()
  - destroyed()



