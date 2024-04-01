# CSS-Cases
This repository records some small CSS cases I wrote



##### HTML + CSS 创建肥皂泡动画

###### 示例

【使用Html和CSS创建肥皂泡动画】 https://www.bilibili.com/video/BV1GU411F7od/?share_source=copy_web&vd_source=aa5ac8ebb4929cac77f7506397cd2331

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

[Skills (yuque.com)](https://www.yuque.com/tanke-pmign/tanke/fiwypgc3cda9ai93#Z5nsn)



scss转化为css

[VScode中的插件Live Sass Compiler](https://blog.csdn.net/qq_44625715/article/details/131491434)



###### 使用场景

使用自定义样式和动画的tab菜单，给每个input绑定单击事件得到当前显示项，从而发送请求，渲染不同的content内容。多个content-box可以使用v-show控制当前显示项。





###### 注意

- input - radio 要形成单选组，不要忘记添加相同的name属性
- input的id需要跟label的for相同才能实现点击label选中相同id的input，从而高亮label





##### 3D卡片翻转

###### 示例

![3D卡片翻转](https://gitee.com/tanke99/pic/raw/master/pic/3D卡片翻转.gif)



###### key words

`perspective`   `transform-style`  `rotateY`

###### 使用场景

- 登录注册用卡片翻转实现；
- 鼠标悬浮图片，翻转出详情或者换图



注意：

`transform: translate3d(0, 0, 1px);`

翻转的元素需要加上以上属性

:这一行代码应用了一个 3D 平移变换到元素上。`translate3d` 函数接受三个参数，分别表示在 X、Y 和 Z 轴上的平移距离。这里的参数是 `(0, 0, 1px)`，表示在 Z 轴上向前平移了 1 像素。这个平移值是非常小的，只是为了防止一些浏览器在执行 3D 变换时可能出现的某些渲染问题。




在CSS中进行3D变换时，可能会出现一些渲染问题，其中一种可能的问题是闪烁或黑线的出现。这通常是由于硬件加速和像素渲染引擎的实现方式引起的。

一种可能的解决方法是在进行3D转换时，使用`translateZ`属性将元素稍微移动一个极小的距离，而不是只在2D平面上旋转。这样做可以触发硬件加速，并且通常可以减少闪烁和黑线的出现。

在给定的代码中，已经应用了`translate3d(0, 0, 1px)`以解决这个问题。但有时即使使用了这种方法，仍可能会出现一些闪烁。这可能取决于浏览器、操作系统、GPU和其他因素，因此不同环境下的表现可能有所不同。









透视perspective





- [x] box-shadow: 8px 8px 0 8px $clr;  详解此属性
- [x] tabs实现切换选中的原理