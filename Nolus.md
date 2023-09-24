## **Useful commands**

View the logs
```
journalctl -u cosmovisor -f
```

Query the status of your node
```
curl http://localhost:26657/status | jq .result.sync_info.catching_up
```

true - node is still syncing

false - node has caught up to the current state of the network, and you are safe to upgrade your node to a validator



List all keys

```
nolusd keys list
```

Find out the address
~~~
nolusd keys show Atlas.Node -a
~~~

How to find out address and voloperaddress using explorer?

Open the validator and click on the transaction at the bottom in the Transactions section.

## **Balance**

nolusd query bank balances [address]

```
nolusd query bank balances nolus144f8fdkdmaxux0zkn6y7dgdwyv9ue0m0520h5s
```


## **Delegate tokens to validator**
nolusd tx staking delegate <TO_VALOPER_ADDRESS> 1000000unls --from wallet --chain-id rila-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
nolusd tx staking delegate nolusvaloper144f8fdkdmaxux0zkn6y7dgdwyv9ue0m0d66jhd 2000000unls --from Atlas.Node --chain-id rila-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
