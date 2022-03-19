# Avalanche Node
Quickly Launch an avalanche node for Validation or RPC. 

## Avalanche node RPC calls

Check if the blockchain is synced

````curl -X POST --data '{
    "jsonrpc":"2.0",
    "id"     :1,
    "method" :"info.isBootstrapped",
    "params": {
        "chain":"X"
    }
}' -H 'content-type:application/json;' 127.0.0.1:9650/ext/info
````

Get your node-id

````curl -X POST --data '{
    "jsonrpc":"2.0",
    "id"     :1,
    "method" :"info.getNodeID"
}' -H 'content-type:application/json;' 127.0.0.1:9650/ext/info


$ {"jsonrpc":"2.0","result":{"nodeID":"NodeID-5gPX5WhrocwHNEvAPofrrGDtxdo9cPJad"},"id":1}
````

If you like the work we do for the Avalanche Community, consider supporting our validator node:
    
    NodeID-F3SZA2ZNdRjTBe3GYyRQFDaCXB3DyaZQQ 
