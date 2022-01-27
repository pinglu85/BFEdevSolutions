# 18. color gradients on text

### Problem

https://bigfrontend.dev/css/gradient-text

#

### Problem Description

Let's give text some color gradients, from `red` on the left to `yellow` on the right.

```html
<span class="gradient-text">practice on BFE.dev, get an offer</span>
```

**1. short text**

<kbd>![result 1](result-1.png)</kbd>

**2. longer text**

<kbd>![result 2](result-2.png)</kbd>

#

### Solution

```css
.gradient-text {
  font-size: 30px;
  font-weight: bold;

  /* The order matters. `background-clip` needs to be 
    written after `background` */
  background: linear-gradient(to right, red, yellow);
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
}
```
