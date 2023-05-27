# How-to-install-grafana
Link https://grafana.com/grafana/download
## Ubuntu and Debian
### Install
```
sudo apt-get install -y adduser libfontconfig1
wget https://dl.grafana.com/enterprise/release/grafana-enterprise_9.5.2_amd64.deb
sudo dpkg -i grafana-enterprise_9.5.2_amd64.deb
```
### Status
```
/bin/systemctl daemon-reloa
/bin/systemctl enable grafana-server
```
### Start Server
```
/bin/systemctl start grafana-server
```
