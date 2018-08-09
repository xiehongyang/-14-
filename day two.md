# 一灯学堂14天训练营笔记(第二天)

## CSS3可以构建3D世界，这个网站有模板可以搭建

tridiv.com

## 启动CSS3

```css
-webkit-transform-style: preserve-3d;
```

> `transform-style属性`确定元素的子元素是否位于3D空间中`，还是在该元素所在的平面内被扁平化。`
>
> 如果被扁平化，则子元素不会独立的存在于三维空间。
>
> 因为该属性不会被（自动）继承，所以必须为元素所有非叶子后代节点设置该属性。
>
> 值：
>
> `preserve-3d`
>
> 指定子元素定位在三维空间内。
>
> `flat`
>
> 指定子元素位于此元素所在平面内。

## 关于Transform属性

> CSS **transform** 属性允许你修改CSS视觉格式模型的坐标空间。使用它，元素可以被转换（translate）、旋转（rotate）、缩放（scale）、倾斜（skew）。 

## 关于perspective属性

> `perspective` 属性指定了观察者与z=0平面的距离，使具有三维位置变换的元素产生透视效果。z>0的三维元素比正常大，而z<0时则比正常小，大小程度由该属性的值决定。
>
> 三维元素在观察者后面的部分不会绘制出来，即z轴坐标值大于perspective属性值的部分。
>
> 默认情况下，*消失点*位于元素的中心，但是可以通过设置[`perspective-origin`](https://developer.mozilla.org/zh-CN/docs/Web/CSS/perspective-origin)属性来改变其位置。



