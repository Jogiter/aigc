## 怎么让一个 div 水平垂直居中

要让一个 div 水平垂直居中，有以下几种常见的方法：

1. 使用 Flex 布局：

```html
<div class="parent">
  <div class="child"></div>
</div>
```

```css
.parent {
  display: flex;
  justify-content: center;
  align-items: center;
}

.child {
  width: 200px;
  height: 200px;
}
```

2. 使用绝对定位和 transform 属性：

```html
<div class="parent">
  <div class="child"></div>
</div>
```

```css
.parent {
  position: relative;
  width: 100%;
  height: 100%;
}

.child {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 200px;
  height: 200px;
  transform: translate(-50%, -50%);
}
```

3. 使用 table-cell 布局：

```html
<div class="parent">
  <div class="child"></div>
</div>
```

```css
.parent {
  display: table;
  width: 100%;
  height: 100%;
}

.child {
  display: table-cell;
  width: 200px;
  height: 200px;
  vertical-align: middle;
  text-align: center;
}
```

以上三种方法都能够实现 div 的水平垂直居中，具体使用哪种方法可以根据实际需求和兼容性情况来选择。
