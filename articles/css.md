###实时编辑CSS
通过设置style标签的display:block样式可以让页面的style标签显示出来，并且加上contentEditable属性后可以让样式成为可编辑状态，更改后的样式效果也是实时更新呈现的。此技巧在IE下无效。大家不妨演示一下！
```
<!DOCTYPE html>
<html>
    <body>
        <style style="display:block" contentEditable>
            body { color: blue }
        </style>
    </body>
</html>
```
###多重边框
利用重复指定box-shadow来达到多个边框的效果
```
/*CSS Border with Box-Shadow Example*/
div {
    box-shadow: 0 0 0 6px rgba(0, 0, 0, 0.2), 0 0 0 12px rgba(0, 0, 0, 0.2), 0 0 0 18px rgba(0, 0, 0, 0.2), 0 0 0 24px rgba(0, 0, 0, 0.2);
    height: 200px;
    margin: 50px auto;
    width: 400px
}
```
效果如下：
<p>![alt text](/assets/images/cssxiaoguo.png)</p>
###CSS中也可以做简单运算
通过CSS中的calc方法可以进行一些简单的运算，从而达到动态指定元素样式的目的。
```
.container{
    background-position: calc(100% - 50px) calc(100% - 20px);
}
```
###简单的文字模糊效果
以下两行简单的CSS3代码可达到将文字模糊化处理的目的，出来的效果有点像使用PS的滤镜!
```
p {
    color: transparent;
    text-shadow: #111 0 0 5px;
}
```