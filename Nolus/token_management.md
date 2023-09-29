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

## Redelegate tokens to another validator
```
nolusd tx staking redelegate $(nolusd keys show wallet --bech val -a) <TO_VALOPER_ADDRESS> 1000000unls --from wallet --chain-id pirin-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
