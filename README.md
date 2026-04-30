# Squawk-2.0
A radio station with a storage unit for walkie-talkies, w/ OLED screen & 3.5mm headphone jack connector
SI4844 powered with Arduino Nano, PAM8403 amplifier with the [pu2clr](https://pu2clr.github.io/SI4844/) library.

<img width="1920" height="960" alt="Radio-2026-04-28 000101" src="https://github.com/user-attachments/assets/28ec7cb4-83d6-4336-adbb-bf1c5156e014" />
<img width="1920" height="960" alt="Radio-2026-04-28 000112" src="https://github.com/user-attachments/assets/76a83ad6-565a-442c-94d9-bc3e877fe70a" />


## About this project
The name "Squawk 2.0" originates from the popular TV show - Stranger Things (Season 5), where they had a master radio station for duplex transmission. Though this station cannot transmit any radio signals for walkie-talkies to pick up (due to legal reasons), it listens to the Citizens Band (CB) with 20 channels and a range of 2-3km. This is designed as a retro tabletop AM/FM/SW radio with the SI4844 chip, and also a handy storage device for the user. Planning to create walkie-talkies in the future that can connect to this station.
### Why did I make this?
Well, I needed a storage compartment for my walkie talkies and also wanted the container to be a bit more exciting than just a regular tin box. 

### How do you use it?
It's pretty simple, here is a layout of all the functions of the buttons you can press:
<img width="1026" height="701" alt="image" src="https://github.com/user-attachments/assets/87387009-2e34-44ea-a3be-593252fc840a" />


## Key features
- SW/MW/AM/FM radio broadcast with SI4844 IC
- Adjustable channel and volume with OLED screen indicator
- Storage compartment in 3D model
- Hinged door to access the compartment
- Arduino powered - open source code and customisable to your own liking
- USB-B connectivity
- 3.5mm headphone jack to listen to the radio independently without interrupting neighbours, like a Walkman
- Optimised 4-layer PCB (front, gnd_front, gnd_back, back) routing for good antenna connectivity

## [Schematic](https://github.com/LinuxDinoGitHub/Squawk-2.0/tree/main/pcb)
<img width="2200" height="1700" alt="Print Schematic" src="https://github.com/user-attachments/assets/da10d078-448f-4f75-9898-b1b98b1ad7ad" />

## [PCB](https://github.com/LinuxDinoGitHub/Squawk-2.0/tree/main/pcb)
A simple, 4-layer PCB. 96mm x 81mm PCB with 3 mounting holes for M3 screws.
### First layer (Front)
<img width="981" height="805" alt="image" src="https://github.com/user-attachments/assets/ea308864-e14e-4614-810a-26f8a153248b" />

### Second layer (GND net)
<img width="982" height="804" alt="image" src="https://github.com/user-attachments/assets/bfb52348-23fe-4223-b285-4982e836aaba" />

### Third layer (GND net)
<img width="978" height="803" alt="image" src="https://github.com/user-attachments/assets/9d2371e3-187c-4ab8-b1e4-7a98db023490" />

### Fourth layer (Back)
<img width="980" height="806" alt="image" src="https://github.com/user-attachments/assets/3af506f0-be6a-4175-9323-983d1c90b498" />

### 3D view
Front
<img width="974" height="806" alt="image" src="https://github.com/user-attachments/assets/56d4a5a0-76be-4536-91bf-99c6caf6efca" />
Back
<img width="932" height="783" alt="image" src="https://github.com/user-attachments/assets/e754293f-e941-4326-bddb-cf63ace13a80" />

## [Firmware](https://github.com/LinuxDinoGitHub/Squawk-2.0/blob/main/firmware/firmware.ino)
After assembling your PCB, use the firmware.ino file in the repository to flash your Arduino Nano. You can customise messages and timings by editing the code with the Arduino IDE.

## [BOM](https://github.com/LinuxDinoGitHub/Squawk-2.0/tree/main/BOM)
The BOM **without** specific values is linked here ([GitHub directory](https://github.com/LinuxDinoGitHub/Squawk-2.0/blob/main/BOM_kicad_generated.csv) or [Google Sheets](https://docs.google.com/spreadsheets/d/1nt2ZC4SuuWCHXpdcqgjWmxoxNzFQoS0aQbvXVXabcSM/edit?gid=0#gid=0). The total cost for the project should not exceed 13USD (after averaging costs out by dividing by the bulk bought quantity).

The BOM **with** specific values is here (Github [directory](https://github.com/LinuxDinoGitHub/Squawk-2.0/blob/main/BOM_with_links.csv) or [Google Sheets](https://docs.google.com/spreadsheets/d/1nt2ZC4SuuWCHXpdcqgjWmxoxNzFQoS0aQbvXVXabcSM/edit?gid=1614936167#gid=1614936167))

### 3D printed case
Use a slicer to print the following [file](https://github.com/LinuxDinoGitHub/Squawk-2.0/blob/main/models/Radio.step). The 3D printed case is not accounted for in the BOM due to the variation between suppliers. The expected filament cost is around 10$ USD.

## Zine page
<img width="676" height="1034" alt="image" src="https://github.com/user-attachments/assets/1f0ec35b-3b42-4107-860f-376ad4edf63c" />


## Credits
Huge thanks to Ricardo for his amazing library and intuitive example code for the SI4844, which genuinely saved me so much time. [Link](https://pu2clr.github.io/SI4844/) to his repo and library. Thanks to the amazing community from Hack Club fallout for helping out my design as well, I couldn't have done it without them.
