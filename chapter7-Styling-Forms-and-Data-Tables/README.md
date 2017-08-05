# 七、对表单和数据表格应用样式

## 对表格应用样式

CSS 规范有两个表格边盒模型：separate 和 collapsed。在 separate 模型中，各个单元格周围都有border，而在 collapsed 模型中，单元格之间是共享边框的。`border-collapse`属性默认为`collapsed`。另外，`border-spacing`属性可以控制单元格之间的距离。

``` css
table {
  border-collapse: separate;
  border-spacing: 0;
}
```

## 简单的表单布局

### 表单元素

`label` 元素极其重要，它可以帮助添加结构和增加表单的可用性和可访问性。单击标签元素将导致相关联的表单元素获得焦点。另外，使用`label`也会使`web`在屏幕阅读器上有更好的体验。

将标签与表单控件关联起来有两种方式:

1. 隐式

   ``` css
   <label>email <input name="email" type="text"/><label>
   ```

2. 显式，把`label`的`for`属性设置为相关联的表单元素的 id 。

   ``` css
   <label for="email">email<label>
   <input name="email" id="email" type="text"/>
   ```

   ​