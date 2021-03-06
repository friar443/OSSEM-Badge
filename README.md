# OSSEM-Badge
An attempt at making a badge. Here is the repository where members of OSSEM can
get the OSSEM badge firmware and share their own spin on their firmware. The
hardware required for the badge development is:
- [STM32F103C8T6](https://www.amazon.com/gp/product/B01DLIJOAO/ref=oh_aui_search_detailpage?ie=UTF8&psc=1)
- [ST-Link
  v2](https://www.amazon.com/Qunqi-ST-LINK-STLINK-debugger-programmer/dp/B016ZPNEYC/ref=sr\_1\_1?s=industrial&ie=UTF8&qid=1484330473&sr=1-1&keywords=st-link+v2)
- Since the agreed upon first objective for this project is to understand how to
  write and interface with the LCD, you will need [SSD1306
  OLED](https://www.amazon.com/Diymall-Serial-128x64-Display-Arduino/dp/B00O2LKEW2/ref=sr_1_1?s=industrial&ie=UTF8&qid=1484331448&sr=1-1&keywords=ssd1306+oled)
- A various collection of
  [resistors](https://www.amazon.com/E-Projects-EPC-103-Value-Resistor-Kit/dp/B00E9YQQSS/ref=sr_1_3?s=industrial&ie=UTF8&qid=1484331498&sr=1-3&keywords=resistors)
- [Breadboard](https://www.amazon.com/eBoot-Experiment-Solderless-Breadboard-400-Points/dp/B01MG5IPUX/ref=sr_1_1?s=industrial&ie=UTF8&qid=1484331573&sr=1-1-spons&keywords=breadboard&psc=1)
. The bigger the better.
All of the above are links to Amazon. Some other good sources for these parts
are Digikey, Mouser and Ebay. These are only some of the places to acquire the
necessary parts.
- Some jumper cables. No, not those jumper cables.
  [These](https://www.amazon.com/Breadboard-Jumper-Wire-75pcs-pack/dp/B0040DEI9M)
  jumper cables. It helps to get an assorted mix of male-male, female-male and
  female-male. 

# Setup
An effort has/will be made to ensure that users/developers are able to
learn on different operating systems. Currently the following operating systems
have a setup guide:
## Different OS Guides
### Windows
- [Windows 7/10](docs/windows-badge-setup-how-to.md)

### Linux
- [Ubuntu 16.04](docs/ubuntu-badge-setup-how-to.md)

## Eclipse
A work in progress guide for setting up [Eclipse](docs/eclipse_setup.md). If you
find issues with the guide or if something is not clear contact either @gaterbyte
or @steve-offutt.

## ST-Link Hook-Up
To hook up the ST-Link V2 to the STM32F103C9T6 board we have to have some female
to female jumpers. If you don't already have some available bum some from
@steve-offutt :-P

The way we hook up the ST-Link is as follows:

| ST-Link V2   |  STM32F103C8T6  |
| :----------: | :-------------: |
| VCC/VDD      | 3.3V Header Pin |
| GND          | GND             |
| CLK          | DCLK            |
| SWD          | DIO             |

**WARNING:** If you are unsure about your wiring, **ASK SOMEONE!!** You can
fry potentially fry your board. It is worth asking before plugging into random
ports! You have been warned. 

# Lessons
[Lesson 1](docs/lesson1.md)
