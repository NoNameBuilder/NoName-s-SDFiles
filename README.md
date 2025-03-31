# T-Embed CC1101 SD Card Files

Welcome to the **T-Embed CC1101 SD Card Files** repository! This project combines my work with contributions from others to provide all the necessary tools for working with the **LilyGO T-Embed CC1101** board. It utilizes the integrated **CC1101** RF transceiver and an SD card for wireless communication and data storage.

This repository is designed to help you unlock the potential of the **T-Embed CC1101** board for various projects, such as wireless communication, RF data transmission, and data logging with the **ESP32-S3-WROOM-1** microcontroller.

## About the T-Embed CC1101

The **T-Embed CC1101** is a development board based on the **ESP32-S3-WROOM-1** microcontroller, specifically designed for wireless communication. Here are the key features and specifications:

- **Microcontroller (MCU)**: ESP32-S3-WROOM-1
- **Flash Memory**: 16MB
- **PSRAM**: 8MB (great for memory-heavy applications)
- **Wireless Communication**: Integrated **CC1101** RF transceiver for sub-GHz communication
- **NFC**: **PN532** NFC module (Address: 0x24)
- **Display**: 320x170 **ST7789** LCD display
- **Battery**: 3.7V-1300mAh lithium-ion rechargeable battery
- **Battery Management**: **BQ25896** (0x6B) and **BQ27220** (0x55) chips for power management
- **LED Control**: **WS2812** RGB LED driver for customizable lighting effects

This board is ideal for projects involving low-power wireless communication, sensor data logging, and mobile battery-powered applications.

## Arduino IDE Settings

To work with the **T-Embed CC1101** in the **Arduino IDE**, use these configuration settings to ensure proper operation:

- **Board**: ESP32S3 Dev Module
- **Port**: Select your specific port
- **USB CDC On Boot**: Enable
- **CPU Frequency**: 240MHz (WiFi)
- **Core Debug Level**: None
- **USB DFU On Boot**: Disable
- **Erase All Flash Before Sketch Upload**: Disable
- **Events Run On**: Core1
- **Flash Mode**: QIO 80MHz
- **Flash Size**: 16MB (128Mb)
- **Partition Scheme**: 16M Flash (3M APP / 9.9MB FATFS)
- **PSRAM**: OPI PSRAM
- **Upload Mode**: UART0 / Hardware CDC
- **Upload Speed**: 921600
- **USB Mode**: CDC and JTAG

These settings ensure seamless uploading and debugging.

## Features

This repository includes several features to help you get started with the **T-Embed CC1101** board:

- **RF Communication**: Use the integrated **CC1101** RF transceiver for sub-GHz wireless communication.
- **SD Card Support**: Store and manage data on an SD card connected to the ESP32 for long-term storage and logging.
- **Battery Management**: Efficient power management with built-in support for lithium-ion batteries.
- **LED Control**: Control **WS2812** RGB LEDs for custom lighting effects or system status indicators.
- **Easy Setup**: Includes guides and example code to help you quickly start using the T-Embed CC1101.

## Getting Started

### Prerequisites

Before getting started, ensure you have the following:

- **T-Embed CC1101 Development Board**
- **Arduino IDE** installed on your computer
- **CC1101** library installed in the Arduino IDE (included in this repo)
- **SD card** for data storage
- **SPI** and **SD** libraries for communication

### Setup Instructions

#### 1. Install Necessary Libraries

To use the **T-Embed CC1101** board, install the following libraries in the **Arduino IDE**:

- **SPI**: For communication between the **ESP32** and external devices (e.g., **SD card**).
- **SD**: For reading and writing data to the **SD card**.
- **CC1101**: For communication with the integrated **CC1101 RF transceiver**.

To install these libraries:

1. Open the **Arduino IDE**.
2. Go to **Sketch** > **Include Library** > **Manage Libraries**.
3. Search for and install each library (SPI, SD, CC1101).

Alternatively, you can download the **CC1101** library from GitHub and place it in your Arduino libraries folder.

#### 2. Connect the Hardware

The **CC1101** RF transceiver is **integrated** into the **T-Embed CC1101** board, so no external connections are required. Simply insert the **SD card** into the SD card reader slot on the board.

> **Note**: Format your SD card as **FAT32** for compatibility with the **SD** library.

#### 3. Upload Example Code

Once you've installed the libraries and connected the hardware, you can start uploading example code to the **T-Embed CC1101** board.

## Contributing

We welcome contributions! If you'd like to help improve this project, here are a few ways you can contribute:

- **Report Issues**: If you encounter any bugs or issues, please report them in the Issues section of the repository.
- **Suggest Features**: Got an idea for a new feature? We’d love to hear from you!
- **Improve Documentation**: Help make the documentation clearer and more detailed by submitting improvements.
- **Fix Issues**: If you spot any bugs or improvements, fork the repository, make the necessary changes, and submit a pull request.

### How to Contribute

1. Fork the repository by clicking the **Fork** button at the top of this page.
2. Clone your forked repository to your local machine.
3. Create a new branch for your changes.
4. Make your changes, ensuring they follow the existing coding style.
5. Thoroughly test your changes.
6. Submit a pull request describing your changes.

Thank you for contributing and helping make this repository even better!

