<h1 align="center">ESP32-BlueJammer - by @emensta</h1>
<div align="center">
  <img src="https://dwdwpld.pages.dev/ESP32-BlueJammerBy@emensta.jpg" alt="ESP32-BlueJammer">
  <h3 align="center">Jamming is ILLEGAL! Educational purposes only!</h3>
</div>



## ESP32-BlueJammer
The ESP32-BlueJammer (Bluetooth jammer, BLE jammer, WiFi jammer, RC jammer) disrupts various devices using an ESP32 and nRF24 modules, causing plenty of noise and sending unnecessary packets (DoS).              
                                                                    
It interrupts:                                                       
audio in speakers, smartphone connections, WiFi, RC Drones (etc.), IoT devices, and much more communicating on 2.4GHz!

Ideal for controlled disruption and security testing. Based on 2,4GHz communication.

It has a big range (over 30Meters+ - may vary on your antenna and hardware setup!) on newest Bluetooth versions with casual 2.4GHz antennas, you can easily increase this aswell by taking some simple "bigger" router antennas.
An amplifier (2.4GHz) may be an good option too!

Remember that jamming is illegal and should not be used with malicious intent!



## Want to buy one? - [Don Anon Tech's online-shop](https://datechlabs.com)
**DIY-PCB:**  "Blue ESP DIY PCB"  
For this one, all you need is listed below:  

**Required:**  
- ESP32 Dev Module (such as ESP32-WROOM-32U, any ESP32 should work as long as it has the needed pins, 38P is recommended!)  
- nRF24L01+PA+LNA (2x)  

**Additional:**  
- TP4056 Charging Module (Micro-USB/Type-C)  
- JST PH 2.0 Connector  
- 3.7V Li-Ion Battery  
- 3rd Antenna: IPEX to SMA-F pigtail  
![DIY-PCB](https://dwdwpld.pages.dev/ESP32-BlueJammer-DIY-PCB.jpg)
[Shop](https://datechlabs.com/products/blue-esp-diy-pcb-back-order)

---

**PRE-SOLDERED:**  "The Blue ESP"  
This is a finished pre-built ESP32-BlueJammer PCB.

**Required:**  
- nRF24L01+PA+LNA (2x)  
Why do you need to get the nRF24's? -> the pinout can be used to connect either nRF24 or CC1101 modules for further experiments with and ESP32 chip.
![TheBlueESP](https://dwdwpld.pages.dev/TheBlueESP.png)
[Shop](https://datechlabs.com/products/the-blue-esp-pre-order)



## Video tutorials and demonstrations
[Full TikTok DIY tutorial](https://www.tiktok.com/@emensta/video/7389783018002550049)

[DIY Video tutorial (if the TikTok is not available for you)](https://www.mediafire.com/file/mgb3wicdifkq1ce/ESP32-BlueJammerByEmensta-DIYTutorial.mp4/file)

[TikTok Demonstration](https://vm.tiktok.com/ZGec5Mqg7/)

[TikTok Demonstration (if the TikTok is not available for you)](https://www.mediafire.com/file/xgru01ihbw26mfu/ESP32-BlueJammerByEmensta-Demonstration.mp4/file)



## Operation Channels
- **Bluetooth** = 79CH  
  Frequency Range: 2.402 GHz to 2.480 GHz  
  Channel Width: 1 MHz

- **BLE** = 40CH  
  Frequency Range: 2.400 GHz to 2.4835 GHz  
  Channel Width: 2 MHz

- **WiFi** = 14CH  
  Frequency Range: 2.400 GHz to 2.4835 GHz  
  Channel Width: Typically 20 MHz, but can be 22 MHz or 40 MHz in some cases

- **RC drones, etc.** = 1-125CH  
  Frequency Range: 2.400 GHz to 2.525 GHz  
  Channel Width: 1 MHz




## Hardware - Make your own ESP32-BlueJammer

### Required:

- **ESP32 Dev Module** (such as ESP32-WROOM-32U, any ESP32 should work as long as it has the needed pins, 38P is recommended!)
- **nRF24L01+PA+LNA** (2x)
- **10uF Capacitor** (2x) (any voltage above 5V)
- **Prototype PCB** (at least 7x9 cm, but you will need to cut it down to fit the 3D-printed case, which fits a size of 7x5,5cm!)

### Additional:

- 3rd Antenna: **IPEX to SMA-F pigtail**
- Status LED: **3mm LED**
- **4.7k Ohm Resistor**

### If you're looking to add a battery:

- **3.7V Li-Ion Battery**
- **JST PH 2.0 Connector**
- **TP4056 Charging Module (Micro-USB/Type-C)**
- **Mini Slide Switch**

### To screw the 3D printed case together you must have:

- **M3x16 Screws** (2x)
- **M3 Nuts** (2x)



## Antennas
A frequently asked question is whether the antennas are needed and what the third antenna is for, here is the answer:
Yes, you need at least both antennas for the nRF24's! Why? To have it working on a decent range!
The average range with standard known chinese 2.4GHz antennas is about 20meters. Upgrading those antennas will help a lot with getting more range!

2 antennas are for the HSPI and VSPI nRF24 modules!

The 3rd antenna is plugged to the ESP32 chip itself, wither via IPEX or soldered onto it's own antenna, if your ESP32 does not provide any option to add that one, it obviously won't be possible!
What is the 3rd antenna used for? The third antenna connected to the ESP32 chip itself helps with reliable long-range interference. It ensures a better intermediate signal and stability when jamming!
(The third antenna is your own decision and therefore optional!)



## Flashing ESP32 via webflasher
![ESP32-BlueJammerFlasher](https://dwdwpld.pages.dev/ESP32BlueJammerFlasher.png)                                                                 
I've created a webflasher to make it super easy for you to flash your ESP32 chip with the ESP32-BlueJammer firmware of your choice!
- Visit [ESP32-BlueJammerFlasher](https://esp32-bluejammerflasher.pages.dev)
- Connect your ESP32 via a data USB cable
- Choose your firmware, chip and connect
- Flash the firmware of your choice :D

If your ESP32 is not showing up in the device list or won't get recognized you will need to have [THESE DRIVERS INSTALLED](https://www.silabs.com/documents/public/software/CP210x_Windows_Drivers.zip) which can be found on my [Discord server](https://discord.gg/yNGhKxzqUE) too!



## ESP32-nRF24L01+ pinout + battery mod
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
| IRQ           |                  |

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
| IRQ           |                  |

### Status LED
| ESP32 | 4.7k Ohm Resistor | 3mm Status LED (blue)|
|-------|-------------------|----------------------|
|  GND  |                   |       (-) LED        |
|       |      Resistor     |       (+) LED        |
|GPIO27 |      Resistor     |                      |

### Battery modification (additional)
| 3.7V Li-Ion battery | JST-PH2 connector    | TP4056 Charging Module | Mini Slide Switch | ESP32 |
|---------------------|----------------------|------------------------|-------------------|-------|
| (+) Battery         | (+) JST-PH2          | Bat +                  |                   |       |
| (-) Battery         | (-) JST-PH2          | Bat -                  |                   |       |
|                     |                      | OUT +                  | Switch in         |       |
|                     |                      | OUT -                  |                   |  GND  |
|                     |                      |                        | Switch out        |  3V3  |


### Schematics
![VisualESP32-BlueJammerSchematics](https://dwdwpld.pages.dev/ESP32-BlueJammerSchematics.png)


## 3D printed case
#### The 3D printed case fits ONLY a PCB size of 7cm x 5.5cm and you'll need to drill out 2 holes according for the M3 screws to fit through the PCB!
<h3 align="center">Access to the ESP32 micro-USB port, aswell as to both EN & Boot buttons</h3>

![ESP32MicroUSB](https://dwdwpld.pages.dev/ESP32-BlueJammerMicroUsb.jpg)

<h3 align="center">TP4056 charging port access with charging state indicator holes (red=charging - blue=fully charged)</h3>

![USB_C_chargerWithIndicators](https://dwdwpld.pages.dev/ESP32-BlueJammerUSB_C_chargerWithIndicators.jpg)

<h3 align="center">On/off switch with blue indicator LED</h3>

![OnOffSwitch](https://dwdwpld.pages.dev/ESP32-BlueJammerOnOffSwitch.jpg)



## V3-Case 3D model view [[download .stl](https://dwdwpld.pages.dev/V3-ESP32-BlueJammerBy@emensta3DCase.stl)]

<h3 align="center">Here's a look at the V3 2 antenna version itself</h3>

![3DCaseView](https://dwdwpld.pages.dev/V3-ESP32-BlueJammer3DCaseView.png)



## V4-Case 3D model view [[download .stl](https://dwdwpld.pages.dev/V4-ESP32-BlueJammerBy@emensta3DCase.stl)]

<h3 align="center">Here's a look at the V4 3 antenna version itself</h3>

![3DCaseView](https://dwdwpld.pages.dev/V4-ESP32-BlueJammer3DCaseView.png)



## PCB

<h3 align="center">That's how the components are placed (PCB size=7cm x 5.5cm - Larger sizes will NOT fit in the case!)</h3>

![DIYPCB](https://dwdwpld.pages.dev/DIYPCB.jpg)



## About the ESP32-BlueJammer and my source code
- **Is my ESP32-BlueJammer really working?**  
  Yes! My ESP32 BlueJammer is fully functional, and no one pauses the sound in the demo video. Many people have built their own ESP32-BlueJammer and confirmed that it works! Join my Discord and see for yourself! ;D

- **Why my ESP32-BlueJammer code is NOT open source**  
  There are several "BLE Jammers" available on GitHub, but they all have limitations in frequency range, channel coverage, and effective distance (around 5 meters). Therefore I decided to develop and code my own firmware for the ESP32-BlueJammer, aiming for superior performance.

  Despite some claims that I might have copied someone else's work, it's important to clarify that extracting source code from a compiled file (.hex, .bin, etc.) is practically impossible. If I had used someone else's work, I wouldn't have been able to create custom console banners, develop multiple firmware versions, or build a web flasher. My code is entirely written from scratch. There is nothing taken from other available codes, sources, codebases or resources as a foundation, if any even exist. My code remains closed source for now, to protect the significant effort and innovation I've invested in this project.

  This isn't my last project. I'm looking forward to implementing the ESP32-BlueJammer in further ongoing projects, so for now, I'd like the code to remain closed source. Maybe someday I'll make it open source!  
  -no one knows. ;D
## Source code snippets by @emensta
- **Here are three snippets of my source code for you to compare with other available sources. This way, you can see that it was written from scratch:** 
![ESP32-BlueJammerByEmenstaCodeSnippets](https://dwdwpld.pages.dev/ESP32-BlueJammerByEmenstaCodeSnippets.jpg)



## Discord
You can join my Discord server [here](https://discord.gg/emensta)!



## Portfolio and all my links
Here you can visit my Portfolio, you'll find everything that you're looking for [here](https://emensta.pages.dev)!



## Donate
If you enjoy what I do and want to support me in creating more content and sharing new ideas, feel free to support me!                                         
[PayPal.me](https://www.paypal.me/emensta)

<h1 align="center"> DISCLAIMER </h1>

<h4 align="center">Please note that the use of this tool is entirely at your own risk. It is intended strictly for educational purposes and should not be used for any illegal or unethical activities. Jamming is illegal and can get you in big trouble!</h4>
<h4 align="center">I'm not responsible for your actions! </h4>
