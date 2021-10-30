# 2. truncate text in one line(with ellipsis)

### Problem

https://bigfrontend.dev/css/truncate-text-with-ellipsis-in-one-line

#

### Problem Description

Truncate text in one line, if needed add ellipsis.

**1. When no overflow**

<kbd>![result 1](result-1.png)</kbd>

**2. When there is need to truncate, add ellipsis**

<kbd>![result 2](result-2.png)</kbd>

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
