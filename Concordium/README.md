
## Concordium News

23.10.23 Upgrade to version 6.1.7

25.09.23 Upgrade to version 6.0.4


## Files system structure

Database - database-v4

var/lib/private/concordium-9dd9ca4d19e9393877d2c44b70f89acbfc0883c2243e5eeaecc0d1cd0503f478/data/database-v4

The database contains files: blockstate-0.dat ... 

and directories:  treestate-0 ...

## Run a node

1. Download the Mainnet Debian package  v6.0.4
2. Install the package
```
sudo apt install /path-to-downloaded-package
```

## [Monitoring](https://medium.com/concordium/how-to-monitor-your-concordium-node-6c329e48c9c0)
How to set up Prometheus and Grafana



## Useful commands

View logs
```
journalctl -u concordium-mainnet-node -f
```
concordium-mainnet-node.service

systemctl status concordium-mainnet-node.service

sudo systemctl stop concordium-mainnet-node.service

sudo systemctl edit concordium-mainnet-node.service

sudo systemctl restart concordium-mainnet-node.service



concordium-mainnet-node-collector

sudo systemctl stop concordium-mainnet-node-collector

sudo systemctl edit concordium-mainnet-node-collector

sudo systemctl restart concordium-mainnet-node-collector
