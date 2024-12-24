# USB2UART Programmer with BOOT and EN/RESET Buttons

This project provides a simple USB to UART programmer that integrates useful features for programming microcontrollers. It is based on the FTDI FT230 chip and features USB Type-C connectivity, BOOT and EN/RESET buttons, as well as multiple connector options including a UART header and a TC2030 connector.

---

## Features

1. **USB Type-C Connector**
   - Modern and versatile USB interface for power and data transfer.

2. **FTDI FT230 Chip**
   - Reliable USB to UART communication.
   - Supports various baud rates and low-latency operation.

3. **BOOT and EN/RESET Buttons**
   - Simplifies the programming process by providing dedicated buttons:
     - **BOOT**: Configures the microcontroller for firmware upload.
     - **EN/RESET**: Resets the microcontroller or triggers a reinitialization.

4. **UART Header**
   - Standard 4-pin UART header for easy interfacing with target devices.

5. **TC2030 Connector**
   - Additional programming interface for Tag-Connect cable compatibility.

---

## Applications

- Programming microcontrollers such as ESP32, STM32, and similar.
- Debugging embedded systems.
- Prototyping and testing UART-based devices.

---

## Hardware Components

1. **FTDI FT230 Chip**
   - Manages USB to UART communication.
2. **USB Type-C Connector**
   - Ensures robust and reversible connections.
3. **Push Buttons**
   - **BOOT**: Activates bootloader mode.
   - **EN/RESET**: Triggers a reset of the target device.
4. **Connectors**
   - **UART Header**: Pinout: VCC, TXD, RXD, GND.
   - **TC2030 Connector**: 6-pin layout compatible with Tag-Connect cables.

---

## Pinout

### UART Header:
| Pin | Signal  |
|-----|---------|
| 1   | VCC     |
| 2   | RXD     |
| 3   | TXD     |
| 4   | GND     |

### TC2030 Connector:
| Pin | Signal  |
|-----|---------|
| 1   | VCC     |
| 2   | GND     |
| 3   | EN      |
| 4   | BOOT     |
| 5   | TXD    |
| 6   | RXD    |

---

## Schematic Overview

Include a detailed schematic diagram here or attach it to your repository to provide users with the hardware details.
![image](https://github.com/user-attachments/assets/ae22d539-2bf9-4187-adec-e5b2eaf938aa)

---

## Usage Instructions

1. **Connect the Programmer**
   - Plug the USB Type-C cable into your computer and the programmer.
   - Connect the UART header or TC2030 connector to your target device.

2. **Install Drivers**
   - Ensure FTDI drivers are installed on your computer. These can be downloaded from the [FTDI website](https://www.ftdichip.com/).

3. **Programming**
   - Press the BOOT button while resetting the device with the EN/RESET button to enter bootloader mode.
   - Use your preferred programming tool (e.g., esptool.py, STM32CubeProgrammer).

4. **Debugging**
   - Monitor UART communication using any serial terminal application.

---

## Additional Notes

- Ensure the target device’s UART voltage levels are compatible with the FT230’s logic level (typically 3.3V).
- The TC2030 connector is designed for Tag-Connect cables, making it ideal for quick and reliable programming connections without the need for soldering headers.
- Use quality USB Type-C cables to ensure stable power and data transmission.
- USB2UART device also has a 3.3V voltage regulator to allow for powering of devices if they are not 5V compatible.

---

## License

This project is open-source under the [GNU Public License](LICENSE). Feel free to modify and use it in your projects.
