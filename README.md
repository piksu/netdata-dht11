# netdata-dht11
This is a plugin to display DHT11 sensor readings attached to Raspberry Pi on netdata dashboard.

## Installation
1. Put dht11.chart.py to `/usr/libexec/netdata/python.d`
2. Put dht11.conf to `/etc/netdata/python.d` and change the pin number
3. Put dashboard_info_dht11.js to `/usr/share/netdata/web/`
4. Edit `/etc/netdata/netdata.conf` so that:
```
[web]
custom dashboard_info.js = dashboard_info_dht11.js
```
5. `service netdata restart`

## Credits
This project uses code from [https://github.com/szazo/DHT11_Python](https://github.com/szazo/DHT11_Python).
