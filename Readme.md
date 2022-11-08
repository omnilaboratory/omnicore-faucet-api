## omnicored proxy api

This proxy offers public anonymous omnicore services to anonymous users and is currently for regtest/testnet only. It acts as the backend of OBD and can be deployed on a remote cloud. The motivation is to decouple the lightning node and the full Bitcoin/Omnilayer node, to lower the barriers of OBD deployment. 

The mainnet version will be available after omnicore V0.12 is activated.   

### main api

* mine: mine blocks, regtest only
* send_coin: the faucet sending tokens to an address, regtest/testnet only
* get_asset_balance
* list_assets
* query_asset
* create_asset  

The complete white-listed interfaces are in: [https://github.com/omnilaboratory/omnicore-proxy/blob/master/whitelist_proxy/whitelist_proxy.go](https://github.com/omnilaboratory/omnicore-proxy/blob/master/whitelist_proxy/whitelist_proxy.go)

### swagger doc  

http://62.234.169.68:29082/swagger/?surl=http://43.138.107.248:8090/openapiv2/foo.swagger.json  

![swagger preview](https://raw.githubusercontent.com/omnilaboratory/omnicore-fauct-api/master/swagger/img.png "swagger image")  


### programe start  
```
go run main.go
```
