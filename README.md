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
- **High-Precision Human Detection**: The 24GHz mmWave Sensor can accurately detect human presence within a maximum range of 30 meters.
- **Stable Data Processing**: The XIAO ESP32C3 microcontroller, with its 400KB SRAM and robust processing capabilities, ensures stable and reliable data processing.
- **Plug-and-Play**: All components are plug-and-play, eliminating the need for complex setups.

## Specification

- **24GHz mmWave Sensor**
  - Detection Range: Up to 30 meters
  - Operating Frequency: 24GHz
  - Output Interface: I2C
  
- **XIAO ESP32C3**
  - Processor: ESP32C3
  - Memory: 400KB SRAM
  - Communication: WiFi, Bluetooth
  - I/O Ports: Multiple GPIO
  
- **Grove System**
  - Interface Types: Digital, Analog, I2C, UART
  - Power Requirements: 3.3V or 5V

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


## Hardware Overview

### Pin Map

<!-- ![](https://raw.githubusercontent.com/Longan-Labs/D7S_SENSOR_RES/main/images/pinmap.png) -->
  <p style={{textAlign: 'center'}}><img src="https://raw.githubusercontent.com/Longan-Labs/D7S_SENSOR_RES/main/images/pinmap.png" alt="pir" width={600} height="auto" /></p>

## Getting Started

:::note
    If this is the first time you work with Arduino, we strongly recommend you to see [Getting Started with Arduino](https://wiki.seeedstudio.com/Getting_Started_with_Arduino/) before the start.
:::

### Play With Arduino

#### Hardware

**Materials required**

| Seeeduino V4.2 | Base Shield| Grove - D7S Vibration Sensor |
|--------------|-------------|-----------------|
|<p><img src="https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_1.jpg" alt="pir" width={600} height="auto" /></p>|<p><img src="https://files.seeedstudio.com/wiki/Grove_Light_Sensor/images/gs_4.jpg" alt="pir" width={600} height="auto" /></p>|<p><img src="https://raw.githubusercontent.com/Longan-Labs/D7S_SENSOR_RES/main/images/small.jpg" alt="pir" width={500} height="auto" /></p>|
|<a href="https://www.seeedstudio.com/Seeeduino-V4.2-p-2517.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/Base-Shield-V2-p-1378.html" target="_blank">Get One Now</a>|<a href="https://www.seeedstudio.com/-Grove-VOC-and-eCO2-Gas-Sensor-(SGP30)-p-3071.html" target="_blank">Get One Now</a>|

:::note
    **1** Please plug the USB cable gently, otherwise you may damage the port. Please use the USB cable with 4 wires inside, the 2 wires cable can't transfer data. If you are not sure about the wire you have, you can click [here](https://www.seeedstudio.com/Micro-USB-Cable-48cm-p-1475.html) to buy
    
    **2** Each Grove module comes with a Grove cable when you buy. In case you lose the Grove cable, you can click [here](https://www.seeedstudio.com/Grove-Universal-4-Pin-Buckled-20cm-Cable-%285-PCs-pack%29-p-936.html) to buy.
:::

- **Step 1.** Connect Grove - D7S Vibration Sensor to **I2C** port of Grove-Base Shield.

- **Step 2.** Plug Grove - Base Shield into Seeeduino.

- **Step 3.** Connect Seeeduino to PC via a USB cable.


| Seeeduino     | Grove - D7S Vibration Sensor |
|---------------|-------------------------|
| 3.3/5V        | Red                     |
| GND           | Black                   |
| SDA           | White                   |
| SCL           | Yellow                  |

#### Software

- **Step 1.** Download the [Grove - D7S Vibration Sensor](https://github.com/Longan-Labs/d7s-grove-arduino) from Github.

- **Step 2.** Refer to [How to install library](https://wiki.seeedstudio.com/How_to_install_Arduino_Library) to install library for Arduino.

- **Step 3.** After downloading and installing the library correctly, you can find an example program named sample.ino in the examples folder. This program is designed for the D7S module.

```Arduino
#include <D7S.h>

//old earthquake data
float oldSI = 0;
float oldPGA = 0;

//flag variables to handle collapse/shutoff only one time during an earthquake
bool shutoffHandled = false;
bool collapseHandled = false;

//function to handle collapse event
void handleCollapse()
{
    //put here the code to handle the collapse event
    Serial.println("-------------------- COLLAPSE! --------------------");
}

void setup()
{
    // Open serial communications and wait for port to open:
    Serial.begin(9600);
    while (!Serial)
    {
        ; // wait for serial port to connect. Needed for native USB port only
    }

    Serial.print("Starting D7S communications (it may take some time)...");
    //start D7S connection
    D7S.begin();
    //wait until the D7S is ready
    while (!D7S.isReady())
    {
        Serial.print(".");
        delay(500);
    }
    Serial.println("STARTED");

    //setting the D7S to switch the axis at inizialization time
    Serial.println("Setting D7S sensor to switch axis at inizialization time.");
    D7S.setAxis(SWITCH_AT_INSTALLATION);

    Serial.println("Initializing the D7S sensor in 2 seconds. Please keep it steady during the initializing process.");
    delay(2000);
    Serial.print("Initializing...");
    //start the initial installation procedure
    D7S.initialize();
    //wait until the D7S is ready (the initializing process is ended)
    while (!D7S.isReady())
    {
        Serial.print(".");
        delay(500);
    }
    Serial.println("INITIALIZED!");

    //check if there there was a collapse (if this is the first time the D7S is put in place the installation data may be wrong)
    if (D7S.isInCollapse())
    {
        handleCollapse();
    }

    //reset the events shutoff/collapse memorized into the D7S
    D7S.resetEvents();

    Serial.println("\nListening for earthquakes!");
}

void loop()
{

    //checking if there is an earthquake occuring right now
    if (D7S.isEarthquakeOccuring())
    {

        //check if the shutoff event has been handled and if the shutoff condition is met
        //the call of D7S.isInShutoff() is executed after to prevent useless I2C call
        if (!collapseHandled && D7S.isInCollapse())
        {
            handleCollapse();
            collapseHandled = true;
        }

        //print information about the current earthquake
        float currentSI = D7S.getInstantaneusSI();
        float currentPGA = D7S.getInstantaneusPGA();

        if (currentSI > oldSI || currentPGA > oldPGA)
        {
            //getting instantaneus SI
            Serial.print("\tInstantaneus SI: ");
            Serial.print(currentSI);
            Serial.println(" [m/s]");

            //getting instantaneus PGA
            Serial.print("\tInstantaneus PGA (Peak Ground Acceleration): ");
            Serial.print(currentPGA);
            Serial.println(" [m/s^2]\n");

            //save the current data
            oldSI = currentSI;
            oldPGA = currentPGA;
        }
    }
    else
    {
        //reset the old earthquake data
        oldPGA = 0;
        oldSI = 0;
        //reset the flag of the handled events
        shutoffHandled = false;
        collapseHandled = false;
        //reset D7S events
        D7S.resetEvents();
    }
}
```

- **Step 4.** Upload the demo. If you do not know how to upload the code, please check [How to upload code](https://wiki.seeedstudio.com/Upload_Code/).

- **Step 5.** Open the **Serial Monitor** of Arduino IDE by click **Tool-> Serial Monitor**. you can generate some vibrations, for example, by tapping the table, and you will obtain the following results.

![](https://raw.githubusercontent.com/Longan-Labs/D7S_SENSOR_RES/main/images/result.png)

## Schematic Online Viewer

<div className="altium-ecad-viewer" data-project-src="https://github.com/Longan-Labs/D7S_SENSOR_RES/raw/main/D7S%20Vibration%20Sensor.zip" style={{borderRadius: '0px 0px 4px 4px', height: 500, borderStyle: 'solid', borderWidth: 1, borderColor: 'rgb(241, 241, 241)', overflow: 'hidden', maxWidth: 1280, maxHeight: 700, boxSizing: 'border-box'}}>
</div>

## Resources

- **[Zip]** [Grove - D7S Vibration Sensor](https://github.com/Longan-Labs/D7S_SENSOR_RES/raw/main/D7S%20Vibration%20Sensor.zip)
- **[PDF]** [D7S Datasheet](https://github.com/Longan-Labs/D7S_SENSOR_RES/blob/main/en-d7s-957666.pdf)
- **[GITHUB]** [D7S Arduino Library](https://github.com/Longan-Labs/d7s-grove-arduino)

## Tech Support
If you have any technical issue.  submit the issue into our [forum](https://forum.seeedstudio.com/).