# 5. modal with max height

### Problem

https://bigfrontend.dev/css/modal-with-max-height

#

### Problem Description

Let's create a modal

1. it has header(fixed height: 50px) and stretching body
2. width of 300px and total max height 300px
3. centered in viewport
4. need minimum space of 30px to viewport top and bottom.

The HTML structure is something like

```html
<div class="modals">
  <div class="modal">
    <div class="modal-header"></div>
    <div class="modal-body"></div>
  </div>
</div>
```

**1. 400x150**

<kbd>![result 1](result-1.png)</kbd>

**2. 400x300**

<kbd>![result 2](result-2.png)</kbd>

**3. 400x400**

<kbd>![result 3](result-3.png)</kbd>

**4. 400x600**

<kbd>![result 4](result-4.png)</kbd>

#

### Solution

```css
.modals {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  padding: 30px 0;
}

.modal {
  width: 300px;
  height: 100%;
  max-height: 300px;
}

.modal-header {
  background-color: #f44336;
  height: 50px;
}

.modal-body {
  background-color: #2973af;
  height: calc(100% - 50px);
}
```
