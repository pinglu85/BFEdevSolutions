# 11. fit the image

### Problem

https://bigfrontend.dev/css/fit-the-image

#

### Problem Description

Suppose we have following image of ratio `1:4`

![image](image.svg)

Now in an HTML structure like below, please fit the image to the container div, just as if it is used as container's background-image with `background-size:cover`.

```html
<div>
  <img class="image" src="..." />
</div>
```

**1. 50x50**

![result 1](result-1.png)

**2. 100x100**

![result 2](result-2.png)

**3. 200x100**

![result 3](result-3.png)

**4. 100x200**

![result 4](result-4.png)

**5. 300x100**

![result 5](result-5.png)

**6. 100x300**

![result 6](result-6.png)

#

### Solution

```css
.image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
```
