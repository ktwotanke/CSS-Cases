# CSS-Cases
This repository records some small CSS cases I wrote



##### HTML + CSS 创建肥皂泡动画

###### 示例

![肥皂泡动画](https://gitee.com/tanke99/pic/raw/master/pic/肥皂泡动画.gif)



调整每个span成border-left

![image-20240307140639999](https://gitee.com/tanke99/pic/raw/master/pic/image-20240307140639999.png)

###### key words

`filter`     `inset`   `zoom`



###### 使用场景

装饰页面



###### 注意

- .bubble::before{}，使用伪类中间不能有空格





##### Tab滑块切换动画

###### 示例

![Tab滑块切换动画](https://gitee.com/tanke99/pic/raw/master/pic/Tab滑块切换动画.gif)

###### key words

`box-shadow`   `linear-gradient`  `scss变量与循环语句`

label: for 与input 联动

http://t.csdnimg.cn/ZDF1X



scss转化为css

[VScode中的插件Live Sass Compiler](https://blog.csdn.net/qq_44625715/article/details/131491434)



###### 使用场景

使用自定义样式和动画的tab菜单，给每个input绑定单击事件得到当前显示项，从而发送请求，渲染不同的content内容。多个content-box可以使用v-show控制当前显示项。





###### 注意

- input - radio 要形成单选组，不要忘记添加相同的name属性
- input的id需要跟label的for相同才能实现点击label选中相同id的input，从而高亮label













- [x] box-shadow: 8px 8px 0 8px $clr;  详解此属性
- [x] tabs实现切换选中的原理