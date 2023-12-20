# NFC_Module
The NFC module is an excellent solution for enthusiasts, makers, and developers who want to harness the power of NFC technology, whether it's for prototyping or building advanced applications, the NFC module delivers the functionality, reliability, and flexibility needed for a wide range of projects.
The term "NFC" refers to a short-range, high-frequency wireless communication technology that is mostly used in mobile or portable devices. It enables radio connection to be established by just touching two phones together or keeping them a few millimeters apart. Holding two devices together and using a wireless communication link for the final few centimeters makes choosing a target straightforward. Induction-coupling, which uses magnetic induction between two loop antennas operating at a frequency of 13.56MHZ with data rates ranging from 106 kbit/s to 424 kbit/s, is the primary communication method used in NFC. 

This github provides instructions to get started with NFC module.
### Features:
- Adopt special base station RF chip, stable performance, good compatibility
- Both Read/Write operation possible
- Integrated Antenna
- Communication Interface: TTL
- Support Protocols like ISO14443B, ISO18092
- Contactless card supports like NTAG213, Mifare one S50, Mifare one S70, ultralight, FM11RF08

### Specifications:
- NFC Module Frequency: 13.56MHz
- Reading Distance: >50mm (The effective distance is related to the IC card and the use environment)
- Reading Time: <200ms
- Output Format: TTL
- Size: 28.9 x 28.9mm
- Supply: 5V DC
- Operating Current: 50mA
- Operating Temperature: -15°C to +55°C
- Storage Temperature: -20°C to +70°C

## Getting Started with NFC module
### Pinout 

<img src="https://github.com/sbcshop/NFC_Module/blob/main/images/nfc_pinout.jpg">

- (1) 5V
- (2) GND
- (3) RXD
- (4) TXD

### NFC module USB to TTL Hardware Connection

  - Here you will need NFC module with any USB to TTL converter, for this guide we are using one which available [here](https://shop.sb-components.co.uk/products/usb-ttl?variant=40312245059667).

    |USB to TTL (CP2102 Variants) | NFC Module | Function |
    |---|---|---|
    |VCC | 5V | Positive Supply |
    |GND | GND | Ground |
    |TXD | TXD | UART Connection | 
    |RXD | RXD | UART Connection |

    |USB to TTL (CH340 Variants) | NFC Module | Function |
    |---|---|---|
    |VCC | 5V | Positive Supply |
    |GND | GND | Ground |
    |TXD | RXD | UART Connection | 
    |RXD | TXD | UART Connection |

    **Note:** Do cross connection of UART pins if module won't respond or showing connection failed in software application

    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/NFCmodule_ttl.png" width="447" height="321">

    Other NFC Module pins:
    | NFC Module | Function |
    |---|---|
    | SEL | Reserved |
    | BUZ | Pulse generated when card scan |
    | ANT1 | Dual Antenna 1 | 
    | ANT2 | Dual Antenna 2 |
    
     **Note:** BUZ pin -> when a card is detected, the signal goes from a high state to a low state and then back to a high state again.
    
  - Once the NFC Module and USB-TTL converter are connected, attach the converter to the USB port of the computer or laptop and check your COM Port in device manager.
    
    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/device_manager_comport_view.png" width="584" height="425">

    If you don't have CH340 driver installed in PC/laptop, then checkout [CH340 Driver Installation Manual Guide](https://github.com/sbcshop/NFC_Module/blob/main/documents/CH340%20Driver%20installation%20steps.pdf).
    
  - Download software folder provided [here](https://github.com/sbcshop/NFC_Module/tree/main/softwares), and run .exe file, so you will see below interface of software.
    
    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/software_interface.png" width="569" height="293">

  - Checkout [Manual](https://github.com/sbcshop/NFC_Module/blob/main/documents/NFC%20Module%20Software%20Usage%20Instruction%20Manual.pdf) having instructions how to use NFC module with software for setup and configuration.

 ### NFC module with Raspberry Pi Pico
   - Follow the below connection to use NFC module with Pico/ Pico W
     
      |Pico | NFC Module | Function |
      |---|---|---|
      |VBUS | 5V | Positive Supply |
      |GND | GND | Ground |
      |GP4 | RX | Serial UART connection |
      |GP5 | TX  | Serial UART connection |

     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/NFC_pico_interfacing.png" width="420" height="323">
     
   - After this you can follow same example and instructions available on [ReadPi NFC GitHub](https://github.com/sbcshop/ReadPi_NFC_Software/tree/main#example-codes) related to NFC operations.

 ## Resources
  * [NFC Module Command Manual](https://github.com/sbcshop/ReadPi_NFC_Software/blob/main/documents/NFC%20Module%20command%20Manual.pdf)
  * [NTAG213/215/216 Datasheet](https://github.com/sbcshop/ReadPi_NFC_Software/blob/main/documents/NTAG213_215_216.pdf)
  * [MicroPython getting started for RPi Pico/Pico W](https://docs.micropython.org/en/latest/rp2/quickref.html)
  * [Pico W Getting Started](https://projects.raspberrypi.org/en/projects/get-started-pico-w)

## Related Products
   * [ReadPi NFC](https://shop.sb-components.co.uk/products/readpi-an-rfid-nfc-reader-powered-with-raspberry-pi-pico-w?variant=40478483087443) - ReadPi with 13.56MHz NFC reader/writer powered by Raspberry Pi Pico W
   * [ReadPi RFID](https://shop.sb-components.co.uk/products/readpi-an-rfid-nfc-reader-powered-with-raspberry-pi-pico-w?variant=40478483054675) - ReadPi with 125KHz RFID powered by Raspberry Pi Pico W
   * [Raspberry Pi Pico RFID expansion](https://shop.sb-components.co.uk/products/raspberry-pi-pico-rfid-expansion) - RFID expansion board with support to incorporate Pico/Pico W 
   * [RFID_Breakout](https://shop.sb-components.co.uk/products/rfid-breakout?_pos=5&_sid=fac219786&_ss=r) - RFID breakout for standalone testing and freedom to choose microcontroller as per requirement.

## Product License

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>     
     

    
    


