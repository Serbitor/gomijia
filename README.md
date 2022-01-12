# gomijia

This is a simple tool, written in Go, that passively listens for Bluetooth LE broadcasts from a [Xiaomi Mijia Temperature/Humidity sensor] (https://www.banggood.com/Xiaomi-Mijia-Bluetooth-Thermometer-Hygrometer-with-LCD-Screen-Magnetic-Suction-Wall-Stickers-p-1232396.html) and writes them to a file for prometheus_node_exporter textfile collector.

It is configured via the `gomijia.ini` file, which specifies the details of the MQTT broker (hostname, username, password) as well as a mapping of Bluetooth MAC addresses to locations.

## Built With

* [Eclipse Paho MQTT Go client](https://github.com/eclipse/paho.mqtt.golang)
* [go-ble](https://github.com/go-ble/ble)
* [INI](https://ini.unknwon.io/)

## Author

* [Jonathan McDowell](https://www.earth.li/~noodles/blog/)
* David Leggett

## License

This project is licensed under the GPL 3+ license, see [COPYING](COPYING) for details.
