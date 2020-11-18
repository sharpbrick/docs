# DuploTrainBaseHub (set 10874)

## Ports & Internal Devices

| Port | Type | Ext. Port |
| --- | --- | --- |
| 0  | [DuploTrainBaseMotor](../devices/duplotrainbasemotor.md) | n/a |
| 1  | [DuploTrainBaseSpeaker](../devices/duplotrainbasespeaker.md) | n/a |
| 17 | [RgbLight](../devices/rgblight.md) | n/a |
| 18 | [DuploTrainBaseColorSensor](../devices/duplotrainbasecolorsensor.md) | n/a |
| 19 | [DuploTrainBaseSpeedometer](../devices/duplotrainbasespeedometer.md) | n/a |
| 20 | [Voltage](../devices/voltage.md) | n/a |

## Hub Properties

| Property Name | Value | Supported | Default Value | Comment |
| --- | --- | --- | --- | --- |
| AdvertisingName | 0x01 | ✅ | Train Base |  |
| Button | 0x02 | ✅ | False |  |
| FwVersion | 0x03 | ✅ | 1.6.0.0  |  |
| HwVersion | 0x04 | ✅ | 1.0.0.0|  |
| Rssi | 0x05 | ✅ | 0 |  |
| BatteryVoltage | 0x06 | ✅ | 100 |  |
| BatteryType | 0x07 | ✅ | Normal |  |
| ManufacturerName | 0x08 | ✅ | LEGO System A/S |  |
| RadioFirmwareVersion | 0x09 | ✅ | 2.2.1 |  |
| LegoWirelessProtocolVersion | 0x0A | ✅ | 3.0 |  |
| SystemTypeId | 0x0B | ✅ | 0b001_00000 | LegoDuplo_DuploTrain |
| HardwareNetworkId | 0x0C | ✅ | 254 |  |
| PrimaryMacAddress | 0x0D | ✅ | n/a |  |
| SecondaryMacAddress | 0x0E | ❌ |  | throw error |
| HardwareNetworkFamily | 0x0F | ❌ |  | throw error |

## Comments

- Operates either in Automatic (kids pushing around) or Bluetooth Mode
- Many deviations from the exposed the LWP port / port mode information

## Firmware Versions

- 1.6.0.0