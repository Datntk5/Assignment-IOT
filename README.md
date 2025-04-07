# Assignment-IOT
# Fruit Recognition IoT Project

This project uses **ESP32-CAM** to recognize various types of fruits using an **Edge Impulse** machine learning model. The recognition results are sent via **Telegram** and stored in **Firebase** for easy access and management. The system also supports sending status notifications via Telegram.

## System Configuration

### Hardware

- **ESP32-CAM**: The device used for capturing fruit images.
- **OV2640 Camera**: Camera used on the ESP32-CAM.
- **LCD OLED Display (Optional)**: Used to display system status (if needed).

### Software

- **Edge Impulse**: The platform used to train the fruit recognition image model.
- **Firebase**: The database used to store recognition results.
- **Telegram Bot**: Sends notifications and recognition results to the user via Telegram.

## Software Requirements

### Library Installation

The following libraries are required for this project:

```cpp
#include <WiFi.h>
#include <WiFiClientSecure.h>
#include <UniversalTelegramBot.h>
#include <FirebaseESP32.h>
