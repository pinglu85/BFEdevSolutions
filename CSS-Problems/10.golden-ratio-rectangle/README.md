# 10. golden ratio rectangle

### Problem

https://bigfrontend.dev/css/golden-ratio-rectangle

#

### Problem Description

Let's create a golden ratio rectangle, which means width/height = 1.618.

This rectangle should have the fixed ratio even when width changes.

```html
<div class="golden-ratio"></div>
```

**1. width: 50px**

<kbd>![result 1](result-1.png)</kbd>

**2. width: 100px**

<kbd>![result 2](result-2.png)</kbd>

**3. width: 200px**

<kbd>![result 3](result-3.png)</kbd>

#

### Solution

```css
.golden-ratio {
  background-color: #ccc;
  aspect-ratio: 1.618;
}
```
