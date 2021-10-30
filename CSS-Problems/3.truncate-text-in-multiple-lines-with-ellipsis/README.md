# 3. truncate text in multiple lines(with ellipsis)

### Problem

https://bigfrontend.dev/css/truncate-text-in-multiple-lines-with-ellipsis

#

### Problem Description

Just like [2. truncate text in one line(with ellipsis)](https://bigfrontend.dev/css/truncate-text-with-ellipsis-in-one-line), please do the same for max 3 lines.

**1. short text(1 line)**

<kbd>![result 1](result-1.png)</kbd>

**2. short text (2 lines)**

<kbd>![result 2](result-2.png)</kbd>

**3. 3 lines(no overflow)**

<kbd>![result 3](result-3.png)</kbd>

**4. more than 3 lines**

<kbd>![result 4](result-4.png)</kbd>

#

### Solution

```css
.max-three-lines {
  /* your code here */
  display: -webkit-box;
  overflow: hidden;
  -webkit-box-orient: vertical;
  -webkit-line-clamp: 3;
}
```
