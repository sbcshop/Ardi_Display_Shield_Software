# Ardi_Display_Shield_Software
<img src="https://cdn.shopify.com/s/files/1/1217/2104/files/ArdiPiDisplayShield.jpg?v=1683880851">
Ardi Display Shield features a vibrant 2" IPS screen with a resolution of 240 x 320 pixels, this shield seamlessly integrates with your Arduino Uno and compatible boards, Ardi32 and ArdiPi. Two programmable buttons and 5-Way Joystick onboard gives ability to add additional control features to your project.

This github provides getting started guide and other working details for Ardi Display Shield 

### Features:
- Onboard 2.0” TFT Display
- Compatible with 3.3V/5V MCU, Selection provided
- Onboard 5-Way Joystick allows better control-related projects
- Two programmable Buttons to add additional functionality to project
- Mounts directly onto your ArdiPi, Ardi32, and Arduino compatible boards

### Specifications:
- Display resolution 240x320 pixels
- Pixel Pitch: 0.1275(H) x 0.1275(V) mm
- Active Area: 30.6(H) x 40.8(V) mm
- Module Size: 34.6(H) x 47.8(V) x2.05(D) mm
- SPI Interface
- Display Colors: 65K colors
- Drive IC: ST7789V2
  
### Hardware Overview
#### Pinout
<img src="https://cdn.shopify.com/s/files/1/1217/2104/files/ardi2.0displayshieldpinout.jpg?v=1688469169">

- (1) & (4) Programmable Buttons
- (2) Voltage Selection 3.3V/5V
- (3) TFT 2.0 Display
- (5) 5-Way Joystick

**Note:** Don't forget to set jumper selection on correct selection when using with 5V or 3.3V board. Put jumpber on **3V3-SEL** when using with **3.3V MCU boards** and on **SEL-5V** when using with **5V MCU Boards**.

#### Interfacing Details

When Relay shield mounted on ArdiPi, selection **jumper** must be on **3V3-SEL** side
|ArdiPi | Display shield | Function |
|---|---|---|
| GP18 | CLK | Clock pin of SPI interface for Display |
| GP16 | BL | BackLight for display |
| GP19 | DIN | MOSI (Master OUT Slave IN) pin of SPI interface for display |  
| GP17 | CS | SPI Chip select pin for display |
| GP14 | RST | Display Reset pin | 
| GP15 | DC | Data/Command pin of SPI interface for display
| GP3 | BT1 | Programmable Button 1 |
| GP11 | BT2 | Programmable Button 2 |
| GP4 | J_U | Joystick Up switch |
| GP0 | J_R | Joystick Right switch |
| GP5 | J_L | Joystick Left switch |
| GP2 | J_D | Joystick Down switch |
| GP1 | J_SEL | Joystick Centre switch |

When Relay shield mounted on Ardi-32, selection **jumper** must be on **3V3-SEL** side
|Ardi-32 | Display shield | 
|---|---|
| IO12 | CLK | 
| IO13 | BL | 
| IO11 | DIN |  
| IO10 | CS |
| IO21 | RST |
| IO47 | DC |
| IO9 | BT1 |
| IO2 | BT2 | 
| IO41 | J_U | 
| IO42 | J_R |
| IO1 | J_L |
| IO17 | J_D | 
| IO18 | J_SEL | 

When Relay shield mounted on Arduino Uno, selection **jumper** must be on **SEL-5V** side 
|Arduino UNO | Display shield | 
|---|---|
| D13 | CLK | 
| D12 | BL | 
| D11 | DIN |  
| D10 | CS |
| D9 | RST |
| D8 | DC |
| D6 | BT2 |
| D5 | BT1 | 
| D4 | J_U | 
| D3 | J_R |
| D2 | J_L |
| D1 | J_D | 
| D0 | J_SEL | 


### Example Codes
   Also, sample codes are available for Ardi Display shield
   - [Ardi Display shield for UNO]() 
   - [Ardi Display shield for Ardi32]() 
   - [Ardi Display shield for ArdiPi]()
   
   Using this sample code as a guide, you can modify, build for other boards and share codes!!  
   
## Resources
  * [Schematic](https://github.com/sbcshop/Ardi_Display_Shield_Hardware/blob/main/Design%20Data/SCH%202.0%20INCH%20LCD%20Shield.pdf)
  * [Hardware Files](https://github.com/sbcshop/Ardi_Display_Shield_Hardware/tree/main)
  * [Step File](https://github.com/sbcshop/Ardi_Display_Shield_Hardware/blob/main/Mechanical%20Data/STEP%202.0%20INCH%20LCD%20Shield.step)


## Related Products
   * [Ardi-32](https://shop.sb-components.co.uk/products/ardi32-uno-r3-alternative-board-based-on-esp32-s3-wroom?_pos=6&_sid=90d9cefb0&_ss=r) - Arduino Uno Form factor with latest powerful ESP32 S3
   * [ArdiPi](https://shop.sb-components.co.uk/products/ardipi-uno-r3-alternative-board-based-on-pico-w?_pos=5&_sid=5704675c2&_ss=r) - Arduino Uno Form factor with powerful Pico W of Raspberry Pi having onboard WiFi and BLE support.
   * [Ardi UHF Shield](https://shop.sb-components.co.uk/products/ardi-uhf-shield-for-arduino-uno?variant=40791294836819) - UHF based shield with Oled display and Buzzer onboard
   * [Ardi RFID Shield](https://shop.sb-components.co.uk/products/ardi-rfid-shield-for-arduino-uno?_pos=5&_sid=b4e4b2ef1&_ss=r) - Ardi RFID Shield with onbard Relay and Status LED
   
   Shields are compatible with ArdiPi, Ardi-32 and Other Arduino Uno Compatible boards.

## Product License

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>
