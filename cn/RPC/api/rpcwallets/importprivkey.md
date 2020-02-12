﻿# importprivkey 方法

导入私钥到钱包。

> 执行此命令前需要先调用`openwallet`方法打开钱包。



```json
{
  "jsonrpc": "2.0",
  "method": "importprivkey",
  "params": [key],
  "id": 1
}
```



### 参数说明

* key: WIF 格式的私钥。



## 调用示例

请求正文：

```json
{
  "jsonrpc": "2.0",
  "method": "importprivkey",
  "params": ["L5c6jz6Rh8arFJW3A5vg7Suaggo28ApXVF2EPzkAXbm94ThqaA6r"],
  "id": 1
}
```

响应正文：

```json
{
    "jsonrpc": "2.0",
    "id": 1,
    "result": {
        "address": "Ad8S24trcuchyLfEbJWqRP7BUScUT4t2pw",
        "haskey": true,
        "label": null,
        "watchonly": false
    }
}
```

响应说明：

返回地址信息。