# NFC_Breakout

<img src="https://github.com/sbcshop/NFC_Breakout_Software/blob/main/images/nfc%20breakout%20front.png" width="380" height="420">

The NFC module is an excellent solution for enthusiasts, makers, and developers who want to harness the power of NFC technology, whether it's for prototyping or building advanced applications, the NFC module delivers the functionality, reliability, and flexibility needed for a wide range of projects.
The term "NFC" refers to a short-range, high-frequency wireless communication technology that is mostly used in mobile or portable devices. It enables radio connection to be established by just touching two phones together or keeping them a few millimeters apart. Holding two devices together and using a wireless communication link for the final few centimeters makes choosing a target straightforward. Induction-coupling, which uses magnetic induction between two loop antennas operating at a frequency of 13.56MHZ with data rates ranging from 106 kbit/s to 424 kbit/s, is the primary communication method used in NFC. 

This Github provides instructions to get started with the NFC module.
### Features:
- Adopt special base station RF chip, stable performance, good compatibility
- Both Read/Write operation possible
- Integrated Antenna
- Communication Interface: TTL
- Support Protocols like ISO14443B, ISO18092
- Contactless card supports like NTAG213, Mifare one S50, Mifare one S70, ultralight, FM11RF08
-  Multi-tune Buzzer to add audio alert into the project
-  Status LED for board power, and Tag Scan indication
-  USB (power and UART)
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

## Getting Started with NFC Module
### Pinout 

<img src="https://github.com/sbcshop/NFC_Breakout_Software/blob/main/images/img1.png">

### NFC Breakout Connection
  <img src = "https://github.com/sbcshop/NFC_Breakout_Software/blob/main/images/breakout%20usb.png">
  - Here you will need to connect Type C to the expansion board.
    
**Note:** BUZ pin -> When a card is detected, the signal goes from a high state to a low state and then back to a high state again.
    
  - Once the NFC Breakout is connected, check your COM Port in the device manager.
    
    <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/device_manager_comport_view.png" width="584" height="425">

    If you don't have the CH340 driver installed on your PC/laptop, then check out [CH340 Driver Installation Manual Guide](https://github.com/sbcshop/NFC_Module/blob/main/documents/CH340%20Driver%20installation%20steps.pdf).
    
  - Download the software folder provided [here](https://github.com/sbcshop/NFC_Module/tree/main/softwares), and run the .exe file, so you will see the below interface of the software.
    
     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/software_interface.png">
     
     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/img12.png"> 
     
     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/img_1.JPG">
     
     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/img13.JPG">
     
     <img src="https://github.com/sbcshop/NFC_Module/blob/main/images/img15.JPG">

  - Checkout [Manual](https://github.com/sbcshop/NFC_Module/blob/main/documents/NFC%20Module%20Software%20Usage%20Instruction%20Manual.pdf) having instructions on how to use the NFC module with software for setup and configuration.

 ### NFC module with Raspberry Pi Pico
   - Follow the below connection to use the NFC module with Pico/ Pico W
     
      |Pico | NFC Module | Function |
      |---|---|---|
      |VBUS | 5V | Positive Supply |
      |GND | GND | Ground |
      |GP0 | RX | Serial UART connection |
      |GP1 | TX  | Serial UART connection |

     
   - After this, you can follow the same example (code) and instructions available on [Pico  NFC Expansion GitHub](https://github.com/sbcshop/Pico_NFC_Expansion_Software/tree/main/examples) related to NFC operations.

 ## Resources
  * [Hardware data](https://github.com/sbcshop/NFC_Breakout_Hardware)
  * [NFC Module Command Manual](https://github.com/sbcshop/ReadPi_NFC_Software/blob/main/documents/NFC%20Module%20command%20Manual.pdf)
  * [NTAG213/215/216 Datasheet](https://github.com/sbcshop/ReadPi_NFC_Software/blob/main/documents/NTAG213_215_216.pdf)
  * [MicroPython getting started for RPi Pico/Pico W](https://docs.micropython.org/en/latest/rp2/quickref.html)
  * [Pico W Getting Started](https://projects.raspberrypi.org/en/projects/get-started-pico-w)

## Related Products 
   * [Pico NFC Expansion](https://shop.sb-components.co.uk/products/nfc-expansion-for-raspberry-pi-pico?_pos=6&_sid=02d74a383&_ss=r) -  Expansion for Pico
   * [NFC Breakout](https://shop.sb-components.co.uk/products/nfc-breakout-board?_pos=5&_sid=02d74a383&_ss=r)
   * [Pico NFC HAT](https://shop.sb-components.co.uk/products/pinfc-nfc-hat-for-raspberry-pi?_pos=7&_sid=02d74a383&_ss=r) - HAT for raspberry pi
   * [ReadPi NFC](https://shop.sb-components.co.uk/products/readpi-an-rfid-nfc-reader-powered-with-raspberry-pi-pico-w?variant=40478483087443) - ReadPi with 13.56MHz NFC reader/writer powered by Raspberry Pi Pico W
   * [ReadPi RFID](https://shop.sb-components.co.uk/products/readpi-an-rfid-nfc-reader-powered-with-raspberry-pi-pico-w?variant=40478483054675) - ReadPi with 125KHz RFID powered by Raspberry Pi Pico W
   * [Raspberry Pi Pico RFID expansion](https://shop.sb-components.co.uk/products/raspberry-pi-pico-rfid-expansion) - RFID expansion board with support to incorporate Pico/Pico W 
   * [RFID_Breakout](https://shop.sb-components.co.uk/products/rfid-breakout?_pos=5&_sid=fac219786&_ss=r) - RFID breakout for standalone testing and freedom to choose microcontroller as per requirement.

## Product License

This is ***open source*** product. Kindly check the LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>     
     

    
    


