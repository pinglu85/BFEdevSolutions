# 2. truncate text in one line(with ellipsis)

### Problem

https://bigfrontend.dev/css/truncate-text-with-ellipsis-in-one-line

#

### Problem Description

Truncate text in one line, if needed add ellipsis.

**1. When no overflow**

![result 1](result-1.png)

**2. When there is need to truncate, add ellipsis**

![result 2](result-2.png)

#

### Solution

```css
.one-line {
  /* your code here */
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}
```
