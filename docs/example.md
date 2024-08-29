---
title: 数组切块
date: 2021-05-10T00:00:00.000Z
head:
    - - meta
    - name: description
      content: 在本文中，提供了一个名为`chunkArray`的函数，该函数接收一个数组`arr`和一个整数`size`作为参数。函数使用reduce函数对数组进行递归切块处理。在每个递归步骤中，首先通过切片操作提取出指定大小的块，然后通过filter函数过滤出剩余元素。最后，将切块后的数组返回。该方法简洁易用，适合处理需要分割数组的情况。
    - - meta
    - name: keywords
      content:  JavaScript 基础知识
---

# 一行代码数组切块

```javascript
// 数组切块
export const chunkArray = (arr, size) => {
    return arr.reduce((result, _, idx) => {
        result.push(arr.slice(idx * idx, idx * size + size));
        return result
    }, []
    ).filter(i => i.length)
}

```
