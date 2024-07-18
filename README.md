<h1 align="center">ESP32-BlueJammer - by @emensta</h1>
<div align="center">
  <img src="https://dwdwpld.pages.dev/ESP32-BlueJammerBy@emensta.jpg" alt="ESP32-BlueJammer">
</div>



## ESP32-BlueJammer
The ESP32-BlueJammer disrupts various devices using an ESP32 NodeMCU and nRF modules, causing plenty of noise and sending unnecessary packets (DoS).              
                                                                    
It interrupts:                                                       
audio in speakers, smartphone connections, WiFi, RC Drones (etc.), IoT devices, and much more communicating on 2.4GHz!

Ideal for controlled disruption and security testing. Based on 2,4GHz communication.

It has a big range (over 30Meters - may vary on your antenna and hardware setup!) on newest Bluetooth versions with casual 2.4GHz antennas, you can easily increase this aswell by taking some simple "bigger" router antennas.
An amplifier (2.4GHz) may be an good option too!




## TikTok video with a complete tutorial
[Full TikTok DIY tutorial](https://www.tiktok.com/@emensta/video/7389783018002550049)



## operation channels
- Bluetooth = 80CH
- BLE = 40CH
- WiFi = 14CH
- RC drones, etc. = 1-125CH



## hardware
- ESP32 Dev Module (such as ESP32-WROOM-32U)
- nRF24L01+PA+LNA (2x)
- 10UF capacitor (2x) any voltage above 5V

If you're looking to add a battery:
- 3.7V Li-Ion battery
- JST PH 2,0 connector
- TP4056 Charging Module
- 3mm LED (blue)
- 470k Ohm resistor
- mini slide switch

To screw the 3D printed case together you must have:
- M3X16 screws (2x)
- M3 Nuts (2x)
### THE 3D printed case fits ONLY a PCB size of 7cm x 5.5cm and you'll need to drill out 2 holes according for the M3 screws to fit through the PCB!


## flashing ESP32 via webflasher
![ESP32-BlueJammerFlasher](https://dwdwpld.pages.dev/ESP32BlueJammerFlasher.png)                                                                 
I've created a webflasher to make it super easy for you to flash your ESP32 chip with the ESP32-BlueJammer firmware of your choice!
- Visit [ESP32-BlueJammerFlasher](https://esp32-bluejammerflasher.pages.dev)
- Connect your ESP32 via a data USB cable
- Choose your firmware, chip and connect
- Flash the firmware of your choice :D



## ESP32-nRF24L01+ pinout
Here are both pinouts for HSPI and VSPI. You need both nRF24L01 modules connected in order to achieve full capability of the device.                
[nRF24L01+ pinout](https://dwdwpld.pages.dev/nRF24L01pinout.png)
### HSPI
| 1st nRF24L01 module Pin | HSPI Pin (ESP32) | 10uf capacitor |
|---------------|------------------|--------------------|
| VCC           | 3.3V             | (+) capacitor |
| GND           | GND              | (-) capacitor |
| CE            | GPIO 16          |
| CSN           | GPIO 15          |
| SCK           | GPIO 14          |
| MOSI          | GPIO 13          |
| MISO          | GPIO 12          |
| IRQ           |     |

### VSPI 
| 2nd nRF24L01 module Pin | VSPI Pin (ESP32) | 10uf capacitor |
|---------------|------------------|--------------------|
| VCC           | 3.3V             | (+) capacitor |
| GND           | GND              | (-) capacitor |
| CE            | GPIO 22          |
| CSN           | GPIO 21          |
| SCK           | GPIO 18          |
| MOSI          | GPIO 23          |
| MISO          | GPIO 19          |
| IRQ           |     |

### Battery mod
| 3.7V Li-Ion battery | JST PH 2.0 connector | TP4056 Charging Module | Mini Slide Switch | ESP32 | 3mm LED (blue) | 470k Ohm Resistor |
|---------------------|----------------------|------------------------|-------------------|-------|----------------|--------------------|
| (+) battery         | (+) JST              | B+                     |                   |       |                |                    |
| (-) battery         | (-) JST              | B-                     |                   |       |                |                    |
|                     |                      | OUT +                  | switch (+) input  |       |                |                    |
|                     |                      | OUT -                  |                   | GND   |                | resistor output    |
|                     |                      |                        | switch (+) output | 3V3   | (+) LED        |                    |
|                     |                      |                        |                   |       | (-) LED        | resistor input     |


## 3D printed case

<h3 align="center">Access to the ESP32 micro-USB port, aswell as to both EN & Boot buttons</h3>

![ESP32MicroUSB](https://dwdwpld.pages.dev/ESP32-BlueJammerMicroUsb.jpg)

<h3 align="center">TP4056 charging port access with charging state indicator holes (red=charging - blue=fully charged)</h3>

![USB_C_chargerWithIndicators](https://dwdwpld.pages.dev/ESP32-BlueJammerUSB_C_chargerWithIndicators.jpg)

<h3 align="center">On/off switch with blue indicator LED</h3>

![OnOffSwitch](https://dwdwpld.pages.dev/ESP32-BlueJammerOnOffSwitch.jpg)



## 3D model view [[download .stl](https://dwdwpld.pages.dev/ESP32-BlueJammerBy@emensta3DCase.stl)]

<h3 align="center">Here's a look at the model itself</h3>

![3DCaseView](https://dwdwpld.pages.dev/ESP32-BlueJammer3DCaseView.png)



## PCB

<h3 align="center">That's how the components are placed (PCB size=7cm x 5.5cm - Larger sizes will NOT fit in the case!)</h3>

![DIYPCB](https://dwdwpld.pages.dev/DIYPCB.jpg)



## Discord
You can join my Discord server [here](https://discord.gg/yNGhKxzqUE)!



## Donate
If you enjoy what I do and want to support me in creating more content and sharing new ideas, feel free to support me!                                         
[PayPal.me](https://www.paypal.me/emensta)

<h1 align="center"> DISCLAIMER </h1>

<h4 align="center">Please note that the use of this tool is entirely at your own risk. It is intended strictly for educational purposes and should not be used for any illegal or unethical activities. Jamming is illegal and can get you in big trouble!</h4>
<h4 align="center">I'm not responsible for your actions! </h4>
