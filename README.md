## 导入NFT元数据

该接口应当具有一定的并发量，后期通过脚本或者aws函数调用来导入数据

#### Request Endpoint:

```
POST {endpoint}
```

#### Headers:
一个用于外部访问的key，未携带key访问此endpoint返回401
```
X-API-KEY
```

#### Request Body:

```
{
  "url": "sting",
  "txn_hash": [
        "string1",
        "string2"
    ],
  "product_code": "string",
  "collection_id": "string",
  "level": "sting",
  "type": int,
  "image": "string",
  "price": float
}
```

#### Response Body:

```
NONE
```

image example: https://d32ju6eqdh546d.cloudfront.net/riverestate/RiverEstate_0196.png

animation image example: https://d32ju6eqdh546d.cloudfront.net/riverestate/RiverEstate_0196.glb
