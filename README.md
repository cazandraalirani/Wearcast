# Wearcast

Wearcast is an environmental monitoring project built with the Seeed Studio Wio Terminal.

## Demo

Watch the Wearcast demonstration on YouTube:

[Watch the Wearcast demo](https://youtu.be/kn96rUHvSbA?si=07AiwrvELlJ7ddT_)

## Features

- Measures temperature using a Grove temperature sensor.
- Measures humidity using a DHT11 sensor.
- Displays temperature and humidity on the Wio Terminal LCD.
- Uses an LED strip to indicate temperature.
- Publishes sensor readings to an MQTT broker.

## Hardware

- Seeed Studio Wio Terminal
- Grove temperature sensor
- DHT11 temperature and humidity sensor
- NeoPixel LED strip (10 LEDs)

## Software libraries

The project uses:

- Adafruit NeoPixel
- DHT sensor library
- TFT_eSPI
- Seeed Arduino rpcWiFi
- PubSubClient

Wire and math are included with the platform/toolchain.

## Configuration

1. Copy `network_info.example.h`.
2. Rename the copy to `network_info.h`.
3. Enter your own Wi-Fi name and password.
4. Keep your real `network_info.h` private.

## MQTT

Broker: broker.emqx.io

Temperature topic: `/WearCast/sensor/temperature`

Humidity topic: `/WearCast/sensor/humidity`

## Credits

Some humidity-reading code was adapted from the Smart_Garden example by lakshanthad:

https://github.com/lakshanthad/Wio_Terminal_Classroom_Arduino

Temperature-reading code was adapted from Seeed Studio's Grove Temperature Sensor documentation.
