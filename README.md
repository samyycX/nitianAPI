# nitianAPI
一个可以获取逆天小作文的API

# API
**API: 124.222.34.97/nitian**

请求方式:GET

# 返回数据(JSON):

**注意:**  
**换行符: 下面的正文中的换行符为\n，请自行处理**  
**emoji: 下面的正文中可能含有emoji代码，如\uD83E\uDD41**  

- `code`    int类型, 状态码，目前2001代表获取成功，1000代表未知错误  
- `err`     string类型，如果错误时会返回对应的文本，获取成功时为""  
- `nitian`  jsonobject, 获取成功时有数据，获取失败时为null  
  - `id` int类型, 逆天小作文的id, 如果内容有错误可以在这里提交issue,并给出这个id
  - `text` string类型, 正文
  
样例:
```
{
  "code": 2001
  "err": ""
  "nitian": {
    "id": 11
    "text": "正文"
  }
}
```
