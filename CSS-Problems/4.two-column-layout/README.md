# 4. two-column layout

### Problem

https://bigfrontend.dev/css/two-column-layout

#

### Problem Description

Implement a basic two-column layout, in which left column takes up 25% width of the container with minimum width of 100px and right column fills up the rest.

**1. 400x300**

![result 1](result-1.png)

**2. 600x300**

![result 2](result-2.png)

**3. 300x300**

![result 3](result-3.png)

#

### Solution 1

```css
.container {
  height: 300px;
  /* your code here */
  display: flex;
}

.left {
  background-color: #f44336;
  /* your code here */
  width: 25%;
  min-width: 100px;
}

.right {
  background-color: #2973af;
  /* your code here */
  flex: 1;
}
```

#

### Solution 2

```css
.container {
  height: 300px;
  /* your code here */
  display: flex;
}

.left {
  background-color: #f44336;
  /* your code here */
  min-width: 100px;

  /* We cannot use `flex: 0.25 0 100px`, because `flex-basis` gives a default proportion, 
    then it will grow and shrink from that basis */
  flex: 1;
}

.right {
  background-color: #2973af;
  /* your code here */
  flex: 3;
}
```

#

### Reference

[flex-basis](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-basis)
