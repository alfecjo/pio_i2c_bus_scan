# PIO I²C Bus [Scanner](https://github.com/alfecjo/pio_i2c_bus_scan/releases/tag/v1.0.0) for Raspberry Pi Pico

This `.uf2` firmware performs a full scan of the I²C bus using the Raspberry Pi Pico’s PIO (Programmable I/O) instead of the built-in I²C peripheral. It identifies which devices are connected and responding to valid 7-bit I²C addresses.

---

## 📦 Features

- Automatic scan of all valid 7-bit I²C addresses.
- Uses PIO-based I²C implementation.
- Pinout:
  - SDA: GPIO2  
  - SCL: GPIO3
- Tested with multiple I²C sensors and displays.
- Scan results printed via USB serial.

---

## 🔧 How to Use

1. Connect your I²C device to GPIO2 (SDA) and GPIO3 (SCL).
2. Ensure 4.7 kΩ pull-up resistors (or similar) are present on the bus.
3. Drag and drop this `.uf2` onto your Pico while in bootloader mode.
4. Open a serial monitor at 115200 baud.
5. Detected I²C addresses will be printed to the terminal.

---

## 🖨️ Sample Output

![Scan I2C](https://github.com/alfecjo/pio_i2c_bus_scan/blob/main/Scan.png)
