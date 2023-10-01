## Get validator info
```
nolusd status 2>&1 | jq .ValidatorInfo

```

## Get sync info
```
nolusd status 2>&1 | jq .SyncInfo

```
catching_up:<br>
- <b>false</b> - node has caught up to the current state of the network<br>
- <b>true</b> - node is still syncing


## Get live peers

```
curl -sS http://localhost:14357/net_info | jq -r '.result.peers[] | "\(.node_info.id)@\(.remote_ip):\(.node_info.listen_addr)"' | awk -F ':' '{print $1":"$(NF)}'
```

## [Restore a Validator](https://docs-nolus-protocol.notion.site/Run-a-Mainnet-Validator-f64624c3423c4c41922c3a1d0d342e17)

- Set up a full Nolus node synced up to the latest block.

- Replace the ~/.nolus/config/priv_validator.json file of the new node with the associated file from the old node, then restart your node.


## Remove Node
```
cd $HOME
sudo systemctl stop nolusd
sudo systemctl disable nolusd
sudo rm /etc/systemd/system/nolusd.service
sudo systemctl daemon-reload
rm -f $(which nolusd)
rm -rf $HOME/.nolus
rm -rf $HOME/nolus-core
```
