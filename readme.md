# EIDOTHEA DEVBOARD

The **Eidothea DevBoard** is designed for testing and development, compatible with the [Eidothea Board](https://github.com/tobsec/eidothea). It can be used both on a test bench and within an engine setup.

![Eidothea DevBoard](https://github.com/tobsec/eidothea-devboard/blob/main/doc/eidothea_devBoard.png?raw=true)

## Hardware Features

### Connectors

- **Sicma 56 Connector**: A weatherproof connector available on [AliExpress](https://aliexpress.com/item/32857771975.html).
- **Connector with 20cm Wiring Harness**: This is available for connecting to the Eidothea Board, also on [AliExpress](https://aliexpress.com/item/1005007332736311.html).

### Connectivity

- **2x CAN Bus Ports**: Available via SubD9 connectors (120Ω selectable).
- **Engine Connections**: All engine connections can be interrupted or disconnected as needed.
- **Pin Headers**: All signals are available on pin headers for easy probing or signal injection.

### Features

- **Ignition Toggle Switch**: For bench testing purposes.
- **Main Power Relay**: For controlling power during testing.
- **Analog Channel Emulation**: Analog channels can be emulated using potentiometers for simulation.

## Pinout
| No. | Pin                   | Description                | IN / OUT | Function                |
|-----|-----------------------|----------------------------|----------|-------------------------|
| 1   | IGN1                  | Ignition Trigger 1         | OUT      | Gate Driver IC          |
| 2   | IGN2                  | Ignition Trigger 2         | OUT      | Gate Driver IC          |
| 3   | IGN3                  | Ignition Trigger 3         | OUT      | Gate Driver IC          |
| 4   | IGN4                  | Ignition Trigger 4         | OUT      | Gate Driver IC          |
| 5   | IGN5                  | Ignition Trigger 5         | OUT      | Gate Driver IC          |
| 6   | IGN6                  | Ignition Trigger 6         | OUT      | Gate Driver IC          |
| 7   | IGN7                  | Ignition Trigger 7         | OUT      | Gate Driver IC          |
| 8   | IGN8                  | Ignition Trigger 8         | OUT      | Gate Driver IC          |
| 9   | GND                   | GND                        | IN       | Supply                  |
| 10  | GND                   | GND                        | IN       | Supply                  |
| 11  | GND                   | GND                        | IN       | Supply                  |
| 12  | DIGITAL_3             | Start Switch/Button Signal | IN       | Digital In 12V          |
| 13  | DIGITAL_VR_1          | Crank Sensor               | IN       | HALL / VR In            |
| 14  | DIGITAL_VR_4          | Cam Sensor                 | IN       | HALL / VR In            |
| 15  | LS4                   | Injector 4                 | OUT      | Low Side Switch         |
| 16  | LS3                   | Injector 3                 | OUT      | Low Side Switch         |
| 17  | LS2                   | Injector 2                 | OUT      | Low Side Switch         |
| 18  | LS1                   | Injector 1                 | OUT      | Low Side Switch         |
| 19  | LS9                   | Spare (e.g. Boost Control) | OUT      | Low Side Switch         |
| 20  | LS10                  | Main Relay Drive           | OUT      | Low Side Switch         |
| 21  | GND                   | Knock Sensor 2 -           | IN       | Knock Sensing           |
| 22  | LS5                   | Injector 5                 | OUT      | Low Side Switch         |
| 23  | LS6                   | Injector 6                 | OUT      | Low Side Switch         |
| 24  | LS7                   | Injector 7                 | OUT      | Low Side Switch         |
| 25  | LS8                   | Injector 8                 | OUT      | Low Side Switch         |
| 26  | 12V_RAW (+ DIGITAL_2) | Ignition (KL15)            | IN       | Supply                  |
| 27  | ETB1-                 | ETB M- / Idle Stepper A2   | OUT      | H Bridge (opt. Stepper) |
| 28  | ETB1+                 | ETB M+ / Idle Stepper A1   | OUT      | H Bridge (opt. Stepper) |
| 29  | CAN+                  | CAN1 H                     | IN / OUT | O2 Sensor CAN (500kbps) |
| 30  | CAN-                  | CAN1 L                     | IN / OUT | O2 Sensor CAN (500kbps) |
| 31  | CAN2+                 | CAN2 H                     | IN / OUT | NMEA2000 CAN (250kbps)  |
| 32  | CAN2-                 | CAN2 L                     | IN / OUT | NMEA2000 CAN (250kbps)  |
| 33  | KNOCK_2               | Knock Sensor 2 +           | IN       | Knock Sensing           |
| 34  | AT1                   | Water Temperature Sensor   | IN       | Analog Temp             |
| 35  | AV9                   | PPS2 (Idle Stepper B2)     | IN (OUT) | Analog  (opt. Stepper)  |
| 36  | AV8                   | PPS1 (Idle Stepper B1)     | IN (OUT) | Analog  (opt. Stepper)  |
| 37  | AV6                   | ETB TPS2                   | IN       | Analog Voltage          |
| 38  | AV3                   | Water Pressure Sensor      | IN       | Analog Voltage          |
| 39  | AV5                   | ETB TPS1                   | IN       | Analog Voltage          |
| 40  | LS11_F                | Tacho Out                  | OUT      | Low Side + PullUp       |
| 41  | LS15_F                | Starter Relay Drive        | OUT      | Low Side Switch         |
| 42  | LS13_F                | ~Main Relay Drive~ Spare   | OUT      | Low Side Switch         |
| 43  | 12V_MR                | Power (from Main Relay)    | IN       | Supply                  |
| 44  | 12V_MR                | Power (from Main Relay)    | IN       | Supply                  |
| 45  | 5V_SENSOR_1           | Sensor Supply 5V           | OUT      | Analog Supply 150mA     |
| 46  | GND                   | Sensor GND                 | OUT      | Analog GND              |
| 47  | KNOCK_1               | Knock Sensor 1 +           | IN       | Knock Sensing           |
| 48  | GND                   | Knock Sensor 1 -           | IN       | Knock Sensing           |
| 49  | AT2                   | Oil Temperature Sensor     | IN       | Analog Temp             |
| 50  | AV7                   | Fuel Pressure Sensor       | IN       | Analog Voltage          |
| 51  | AV2                   | IAT Sensor                 | IN       | Analog ~Voltage~ Temp   |
| 52  | AV4                   | Oil Pressure Sensor        | IN       | Analog Voltage          |
| 53  | AV1                   | MAP Sensor                 | IN       | Analog Voltage          |
| 54  | LS12_F                | Audio Warning Horn / MIL   | OUT      | Low Side Switch         |
| 55  | LS16_F                | Fuel Pump Relay Drive      | OUT      | Low Side Switch         |
| 56  | LS14_F                | Spare (e.g. Boost Control) | OUT      | Low Side Switch         |
