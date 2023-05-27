# How-to-install-influxdb-grafana
influxdb : https://docs.influxdata.com/influxdb/v2.0/install/?t=Linux
grafana : https://grafana.com/grafana/download

## install influxdb
```

```

## Install grafana Ubuntu and Debian
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
