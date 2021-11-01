# 6. different checkbox style

### Problem

https://bigfrontend.dev/css/checkbox-style

#

### Problem Description

The default checkbox style might not be what you want for most of the time, in this problem you are asked to create a different checkbox style.

1. when unchecked, show a gray circle (`'color: gray'`)
2. when checked, show a green circle (`'color: green'`)

Set the circle with radius of 5px and don't add extra padding, the HTML structure is

```html
<label class="my-checkbox">
  <input type="checkbox" />
  <span>a checkbox</span>
</label>
```

**1. unchecked**

<kbd>![result 1](result-1.png)</kbd>

**2. checked**

<kbd>![result 2](result-2.png)</kbd>

#

### Solution

```css
/* your code here */
.my-checkbox {
  display: flex;
  align-items: center;
}

input[type='checkbox'] {
  /* Disable default styles */
  appearance: none;
  -webkit-appearance: none;

  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: gray;
  margin: 0;
}

input[type='checkbox']:checked {
  background: green;
}
```
