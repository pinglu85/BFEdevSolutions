# 19. color of input elements

### Problem

https://bigfrontend.dev/css/change-color-of-input-elements

#

### Problem Description

We have a slider but we want to change the default color into `#F44336`.

```html
<input type="range" min="0" max="10" />
```

**#F44336**

<kbd>![result](result.png)</kbd>

#

### Solution

```css
input[type='range'] {
  accent-color: #f44336;
}
```

#

### Reference

[accent-color](https://developer.mozilla.org/en-US/docs/Web/CSS/accent-color)
