# PIO I²C Bus [Scanner](https://github.com/alfecjo/pio_i2c_bus_scan/releases/tag/v1.0.0) para Raspberry Pi Pico

Este firmware `.uf2` realiza a varredura completa do barramento I²C utilizando a PIO (Programmable I/O) do Raspberry Pi Pico. Ele identifica quais dispositivos estão conectados e respondem a endereços válidos.

---

## 📦 Funcionalidades

-  Varredura automática de todos os endereços válidos I²C (7 bits).
-  Usa implementação PIO (em vez do I²C hardware nativo).
-  Pinos utilizados:
  - SDA: GPIO2  
  - SCL: GPIO3
-  Testado com múltiplos sensores e displays I²C.
-  Resultados exibidos via porta serial (USB).

---

## Como usar

1. Conecte seu dispositivo I²C aos pinos 2 (SDA) e 3 (SCL) do Pico.
2. Garanta resistores de *pull-up* de 4.7 kΩ ou similares no barramento.
3. Arraste este `.uf2` para o Pico em modo bootloader.
4. Abra um monitor serial (baud rate 115200).
5. Veja os endereços detectados impressos no terminal.

---

## Exemplo de saída:

![Scan I2C](https://github.com/alfecjo/pio_i2c_bus_scan/blob/main/Scan.png)
