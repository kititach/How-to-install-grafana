# How-to-install-influxdb-grafana
influxdb : https://docs.influxdata.com/influxdb/v2.0/install/?t=Linux
grafana : https://grafana.com/grafana/download

## For Ubuntu/Debian users, add the InfluxData repository with the following commands
```
apt install gpg -y
wget -q https://repos.influxdata.com/influxdata-archive_compat.key
echo '393e8779c89ac8d958f81f942f9ad7fb82a25e133faddaf92e15b16e6ac9ce4c influxdata-archive_compat.key' | sha256sum -c && cat influxdata-archive_compat.key | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/influxdata-archive_compat.gpg > /dev/null
echo 'deb [signed-by=/etc/apt/trusted.gpg.d/influxdata-archive_compat.gpg] https://repos.influxdata.com/debian stable main' | sudo tee /etc/apt/sources.list.d/influxdata.list
```
### Status
```
systemctl start influxdb
systemctl status influxdb
```

## Install grafana Ubuntu and Debian
```
apt-get install -y adduser libfontconfig1
wget https://dl.grafana.com/enterprise/release/grafana-enterprise_9.5.2_amd64.deb
dpkg -i grafana-enterprise_9.5.2_amd64.deb
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
