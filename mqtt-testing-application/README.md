# MQTT Testing Application

This module provides a basic MQTT client script for testing communication with the Smartbike IoT infrastructure.

## Purpose

- Test publishing to and subscribing from MQTT topics
- Debug message formats
- Validate broker/device communication

## Location

`redback-smartbike-iot/mqtt-testing-application/`

## Setup

### Prerequisites

- Python 3.8+
- `paho-mqtt` installed (`pip install paho-mqtt`)
- MQTT broker credentials (Azure IoT Hub or local broker)

### Configuration 

Update the following in `testing_client.py`:

```python
MQTT_HOST = '<your_broker>'
MQTT_USER = '<your_username>'
MQTT_PASS = '<your_password>'
TOPICS = ['bike/+/speed', 'bike/+/cadence']  # or ['#'] for all topics

### Running the Script

python3 testing_client.py
