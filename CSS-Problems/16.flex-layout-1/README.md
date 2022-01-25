# 16. flex layout 1

### Problem

https://bigfrontend.dev/css/flex-layout-1

#

### Problem Description

Suppose we have to layout a bunch of items with below requirements.

1. Fill out to width:100px, but stretch to fill the available space and shrink if not enough
2. Stack them if needed

HTML structure is

```html
<div class="container">
  <div class="item"></div>
  <div class="item"></div>
  <div class="item"></div>
</div>
```

**1. width:60px**

<kbd>![result 1](result-1.png)</kbd>

**2. width:150px**

<kbd>![result 2](result-2.png)</kbd>

**3. width:250px**

<kbd>![result 3](result-3.png)</kbd>

**4. width:400px**

<kbd>![result 4](result-4.png)</kbd>

#

### Solution

```css
.container {
  display: flex;
  flex-wrap: wrap;
}

.item {
  background-color: #7aa4f0;
  height: 50px;
  margin: 5px;
  flex: 1 1 100px;
}
```
