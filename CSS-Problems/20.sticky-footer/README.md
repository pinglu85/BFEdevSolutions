# 20. sticky footer

### Problem

https://bigfrontend.dev/css/sticky-footer

#

### Problem Description

"Sticky footer" is a layout pattern that

1. if content is short, the footer "sticks" to the bottom
2. otherwise, footer is is displayed after the content as normal.

Suppose we have some HTML structure:

```html
<div class="container">
  <div class="header">header</div>
  <div class="body">content here might be tall , might be short</div>
  <div class="footer">footer</div>
</div>
```

Blow is how Sticky Footer pattern should behave.

**1. footer sticks to bottom if content is short**

<kbd>![result 1](result-1.png)</kbd>

**2. otherwise footer is displayed as normal**

<kbd>![result 2](result-2.png)</kbd>

**3. event be pushed out from viewport if enough content**

<kbd>![result 3](result-3.png)</kbd>

#

### Solution

```css
html,
body {
  height: 100%;
}

.container {
  display: flex;
  flex-direction: column;
  height: 100%;
}

.header {
  background-color: #555;
  color: #fff;
  padding: 20px 10px;
}

.body {
  padding: 20px 10px;
  flex: 1 0 auto;
}

.footer {
  background-color: #555;
  color: #fff;
  padding: 20px 10px;
  flex-shrink: 0;
}
```

#

### Reference

[Sticky Footer, Five Ways](https://css-tricks.com/couple-takes-sticky-footer/)
