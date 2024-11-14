# Portenta H7 LED Control Web Server

This project demonstrates how to create a simple web server on the Arduino Portenta H7 that can be controlled by a phone or any device connected to the same network. The server provides a web interface with buttons to control the red, green, and blue LEDs on the Portenta H7.

## Features

- Control red, green, and blue LEDs via a web interface
- Hosted on the Arduino Portenta H7
- Accessible from any device connected to the same network
- Visual feedback on the web page for LED states

## Getting Started

### Prerequisites

- Arduino IDE installed on your computer
- Portenta H7 board support package installed in the Arduino IDE
- Arduino Portenta H7 board
- USB-C cable for programming

### Installation

1. **Clone the repository:**

    ```sh
    git clone https://github.com/yourusername/portenta-h7-led-control.git
    cd portenta-h7-led-control
    ```

2. **Open the project in Arduino IDE:**

    - Open the `SimpleWebServer.ino/SimpleWebServer.ino.ino` file in the Arduino IDE.

3. **Configure Wi-Fi credentials:**

    - Open the `SimpleWebServer.ino/arduino_secrets.h` file and update the `SECRET_SSID` and `SECRET_PASS` with your network credentials

.



    ```cpp
    #define SECRET_SSID "YourNetworkSSID"
    #define SECRET_PASS "YourNetworkPassword"
    ```

4. **Upload the sketch:**

    - Connect your Portenta H7 to your computer using the USB-C cable.
    - Select "Arduino Portenta H7 (M7 core)" as the board in the Arduino IDE.
    - Click the upload button to upload the sketch to the board.

### Usage

1. **Connect to the Access Point:**

    - After uploading the sketch, the Portenta H7 will create a Wi-Fi access point with the SSID you configured.
    - Connect your phone or any device to this access point.

2. **Access the Web Interface:**

    - Open a web browser on your connected device.
    - Enter the IP address displayed in the serial monitor (e.g., `http://192.168.3.1`).

3. **Control the LEDs:**

    - Use the buttons on the web page to turn the red, green, and blue LEDs on and off.


```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Created by Carl Kho for CAETI @ UAI using Arduino Portenta H7
- Inspired by the Arduino examples and documentation
