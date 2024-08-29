---
{
  "title": "数据库范式",
  "description": "关系数据库设计必备八股文",
  "author": "leedaisen",
  "date": "2022-04-14T00:00:00.000Z",
  "tags": [
    "数据库",
    "other"
  ],
  "minutes": 8.715,
  "words": 1743,
  "head": {
    "meta": [
      {
        "name": "description",
        "content": "本文介绍了数据库范式的概念，从1NF到5NF分别阐述了不同范式的特点和应用场景。在实际应用中，我们需要根据具体需求选择合适的范式进行数据库设计。总的来说，3NF和BCNF在减少数据冗余和维护数据完整性方面表现优秀，适用于大多数场景。但对于实际应用中的数据规范化，还需要结合具体业务需求进行权衡。"
      },
      {
        "name": "image",
        "content": "https://leelaa.cn/logo.webp"
      },
      {
        "name": "keywords",
        "content": "数据库,other"
      },
      {
        "name": "og:title",
        "content": "数据库范式"
      },
      {
        "name": "og:description",
        "content": "本文介绍了数据库范式的概念，从1NF到5NF分别阐述了不同范式的特点和应用场景。在实际应用中，我们需要根据具体需求选择合适的范式进行数据库设计。总的来说，3NF和BCNF在减少数据冗余和维护数据完整性方面表现优秀，适用于大多数场景。但对于实际应用中的数据规范化，还需要结合具体业务需求进行权衡。"
      },
      {
        "name": "og:keywords",
        "content": "数据库,other"
      },
      {
        "name": "og:type",
        "content": "article"
      },
      {
        "name": "twitter:card",
        "content": "summary_large_image"
      },
      {
        "name": "twitter:image",
        "content": "https://leelaa.cn/logo.webp"
      },
      {
        "name": "twitter:title",
        "content": "数据库范式"
      },
      {
        "name": "twitter:description",
        "content": "本文介绍了数据库范式的概念，从1NF到5NF分别阐述了不同范式的特点和应用场景。在实际应用中，我们需要根据具体需求选择合适的范式进行数据库设计。总的来说，3NF和BCNF在减少数据冗余和维护数据完整性方面表现优秀，适用于大多数场景。但对于实际应用中的数据规范化，还需要结合具体业务需求进行权衡。"
      }
    ],
    "link": [
      {
        "rel": "canonical",
        "href": "https://leelaa.cn/posts/ahsuea"
      }
    ]
  }
}
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
