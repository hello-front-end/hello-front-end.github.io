---
layout: default
title: css中的过渡和动画效果
---
现在看一下css中的过渡和动画效果：
首先要说的是translate，它的作用是让元素产生平移，现在各大浏览器应该是都已经支持了，如果不支持的话，需要加上浏览器的内核标识。eg：
```.translate{
	transform: translate(100px,100px);
}
```
这就会让这个div向下，向右都平移100px；
接下来是rotate，它的作用是让元素旋转，参数是需要旋转的角度，单位是deg，正值代表顺时针旋转，eg：
```.rotate {
	transform: rotate(20deg);
}
```
之后还有skew来指定倾斜角度，

接下来是过渡，这里最重要的是transition属性，它是一个复合属性，可同时指定需要过渡的属性，延时开始的时间transition-delay，过渡的持续时间transition-duration，以及过渡效果的时间曲线transition-timing-function的类型，
当然也可以分开使用这几个属性

之后应该是动画，用的是animation属性，它的值有多个，一个是自己设置的关键帧@keyframe的名称，另一个是整个动画的执行时间，还有其他的一些属性用到时可以自己去查找。
之后会在@keyframe中指定动画中的一些路径点的效果样式


