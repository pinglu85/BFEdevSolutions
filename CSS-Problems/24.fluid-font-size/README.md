# 24. fluid font size

### Problem

https://bigfrontend.dev/css/fluid-font-size

#

### Problem Description

Create a heading of fluid font size.

1. if viewport width is smaller than 200px, use 16px
2. if viewport width is bigger than 400px, use 32px
3. otherwise font-size is linearly scaled. For example if viewport is 300px = (200px + 400px) / 2, then font-size is 24px = (16px + 32px) / 2

```html
<h1 class="title">BFE.dev</h1>
```

**1. 100px**

<kbd>![result 1](result-1.png)</kbd>

**2. 150px**

<kbd>![result 2](result-2.png)</kbd>

**3. 200px**

<kbd>![result 3](result-3.png)</kbd>

**4. 219px**

<kbd>![result 4](result-4.png)</kbd>

**5. 252px**

<kbd>![result 5](result-5.png)</kbd>

**6. 300px**

<kbd>![result 6](result-6.png)</kbd>

**7. 379px**

<kbd>![result 7](result-7.png)</kbd>

**8. 400px**

<kbd>![result 8](result-8.png)</kbd>

**9. 500px**

<kbd>![result 9](result-9.png)</kbd>

#

### Solution

```css
.title {
  text-align: center;
  font-size: clamp(16px, 8vw, 32px);
}
```
