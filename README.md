---
description: TBD
title: TBD
keywords:
- Grove
image: TBD
slug: Human Detection Sensor Kit
last_update:
  date: 8-26-2023
  author: Stephen Lo
---


<!-- ![](https://files.seeedstudio.com/wiki/Grove-VOC_and_eCO2_Gas_Sensor-SGP30/img/IMG_0012a.jpg) -->
  <p style={{textAlign: 'center'}}><img src="https://raw.githubusercontent.com/Longan-Labs/XIAO_MMWARE_RES/main/images/5-Human-Detection-Sensor-Kit-45feature.jpg" alt="pir" width={600} height="auto" /></p>

The Human Detection Sensor Kit is more than just a hardware bundle; it's a comprehensive solution for human detection that integrates a variety of advanced technologies and modules. At the heart of this kit are three core components: a 24GHz mmWave Sensor, a XIAO ESP32C3 microcontroller board, and a set of Grove system interfaces. Together, these elements form a highly flexible and scalable platform designed to meet a diverse range of human detection needs.

In terms of functionality, the 24GHz mmWave Sensor serves as the "eyes" of the kit, capable of accurately detecting human presence within a certain range. This feature makes it highly applicable in a variety of scenarios, including but not limited to home security, commercial access control, and health monitoring. The XIAO ESP32C3, on the other hand, acts as the "brain" of the kit. Not only does it offer robust data processing capabilities, but it also supports WiFi and Bluetooth communications, allowing users to easily transmit detection data to other devices or the cloud.

The WiFi capabilities of the XIAO ESP32C3 deserve special mention. Beyond basic data transmission, it supports complex interactions with other IoT devices or services through protocols like MQTT and HTTP. This means you can seamlessly integrate this kit into your existing smart home or enterprise systems for more advanced automation and data analytics.

The inclusion of the Grove system further amplifies the kit's scalability. With simple plug-and-play actions, you can add more Grove modules, such as temperature sensors, cameras, or sound sensors, to achieve more personalized functionalities.

In summary, whether you're a DIY enthusiast, a business in need of a customized solution, or an educational institution focused on research and teaching, the Human Detection Sensor Kit offers a comprehensive, efficient, and user-friendly solution for human detection.

<p style={{textAlign: 'center'}}><a href="https://www.seeedstudio.com/-Grove-VOC-and-eCO2-Gas-Sensor-(SGP30)-p-3071.html" target="_blank"><img src="https://files.seeedstudio.com/wiki/Seeed-WiKi/docs/images/300px-Get_One_Now_Banner-ragular.png" /></a></p>

## Features

- **Modular Design**: The kit employs the Grove system, allowing users to easily add or swap functional modules.
- **Multi-Protocol Support**: The XIAO ESP32C3 supports multiple communication protocols such as MQTT and HTTP, facilitating interaction with other IoT devices or services.
- **High-Precision Human Detection**: The 24GHz mmWave Sensor can accurately detect human presence within a maximum range of 5 meters.
- **Stable Data Processing**: The XIAO ESP32C3 microcontroller, with its 400KB SRAM and robust processing capabilities, ensures stable and reliable data processing.
- **Plug-and-Play**: All components are plug-and-play, eliminating the need for complex setups.

## Specification

- **24GHz mmWave Sensor**
  - Detection Range: Up to 5 meters
  - Operating Frequency: 24GHz
  - Output Interface: I2C
  
- **XIAO ESP32C3**
  - Processor: ESP32C3
  - Memory: 400KB SRAM
  - Communication: WiFi, Bluetooth
  - I/O Ports: Multiple GPIO
  
- **Grove System**
  - Interface Types: Digital, Analog, I2C, UART
  - Power Output: 3.3V (You can only use the 3.3V Grove module)

- **Additional Accessories**
  - USB Cable Length: 1.2 meters
  - Box Dimensions: 100 x 100 x 50 mm
  - Copper Pillars and Screws: 6mm height

## In the Box

![](https://raw.githubusercontent.com/Longan-Labs/XIAO_MMWARE_RES/main/images/6-110061541-mmWave-Human-Detection-Sensor-Kit-fontall.jpg)

This section provides a detailed list of all the components included in the Human Detection Sensor Kit.

- **24GHz mmWave Sensor**: The primary sensor for human detection.
- **Circuit Board with XIAO ESP32C3**: The control unit of the kit, pre-soldered with a XIAO ESP32C3 microcontroller that is equipped with WiFi and Bluetooth capabilities.
- **White Box**: A casing to house the circuit board.
- **Cross Screwdriver**: A tool for assembling the components.
- **1.2m Type C USB Cable**: Used for programming the microcontroller board and for power supply.
- **2 x 3M Double-Sided Tape**: For securing the white box in place.
- **3 x 6mm Copper Pillars and 6 Small Screws**: For mounting Grove modules onto the circuit board.


## Applications

The Human Detection Sensor Kit is versatile and can be adapted for various application scenarios. Below are some ideas to inspire your next project:

#### Home Security

- **Intruder Alert**: Use the kit to detect unauthorized entry into your home and trigger an alarm or notification.
- **Smart Doorbell**: Integrate the kit with a camera to create a smart doorbell that only alerts you when someone is at the door.

#### Commercial Applications

- **Automated Access Control**: Implement the kit in office buildings or factories to control access to restricted areas.
- **Retail Analytics**: Use the sensor to count the number of people entering and exiting a retail store for better customer analytics.

#### Health Monitoring

- **Elderly Care**: Use the kit to monitor the movement of elderly people in a home or care facility, alerting caregivers in case of unusual activity.
- **Occupancy Sensing**: In hospitals, use the kit to detect whether a bed is occupied or not, helping in efficient room management.

#### Industrial Automation

- **Safety Monitoring**: In industrial settings, use the kit to ensure that no one enters hazardous areas without proper authorization.
- **Resource Allocation**: Use the kit to monitor the number of workers in different areas and allocate resources more efficiently.

## Getting Started

This section aims to quickly guide you through the initial setup and basic usage of the Human Detection Sensor Kit. The circuit board of the kit comes pre-soldered with a XIAO ESP32 C3 microcontroller and a 24GHz mmWave sensor. Due to the comprehensive documentation already available for the XIAO ESP32 C3 and 24GHz mmWave Sensor, this section will provide only a brief overview.

### How to Start

1. **XIAO ESP32 C3 Setup**: Since the XIAO ESP32 C3 microcontroller is already soldered onto the circuit board, you can directly refer to the [Wiki page here](https://wiki.seeedstudio.com/XIAO_ESP32C3_Getting_Started/) for setup and programming.

2. **24GHz mmWave Sensor Setup**: Likewise, for setting up and using the 24GHz mmWave sensor, you can refer to the [Wiki page here](https://wiki.seeedstudio.com/Radar_MR24HPC1/).

### Points to Note

- Make sure you have the Arduino IDE installed on your computer.
- Ensure a stable connection between the circuit board and your computer before proceeding with any programming.

### Programming Considerations

1. **Power Control for 24GHz mmWave Sensor**: To conserve power, we've added a switch to control the power supply to the 24GHz mmWave Sensor. You can control it via the D6 pin on the XIAO ESP32 C3. To turn the sensor on, include `digitalWrite(D6, HIGH)` in your code. To turn it off, use `digitalWrite(D6, LOW)`.

2. **Serial Communication**: The D2 pin of the XIAO ESP32C3 is connected as TX to the RX of the 24GHz mmWave Sensor, and the D3 pin is connected as RX to the TX of the sensor. Therefore, include the following in your `setup()` function:  
   `Serial1.begin(115200, SERIAL_8N1, D3, D2);`

3. **Example Code**: Below is a simple example that you can also find in the 24GHz mmWave Sensor's Wiki. Due to the points mentioned above, the code will have some differences.

```arduino
#include "Arduino.h"
#include <humanstaticLite.h>

HumanStaticLite radar = HumanStaticLite(&Serial1);
const int pinPwrCtrl  = D6;

void setup() {
  Serial.begin(115200);
  Serial1.begin(115200, SERIAL_8N1, D3, D2);    // init the Serial1
  pinMode(pinPwrCtrl, OUTPUT);
  
  digitalWrite(pinPwrCtrl, HIGH);           // Open power to the mmWare sensor

  while(!Serial);
  Serial.println("Ready");
}

void loop() {
  radar.recvRadarBytes();
  radar.showData();
  delay(200);
}
```

For all code related to the 24GHz mmWave Sensor, you will need to make similar modifications as shown in the example code above.

## Schematic Online Viewer

<div className="altium-ecad-viewer" data-project-src="https://github.com/Longan-Labs/XIAO_MMWARE_RES/raw/main/Human_Detection_Sensor_Board.zip" style={{borderRadius: '0px 0px 4px 4px', height: 500, borderStyle: 'solid', borderWidth: 1, borderColor: 'rgb(241, 241, 241)', overflow: 'hidden', maxWidth: 1280, maxHeight: 700, boxSizing: 'border-box'}}>
</div>

## Resources

- [Eagle File](https://github.com/Longan-Labs/XIAO_MMWARE_RES/raw/main/Human_Detection_Sensor_Board.zip)
- [Wiki for XIAO ESP32 C3](https://wiki.seeedstudio.com/XIAO_ESP32C3_Getting_Started/)
- [Wiki for 24GHz mmWare Sensor](https://wiki.seeedstudio.com/Radar_MR24HPC1/)

## Tech Support
If you have any technical issue.  submit the issue into our [forum](https://forum.seeedstudio.com/).