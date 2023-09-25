**Get validator info**
```
nolusd status 2>&1 | jq .ValidatorInfo

```

**Get sync info**
```
nolusd status 2>&1 | jq .SyncInfo

```

**Get live peers**

```
curl -sS http://localhost:14357/net_info | jq -r '.result.peers[] | "\(.node_info.id)@\(.remote_ip):\(.node_info.listen_addr)"' | awk -F ':' '{print $1":"$(NF)}'
```

**Remove Node**
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
