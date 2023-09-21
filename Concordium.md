## **Files system structure**

Database - database-v4
var/lib/private/concordium-9dd9ca4d19e9393877d2c44b70f89acbfc0883c2243e5eeaecc0d1cd0503f478/data/database-v4
Database содержит файлы blockstate-0.dat ... и папки  treestate-0 ...

1. Download the Mainnet Debian package  v6.0.4
2. Install the package
    sudo apt install /path-to-downloaded-package

## **Useful commands**

View logs
journalctl -u concordium-mainnet-node -f

concordium-mainnet-node.service
systemctl status concordium-mainnet-node.service
sudo systemctl stop concordium-mainnet-node.service
sudo systemctl edit concordium-mainnet-node.service
sudo systemctl restart concordium-mainnet-node.service

concordium-mainnet-node-collector
sudo systemctl stop concordium-mainnet-node-collector
sudo systemctl edit concordium-mainnet-node-collector
sudo systemctl restart concordium-mainnet-node-collector
