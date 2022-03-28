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
   "tokenId":"string",//token编号
   "productId":"string",//产品码
   "image":"string",//图片地址
   "owner":"string"//持有人
}
```

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

## 
