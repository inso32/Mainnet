## **Useful commands**


Узнать address
~~~
nolusd keys show Atlas.Node -a
~~~

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
