# 1. center an element vertically

### Problem

https://bigfrontend.dev/css/center-an-element-vertically

#

### Problem Description

This is a very basic question and good to be the first CSS problem on BFE.dev.

Suppose you have an HTML structure as below

```html
<div class="outer">
  <div class="inner"></div>
</div>
```

Please center the inner div vertically without changing their dimensions and colors.

**1. Should be centered vertically**

![result 1](result-1.png)

**2. even if container size changes**

![result 2](result-2.png)

#

### Solution

```css
.outer {
  width: 100%;
  height: 100%;
  background-color: #efefef;
  /* your code here */
  display: flex;
  justify-content: center;
  align-items: center;
}

.inner {
  width: 100px;
  height: 100px;
  background-color: #f44336;
  /* your code here */
}
```
