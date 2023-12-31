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
