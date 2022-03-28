## 根据交易hash查询token

#### Request Endpoint:

```
GET {endpoint}/blockchain/v1/token
```

#### Headers:

```
None
```

#### Request Body:

```json
{
  "txnHash":"string"
}
```

#### Response Body:

```
{
   "contractId":"string",//合约地址
   "tokenId": integer,//token编号
   "productId":"string",//产品码
   "image":"string",//图片地址
   "animationUrl":"string",//动画地址，可以是glb/gif/mp4等
   "owner":"string"//持有人
}
```

image example: https://d32ju6eqdh546d.cloudfront.net/riverestate/RiverEstate_0196.png

animationUrl example: https://d32ju6eqdh546d.cloudfront.net/riverestate/RiverEstate_0196.glb

## 购买一个token

#### Request Endpoint:

```
POST {endpoint}/blockchain/v1/token
```

#### Headers:

```
x-api-key: {apiKey}
```

#### Request Body:

```json
{
  "productId":"string"
}
```

#### Response Body:

```json
{
    "txnHash":"string"
}
```

## 转赠一个token

TBD
