---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - javascript
---


# BlockQuery

### HTTP Request

`post http://state-api.otcgo.cn/api/v1/mainnet/public/graphql`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------

```javascript
ajax({
    url: url,
    method: 'post', 
    data: {
        query: 
        '{'+
            'BlockQuery (skip:skip, limit:limit) {'+
            'count,'+
            'rows {'+
              ' _id '+
              ' size '+
              ' version '+
              ' previousblockhash '+
              ' merkleroot '+
              ' time '+
              ' index '+
              ' nonce '+
              ' nextconsensus '+
              ' confirmations '+
              ' nextblockhash '+
              ' transactions '+
            '}'+
          '}'+
        '}'
    }
})
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "BlockQuery": {
      "count": 2045244,
      "rows": [
        {
          "_id": "5ab13d3794778f056f1364e6",
          "hash": "0xd2ccd6efab6fee10361e1c88dba017060f10fd3bf50e923220a9f0919698a0b4",
          "size": 3519,
          "version": 0,
          "previousblockhash": "0x01c74b1583534fa64719cb3ae341ad0914b85bf47b538783ba403033ace978cf",
          "merkleroot": "0xd6676ddd3d7760cea378295873a72ffeda4ad4bcea279778d96a3e33e25e698f",
          "time": 1521564937,
          "index": 2045243,
          "nonce": "6253ee6d5f4478d8",
          "script": {
            "invocation": "4089c6cff6323eb95dcb319e305acb4e32006bf5828cada07535f7f4e746924eb0e2be1b5d3cde93a17a0638ac7c573b18d48591d933716daf75191408d2c84de9409a3133846730b373ad77cc501399df73ac533a4188c7c00bccc8bfdde73df94a433fdd45763cc15ae12ca1f63dd5e2f2c26828c33680cc278f5a01fba857790c40a869984396338723e2c16e0c232d1facf32a70f02692ac46ad51aa675b95ef610d2fc0f136c63a1ed31606893e5e16be30926721d0602b78960066d8628f8b4b40e03eff699232f83d39c518f19f21d4860b3d2db8ca32e02870eb740034dc5b42461df6fc9df82b6f4c2268f7dd40bb0b2719d59db67effa90ff7e57e0305b25a402ae3e0b19c7b89e87b6e85be9a818638ef1639c9097b51fc19d55da86d45062fa962c0dce51f573f34cd83bf1748e5a4c4c11bda0f31cba8d7ac67beace37018",
            "verification": "552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
          },
          "nextconsensus": "APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR",
          "confirmations": 2,
          "nextblockhash": "0x317f2b2dda2b09c40e6f9f68fc1e5e85a45132f195089de74f4e6340d5090b1e",
          "transactions": 10
        },
        {
          "_id": "5ab13d1994778f056f1364de",
          "hash": "0x01c74b1583534fa64719cb3ae341ad0914b85bf47b538783ba403033ace978cf",
          "size": 2072,
          "version": 0,
          "previousblockhash": "0x3124b9de822d6e8d1ab38093edf291dc9958dcfbd7f2cc621fd65bce55221f44",
          "merkleroot": "0x84fa7bdb099ebcf8ab892b19ea24b541158cbf7e2e59fc58fd255e944c3d84d0",
          "time": 1521564916,
          "index": 2045242,
          "nonce": "667ac61567c8f247",
          "script": {
            "invocation": "40f6aeb19390e2aa48803a59dd3fbae6640f809f9ac991165f94cf1777f630512b4e1542792a0daf2dcae6a0f846144cd1b5f8d71166b6f3412ee175b8d20d4a27400e953abe0c2c0ebef467cb105e42b2c796cb971ba5640bd69f6d28a748f4aacdc94522c34e3dcfefd993a4229e6b3495b308999ee4bd369afaf68bf01e9131cf40a13c41de6487df97d6208e51a94bc21536662685be96c85738148e6bedcf65e53330af8c1a5b2a9947588ceec5c60eb1c0369489811f8f274afc5eb61f836e5440412262ff4a414f7cf80d8e62fb64735afa51651e9f23091c4ab3fcead4520c30e768425b78e0824fc83b33028c23461401a156bd18c4d1b4b58618c8ef08fb7540157b536e7b18b213b1ceb1dba6b49bf83f904e8f574d7f2f29f687624923102a0669fd92efae83b8448b352ba2c498ffe980ec5e54416ea2e5f0fa91c8a581ba",
            "verification": "552102486fd15702c4490a26703112a5cc1d0923fd697a33406bd5a1c00e0013b09a7021024c7b7fb6c310fccf1ba33b082519d82964ea93868d676662d4a59ad548df0e7d2102aaec38470f6aad0042c6e877cfd8087d2676b0f516fddd362801b9bd3936399e2103b209fd4f53a7170ea4444e0cb0a6bb6a53c2bd016926989cf85f9b0fba17a70c2103b8d9d5771d8f513aa0869b9cc8d50986403b78c6da36890638c3d46a5adce04a2102ca0e27697b9c248f6f16e085fd0061e26f44da85b58ee835c110caa5ec3ba5542102df48f60e8f3e01c48ff40b9b7f1310d7a8b2a193188befe1c2e3df740e89509357ae"
          },
          "nextconsensus": "APyEx5f4Zm4oCHwFWiSTaph1fPBxZacYVR",
          "confirmations": 2,
          "nextblockhash": "0xd2ccd6efab6fee10361e1c88dba017060f10fd3bf50e923220a9f0919698a0b4",
          "transactions": 7
        },
        ...
      ]
    }
  },
  "code": 200,
  "status": "OK",
  "server_time": "2018-03-20T16:56:51.792Z"
}
```


# TransactionQuery

### HTTP Request

`post http://state-api.otcgo.cn/api/v1/mainnet/public/graphql`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------


```javascript
ajax({
    url: url,
    method: 'post', 
    data: {
        query: 
        '{'+
            'TransactionQuery (skip:skip, limit:limit) {'+
            'count,'+
            'rows {'+
              ' _id '+
              ' txid '+
              ' blockIndex '+
              ' time '+
              ' size '+
              ' type '+
              ' vin { '+
                ' vout '+
                ' txid '+
                ' utxo { '+
                    ' address '+
                    ' value '+
                    ' asset '+
                    ' name '+
                ' } '+
              ' } '+
              ' vout { '+
                    ' address ' +
                    ' value ' +
                    ' asset ' +
                    ' n ' +
                    ' name ' +
              ' } '+
              ' nep5 { '+
                    ' to'+
                    ' from  '+
                    ' symbol '+
                    ' value '+
                    ' operation '+
                    ' assetId '+
              ' } '+
              ' scripts { '+
                ' invocation '+
                ' verification '+
              ' } '+
            '}'+
          '}'+
        '}'
    }
})
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "TransactionQuery": {
      "count": 2045244,
      "rows": [
        {
          "_id": "5ab1418d94778f056f136754",
          "txid": "0xa388154e18de89587b2a432bdea601f56db3d4f97bae07faec64f9f16208dbc7",
          "time": 1521566051,
          "blockIndex": 2045290,
          "size": 211,
          "type": "ContractTransaction",
          "vin": [
            {
              "vout": 0,
              "txid": "0x578fa728ac2c5ee1d31a364f37febe19bd102bdd2fb6b1e58d073a84e0decf75",
              "utxo": {
                "address": "AXsYAqEy4Cuw3S6UaVDawD3xueYC4b2xib",
                "value": "2",
                "asset": "0xc56f33fc6ecfcd0c225c4ab356fee59390af8560be0e930faebe74a6daff7c9b",
                "name": "NEO"
              }
            }
          ],
          "vout": [
            {
              "address": "AXsYAqEy4Cuw3S6UaVDawD3xueYC4b2xib",
              "value": "2",
              "asset": "0xc56f33fc6ecfcd0c225c4ab356fee59390af8560be0e930faebe74a6daff7c9b",
              "n": 0,
              "name": "NEO"
            }
          ],
          "scripts": [
            {
              "invocation": "40cb2ad0b824ab7d3faa3967102375269e10e36d0e4f5edf7e88c4134d02a639bfea088b8324aab67fc7eed21ff8f7cbbfcae6c23ad1be0d2bec12a5d2163bcccd",
              "verification": "2103180a17928e6ae7911413392d997e4bfebb44fc005d23fd55612fc4b95b3d5f4aac"
            }
          ],
          "sys_fee": "0",
          "net_fee": "0"
        },
        {
          "_id": "5ab1418d94778f056f136753",
          "txid": "0xd716b21b38393ecfb7b7c8feb7726d55fc5af54f14d4141496e7395d1a455b42",
          "time": 1521566051,
          "blockIndex": 2045290,
          "size": 203,
          "type": "ClaimTransaction",
          "vin": [],
          "vout": [
            {
              "address": "AMu4vUVHwd43u6FC4M1pkJtayCLtcXNzoS",
              "value": "1.40105875",
              "asset": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
              "n": 0,
              "name": "GAS"
            }
          ],
          "scripts": [
            {
              "invocation": "404298620f1ca5ba04c003293c88c20994f4bd948ccc0fc96d58f9b5283d1ca4f3655ad2b42364ac4330240667eaec0d86fec76a54f87f6c61d5af9e25d6669272",
              "verification": "2103e995a1e859a6689bce05cebb97e44d0d282632b87e47c01b1ce397c4bbe793f7ac"
            }
          ],
          "sys_fee": "0",
          "net_fee": "0"
        },
        ...
      ]
    }
  },
  "code": 200,
  "status": "OK",
  "server_time": "2018-03-20T16:56:51.792Z"
}
```

# AddressQuery

### HTTP Request

`post http://state-api.otcgo.cn/api/v1/mainnet/public/graphql`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------

```javascript
ajax({
    url: url,
    method: 'post', 
    data: {
        query: 
        '{'+
            'AddressQuery (skip:skip, limit: limit) {'+
            'count,'+
            'rows {'+
              ' _id '+
              ' address '+
              ' time '+
              ' blockIndex '+
            '}'+
          '}'+
        '}'
    }
})
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "AddressQuery": {
      "count": 797443,
      "rows": [
        {
          "_id": "5ab1427d94778f056f1367d9",
          "address": "AM5WFKAeTjnJ78vVMUP2LSs6PwKfa7pX3w",
          "blockIndex": 2045301,
          "time": 1521566296
        },
        {
          "_id": "5ab1422394778f056f1367a5",
          "address": "ASNyHHEbB1ieSvxEqXfZHXMtGAMXsmTHdn",
          "blockIndex": 2045296,
          "time": 1521566193
        },
        ...
      ]
    }
  },
  "code": 200,
  "status": "OK",
  "server_time": "2018-03-20T17:19:02.378Z"
}
```


# AssetQuery

### HTTP Request

`post http://state-api.otcgo.cn/api/v1/mainnet/public/graphql`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------

```javascript
ajax({
    url: url,
    method: 'post', 
    data: {
        query:'{'+
                ' AssetQuery(skip: skip, limit: limit ){ '+
                    ' count '+
                    ' rows { '+
                        ' _id '+
                        ' assetId '+
                        ' symbol '+
                        ' type '+
                        ' amount '+
                        ' name { '+
                            ' lang '+
                            ' name '+
                        ' } '+
                    ' } '+
                ' } '+
            ' } '
    }
})
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "AssetQuery": {
      "count": 35,
      "rows": [
        {
          "_id": "5aa9fa5e94778f592b2f47e5",
          "assetId": "0xc56f33fc6ecfcd0c225c4ab356fee59390af8560be0e930faebe74a6daff7c9b",
          "name": [
            {
              "lang": "zh-CN",
              "name": "NEO"
            },
            {
              "lang": "en",
              "name": "NEO"
            }
          ],
          "symbol": null,
          "type": "GoverningToken",
          "amount": "100000000"
        },
        {
          "_id": "5aa9fa6b94778f59302f47f6",
          "assetId": "0x602c79718b16e442de58778e148d0b1084e3b2dffd5de6b7b16cee7969282de7",
          "name": [
            {
              "lang": "zh-CN",
              "name": "GAS"
            },
            {
              "lang": "en",
              "name": "GAS"
            }
          ],
          "symbol": null,
          "type": "UtilityToken",
          "amount": "100000000"
        },
       ...
      ]
    }
  },
  "code": 200,
  "status": "OK",
  "server_time": "2018-03-20T17:20:41.423Z"
}
```

# SystemQuery

### HTTP Request

`post http://state-api.otcgo.cn/api/v1/mainnet/public/graphql`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------


## Get All Block

```javascript
ajax({
    url: url,
    method: 'post', 
    data: {
        query: '{'+
            ' SystemQuery { '+
                ' rows {'+
                    ' startTime '+
                    ' curretTime '+
                    ' blockNum '+
                    ' assetNum '+
                    ' addressNum '+
                    ' transactionNum '+
                ' } '+
            ' } '+
        ' } '
    }
})
```

> The above command returns JSON structured like this:

```json
{
  "data": {
    "SystemQuery": {
      "rows": {
        "startTime": "1468595301",
        "curretTime": "1521566679",
        "blockNum": "2045318",
        "assetNum": "35",
        "addressNum": "797448",
        "transactionNum": "10325580"
      }
    }
  },
  "code": 200,
  "status": "OK",
  "server_time": "2018-03-20T17:36:31.460Z"
}
```

# BalanceQuery

### HTTP Request

`get http://state-api.otcgo.cn/api/v1/mainnet/address/balances/{address}`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------


## Get All Block

```javascript
ajax({
    url: url,
    method: 'get'
})
```

> The above command returns JSON structured like this:

```json
{
status: "OK",
code: 200,
data: [
  {
  assetId: "0xc56f33fc6ecfcd0c225c4ab356fee59390af8560be0e930faebe74a6daff7c9b",
  name: "NEO",
  type: "GoverningToken",
  balances: "1"
  },
  {
  assetId: "0xceab719b8baa2310f232ee0d277c061704541cfb",
  name: "ONT",
  type: "nep5",
  balances: "0"
  },
  ...
],
server_time: "2018-03-20T17:39:07.208Z"
}
```