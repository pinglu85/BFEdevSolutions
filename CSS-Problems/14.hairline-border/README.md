# 14. 0.5px border

### Problem

https://bigfrontend.dev/css/hairline

#

### Problem Description

When we set 0.5px in CSS, usually it will be rounded by browsers. But with better and better display like Retina display, 1px would sometimes looks thick.

Please add 0.5px top border of black for the following div.

```html
<div class="hairline"></div>
```

**should be thin enough**

<kbd>![result](result.png)</kbd>

#

### Solution

```css
.hairline {
  width: 300px;
  border-top: 1px solid black;
  transform: scale(0.5);
  transform-origin: 0 0;
}
```
