# ds18b20
DS18B20 temp sensor on a RPi

# Prerequisites

Because kernel modules need to be loaded, this script should be run with `sudo`.  Alternatively you can load the kernel modules first & ignore the `modprobe` errors:
```
sudo modprobe w1-gpio
sudo modprobe w1-therm
```

## InfluxDB

Install Python InfluxDB library if you want to use InfluxDB:
```
pip install influxdb
```

Fill in the `ds18b20.ini` with your InfluxDB information.
