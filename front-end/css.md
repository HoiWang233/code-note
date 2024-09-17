###### transition: 渐入

```
transition: 0.3s;
```

###### cursor: 停留在元素上改变鼠标外观

可以用于按钮等可以交互的元素

* pointer: 可以交互小手
* wait: 读取中小圈
* not-allowed: 不允许交互

```
cursor: pointer;
```

###### display:

grid

把容器分为一个个网格,然后就可以设置元素占多少个网格

```

        .banner__container {
            display: grid;
            gap: 1rem;
            grid-auto-rows: 200px;
        }

    .banner__card:nth-child(1) {
            grid-area: 1 / 1 / 3 / 3;
        }

```

flex

###### :root 初始化参数

用作初始化一些参数,简化代码

```
:root {
  --primary-color: #42200b;
  --secondary-color: #ffc135;
  --tertiary-color: #df1c1c;
  --text-dark: #212529;
  --white: #ffffff;
  --max-width: 1200px;
  --header-font-1: "Alfa Slab One", serif;
  --header-font-2: "Bebas Neue", sans-serif;
}
```

###### text-align 设置字的水平对齐

```
/* 左对齐 */
.left-align {
    text-align: left;
}

/* 右对齐 */
.right-align {
    text-align: right;
}

/* 居中对齐 */
.center-align {
    text-align: center;
}
```

###### z-index 控制图层顺序

```
ss
深色版本
/* 图层 A */
.layer-a {
    position: absolute;
    z-index: 1;
    background-color: red;
    width: 100px;
    height: 100px;
}

/* 图层 B */
.layer-b {
    position: absolute;
    z-index: 2;
    background-color: blue;
    width: 100px;
    height: 100px;
    left: 50px;
    top: 50px;
}
```
