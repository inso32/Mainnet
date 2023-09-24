## **Useful commands**

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

## **Start service and check the logs**
```
sudo systemctl start nolusd
```
```
journalctl -u nolusd -f --no-hostname -o cat
```


## **Balance**

nolusd query bank balances [address]

```
nolusd query bank balances nolus1wxkayzug62vmy84askp5sh79jnc5kkv83v2tnn
```


## **Delegate tokens to validator**
nolusd tx staking delegate <TO_VALOPER_ADDRESS> 1000000unls --from wallet --chain-id rila-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```
nolusd tx staking delegate nolusvaloper144f8fdkdmaxux0zkn6y7dgdwyv9ue0m0d66jhd 2000000unls --from Atlas.Node --chain-id rila-1 --gas-adjustment 1.4 --gas auto --fees 2500unls -y
```

## **Validator management**

Edit existing validator
```
nolusd tx staking edit-validator \
--new-moniker "YOUR_MONIKER_NAME" \
--identity "YOUR_KEYBASE_ID" \
--details "YOUR_DETAILS" \
--website "YOUR_WEBSITE_URL" \
--chain-id pirin-1 \
--commission-rate 0.05 \
--from wallet \
--gas-adjustment 1.4 \
--gas auto \
--fees 2500unls \
-y

```
