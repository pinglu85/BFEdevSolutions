# 23. Grid Layout 2

### Problem

https://bigfrontend.dev/css/grid-layout-2

#

### Problem Description

Layout the items in a grid so that:

- items have minimum width of 100px and fill up the space
- place as many items in a row as possible
- gap between items is 10px

```html
<div class="container">
  <div class="item"></div>
  <div class="item"></div>
  <div class="item"></div>
</div>
```

**1. width:100px**

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
  display: grid;
  /* We can also replace `1fr` with `auto` */
  grid-template-columns: repeat(auto-fill, minmax(100px, 1fr));
  gap: 10px;
}

.item {
  height: 50px;
  background-color: #7aa4f0;
}
```

### Explanation

We use the `auto-fill` keyword for `repeat()` to make the browser fill the row with as many columns as it can fit.

#

### Reference

[repeat()](https://developer.mozilla.org/en-US/docs/Web/CSS/repeat)
