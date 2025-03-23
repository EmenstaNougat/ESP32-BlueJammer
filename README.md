<h1 align="center">ESP32-BlueJammer - by @emensta</h1>
<div align="center">
  <img src="https://dwdwpld.pages.dev/ESP32-BlueJammerBy@emensta.jpg" alt="ESP32-BlueJammer">
  <h3 align="center">Jamming is ILLEGAL! Educational purposes only!</h3>
</div>

<div align="center">
<a href="https://github.com/EmenstaNougat/ESP32-BlueJammer" title="Go to GitHub repo">
  <img src="https://img.shields.io/static/v1?label=EmenstaNougat&message=ESP32-BlueJammer&color=purple&logo=github" alt="EmenstaNougat - ESP32-BlueJammer">
</a>
<a href="https://github.com/EmenstaNougat/ESP32-BlueJammer">
  <img src="https://img.shields.io/github/stars/EmenstaNougat/ESP32-BlueJammer?style=social" alt="stars - ESP32-BlueJammer">
</a>
<a href="https://github.com/EmenstaNougat/ESP32-BlueJammer">
  <img src="https://img.shields.io/github/forks/EmenstaNougat/ESP32-BlueJammer?style=social" alt="forks - ESP32-BlueJammer">
</a>
</div>


<h4 align="center">
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer#hardware---make-your-own-esp32-bluejammer">Make your own</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer#esp32-nrf24l01-pinout--battery-mod">Schematics</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer?tab=readme-ov-file#pcb">Hardware layout</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer?tab=readme-ov-file#pcbs-with-esp32-and-rf-module-capability---don-anon-techs-online-shop">PCB's</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer#video-tutorials-and-demonstrations">Demos</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer#operation-channels">Channels</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer?tab=readme-ov-file#flashing-the-firmware">Flashing</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer#3d-printed-case">3D case</a>
    <span> | </span>
  <a href="https://github.com/EmenstaNougat/ESP32-BlueJammer?tab=readme-ov-file#about-the-esp32-bluejammer-and-my-source-code">About</a>
    <span> | </span>
  <a href="https://emensta.pages.dev">Website</a>
</h4>

## ESP32-BlueJammer
The ESP32-BlueJammer (Bluetooth jammer, BLE jammer, WiFi jammer, RC jammer) disrupts various devices using an ESP32 and nRF24 modules, causing plenty of noise and sending unnecessary packets (DoS).              
                                                                    
It interrupts:  
**The whole 2.4GHz broadband!** Everything that works on 2.4GHz is being interfered, like:                                                       
audio in speakers being transmitted over bluetooth, microphones on 2.4GHz, smartphone connections, WiFi, RC Drones (etc.), IoT devices, smart gadgets, wireless keyboard & mouse, just anything on 2.4GHz!

Ideal for controlled disruption and security testing. Based on 2,4GHz communication.

It has a big range (over 30Meters+ - may vary on your antenna and hardware setup!) on newest Bluetooth versions with casual 2.4GHz antennas, you can easily increase this aswell by taking some simple "bigger" router antennas.
An amplifier (2.4GHz) may be an good option too!

Remember that jamming is illegal and should not be used with malicious intent!



## PCB's with ESP32 and RF-module capability - [Don Anon Tech's online-shop](https://datechlabs.com)
**DIY-PCB:**  "Blue ESP DIY PCB"  
This PCB can fit an ESP32 DevKit and 2 RF-modules such as nRF24 or CC1101 etc., you can use it in combinations (1x nRF, 1x CC1101) to create several things.  
***Remember: It is not intended for illegal use, neither for my project!***  
For this one, all you need is listed below:  

**Required:**  
- **[ESP32 Dev Module](https://s.click.aliexpress.com/e/_onYIVKr)** (**Recommended: ESP32-32U CP2102**, any ESP32 should work as long as it has the needed pins, 38P required!)  
- **[nRF24L01+PA+LNA](https://s.click.aliexpress.com/e/_oma5UQx)** (2x)  

**Additional:**  
- **[TP4056 Charging Module (Micro-USB/Type-C)](https://s.click.aliexpress.com/e/_oCqORHE)**  
- **[JST PH 2.0 Connector](https://s.click.aliexpress.com/e/_ooSOhDd)**  
- **[3.7V Li-Ion Battery](https://s.click.aliexpress.com/e/_on04mQ7)**  
- **[3rd Antenna: **IPEX to SMA-F pigtail](https://s.click.aliexpress.com/e/_oFDpn1V)**  
![DIY-PCB](https://dwdwpld.pages.dev/ESP32-BlueJammer-DIY-PCB.jpg)
[Shop](https://datechlabs.com/products/blue-esp-diy-pcb-back-order)

---

**PRE-SOLDERED:**  "The Blue ESP"  
This is an ESP32 with RF-module breakouts (nRF24/CC1101 etc.) for experimenting.   ***Remember: It is not intended for illegal use, neither for my project!***  

**Required:**  
- **[nRF24L01+PA+LNA](https://s.click.aliexpress.com/e/_oma5UQx)** (2x)  
Why do you need to get the nRF24's? -> the pinout can be used to connect either nRF24 or CC1101 modules for further experiments with an ESP32 chip.
![TheBlueESP](https://dwdwpld.pages.dev/theblueespwavychat.png)
[Shop](https://datechlabs.com/products/the-blue-esp-pre-order)



## Video tutorials and demonstrations
[Full DIY assembling video tutorial](https://www.tiktok.com/@emensta/video/7389783018002550049)

[Full DIY assembling video tutorial (if the TikTok is not available for you)](https://www.mediafire.com/file/mgb3wicdifkq1ce/ESP32-BlueJammerByEmensta-DIYTutorial.mp4/file)

---

[Demonstration](https://vm.tiktok.com/ZGec5Mqg7/)

[Demonstration (if the TikTok is not available for you)](https://www.mediafire.com/file/xgru01ihbw26mfu/ESP32-BlueJammerByEmensta-Demonstration.mp4/file)

---

[Flashing process](https://www.tiktok.com/@emensta/video/7413509704401292577)

[Flashing process (if the TikTok is not available for you)](https://www.mediafire.com/file/2aj4hmf9zt7w6sw/ESP32-BlueJammerByEmensta-FlashingProcess.mp4/file)

---

ESP32-BlueJammer tutorial by @ElMackflay  
[![ESP32-BlueJammer tutorial by @ElMackflay](https://img.youtube.com/vi/1kjkWU25_qo/0.jpg)](https://www.youtube.com/watch?v=1kjkWU25_qo)  
---


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
(Aliexpress affilate links to support me-linked to the item names)
### Required:

- **[ESP32 Dev Module](https://s.click.aliexpress.com/e/_onYIVKr)** (**Recommended: ESP32-32U CP2102**, any ESP32 should work as long as it has the needed pins)
- **[nRF24L01+PA+LNA](https://s.click.aliexpress.com/e/_oma5UQx)** (2x)
- **[10uF Capacitor](https://s.click.aliexpress.com/e/_oFvFeYX)** (2x) (any voltage above 5V)
- **[Prototype PCB](https://s.click.aliexpress.com/e/_oBtd18j)** (at least 7x9 cm, but you will need to cut it down to fit the 3D-printed case, which fits a size of 7x5,5cm!)

### Additional:

- **[0.96" OLED Display I2C](https://s.click.aliexpress.com/e/_oCdkjPX)**
- [3rd Antenna: **IPEX to SMA-F pigtail**](https://s.click.aliexpress.com/e/_oFDpn1V)
- [Status LED: **3mm LED**](https://s.click.aliexpress.com/e/_ooxufHV)
- **[4.7k Ohm Resistor](https://s.click.aliexpress.com/e/_oBV1Q1Z)**

### If you're looking to add a battery:

- **[3.7V Li-Ion Battery](https://s.click.aliexpress.com/e/_on04mQ7)**
- **[JST PH 2.0 Connector](https://s.click.aliexpress.com/e/_ooSOhDd)**
- **[TP4056 Charging Module (Micro-USB/Type-C)](https://s.click.aliexpress.com/e/_oCqORHE)**
- **[Mini Slide Switch](https://s.click.aliexpress.com/e/_ooC8DXh)**

### To screw the 3D printed case together you must have:

- **M3x16 Screws** (2x)  
- **M3 Nuts** (2x)  
Get this M3 kit instead:
- **[M3 screws&nuts kit](https://s.click.aliexpress.com/e/_oC24YXH)**



## Antennas
A frequently asked question is whether the antennas are needed and what the third antenna is for, here is the answer:
Yes, you need at least both antennas for the nRF24's! Why? To have it working on a decent range!
The average range with standard known chinese 2.4GHz antennas is about 20meters. Upgrading those antennas will help a lot with getting more range!

2 antennas are for the HSPI and VSPI nRF24 modules!

The 3rd antenna is plugged to the ESP32 chip itself, wither via IPEX or soldered onto it's own antenna, if your ESP32 does not provide any option to add that one, it obviously won't be possible!
What is the 3rd antenna used for? The third antenna connected to the ESP32 chip itself helps with reliable long-range interference. It ensures a better intermediate signal and stability when jamming!
(The third antenna is your own decision and therefore optional!)



## Flashing the firmware
### via webflasher (Easy)  
![ESP32-BlueJammerFlasher](https://dwdwpld.pages.dev/ESP32BlueJammerFlasher.png)                                                                 
I've created a webflasher to make it super easy for you to flash your ESP32 chip with the ESP32-BlueJammer firmware of your choice!  
- Visit [ESP32-BlueJammerFlasher](https://esp32-bluejammerflasher.pages.dev)
- First, choose the firmware type, "Generic" or "0.96" OLED"
- choose the firmware you want to flash
- Connect your ESP32 via a data USB cable
- Flash the firmware of your choice :D

### via BlueFlasher.exe -Windows application (Easy)  
<img src="https://dwdwpld.pages.dev/BlueFlasherMain.jpg" width="650" height="auto">

The BlueFlasher.exe lets you flash any available firmware with no more than 3 clicks! It is always the latest up-to-date firmware!  
- Download the [BlueFlasher.exe](https://github.com/EmenstaNougat/ESP32-BlueJammer/raw/refs/heads/main/BlueFlasher/BlueFlasher.exe)
- run the application [(Image)](https://dwdwpld.pages.dev/BlueFlasherMain.jpg)
- simply choose the COM port of your ESP32 [(Image)](https://dwdwpld.pages.dev/BlueFlasherCOM.jpg)
- hold the "Boot" button on your ESP32 from now on
- choose the firmware you want to flash
- release the "Boot" button on your ESP32
- wait for the firmware to be flashed (check console) :D

https://github.com/user-attachments/assets/9c6b7322-9d39-48a1-9ef4-535c6ff64681

**Developed by [9dl](https://github.com/9dl)**

### Flashing ESP32 via binary files (Advanced)  
- Download the **.bin files** available on this repository
- Use any flasher of your choice
- Flash it :D

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

### OLED Display I2C (additional - make sure to use the correct firmware!)
| 0.96" OLED Display I2C | ESP32 |
|------------------------|-------|
|          GND           |  GND  |
|          VCC           | 3.3V  |
|          SCL           |GPIO 5 |
|          SDA           |GPIO 4 |

### Battery modification (additional)
| 3.7V Li-Ion battery | JST-PH2 connector    | TP4056 Charging Module | Mini Slide Switch | ESP32 |
|---------------------|----------------------|------------------------|-------------------|-------|
| (+) Battery         | (+) JST-PH2          | Bat +                  |                   |       |
| (-) Battery         | (-) JST-PH2          | Bat -                  |                   |       |
|                     |                      | OUT +                  | Switch in         |       |
|                     |                      | OUT -                  |                   |  GND  |
|                     |                      |                        | Switch out        |  3V3  |



### Schematics
![VisualESP32-BlueJammerSchematics](https://dwdwpld.pages.dev/tempunavailable.jpg)



## PCB

<h3 align="center">That's how the components are placed (PCB size=7cm x 5.5cm - Larger sizes will NOT fit in the case!)</h3>

![DIYPCB](https://dwdwpld.pages.dev/DIYPCB.jpg)



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



<h1 align="center"> DISCLAIMER </h1>

<h4 align="center">Please note that the use of this tool is entirely at your own risk. It is intended strictly for educational purposes and should not be used for any illegal or unethical activities. Jamming is illegal and can get you in big trouble!</h4>
<h4 align="center">I'm not responsible for your actions! </h4>
