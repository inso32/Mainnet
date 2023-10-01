## Query commission
```
nolusd query distribution commission nolusvaloper1wxkayzug62vmy84askp5sh79jnc5kkv8gulwsw

```

## Query rewards for a validator and all their delegations

```
nolusd query distribution validator-outstanding-rewards nolusvaloper1wxkayzug62vmy84askp5sh79jnc5kkv8gulwsw

```


## Withdraw rewards from all validators
```
nolusd tx distribution withdraw-all-rewards --from wallet --chain-id pirin-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y


```

## Withdraw  commission and rewards from your validator

```
nolusd tx distribution withdraw-rewards nolusvaloper1wxkayzug62vmy84askp5sh79jnc5kkv8gulwsw --commission --from Atlas.Node --chain-id pirin-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```

## **Delegate tokens to validator**
nolusd tx staking delegate <TO_VALOPER_ADDRESS> 1000000unls --from wallet --chain-id rila-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
nolusd tx staking delegate nolusvaloper144f8fdkdmaxux0zkn6y7dgdwyv9ue0m0d66jhd 2000000unls --from Atlas.Node --chain-id pirin-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```


## Redelegate tokens to another validator
```
nolusd tx staking redelegate $(nolusd keys show wallet --bech val -a) <TO_VALOPER_ADDRESS> 1000000unls --from wallet --chain-id pirin-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
