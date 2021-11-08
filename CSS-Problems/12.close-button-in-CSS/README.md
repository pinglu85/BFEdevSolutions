# 12. close button in CSS

### Problem

https://bigfrontend.dev/css/css-cross-button

#

### Problem Description

Create a close button in CSS.

Lines for the cross should have

1. length : 3/4 of button width
2. thickness: 2px
3. color: `#aaa`

```html
<button class="close"></button>
```

**1. 20x20**

<kbd>![result 1](result-1.png)</kbd>

**2. 40x40**

<kbd>![result 2](result-2.png)</kbd>

**3. 60x60**

<kbd>![result 3](result-3.png)</kbd>

#

### Solution

```css
.close {
  position: relative;
  border: 1px solid #aaa;
  border-radius: 50%;
}

.close::after,
.close::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 75%;
  height: 2px;
  background: #aaa;
}

.close::after {
  transform: translate(-50%, -50%) rotate(45deg);
}

.close::before {
  transform: translate(-50%, -50%) rotate(-45deg);
}
```
