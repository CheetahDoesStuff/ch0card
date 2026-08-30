# ch0card
**An NFC business card! Very cool!**

## What is this?
This is a business card, by me, for me. But its not just a card, its a PCB! Yes, you heard that right, its a custom pcb!  
It features an nfc chip you can flash to open a url or show text! When the phone makes contact, an LED lights up as well!

## Information

### Repo structure
```
ch0card (root)
|- BOMs
|  |- parts_bom.csv - the parts BOM, containing the components
|  |- pcb_and_pcba_bom.csv - the price of the PCB itself and PCBA from JLCPCB, from the time of writing
|
|- Images
|  |- 3d-back.png - Back of the pcb (3d model)
|  |- 3d-front.png - Front of the pcb (3d model)
|  |- pcb.png - The PCB, in the EasyEda Pro editor
|  |- schem.png - The schematic, in the EasyEda Pro editor
|
|- PCB
|  |- ch0card-gerbers.zip - The PCB gerber files (used to order the pcb)
|  |- ch0card-model.step - The 3D model of the pcb and components, in STEP form
|
|- README.md - This!!
```

### Details
It is a really simple PCB, containing only 5 components:
- NFC Chip (NTAG I2C Plus)
- The antenna (Copper traces on the PCB, forming a "coil")
- The led (amber/orange colored)
- A resistor
- A capacitor

### Images
![Front](Images/3d-front.png)
![Back](Images/3d-back.png)
![PCB](Images/pcb.png)
![Schematic](Images/schem.png)

## Making it yourself
To make something like this yourself, you can follow [this](https://jams.hackclub.com/jam/hacker-card) tutorial!  
When the PCB has arrived you can flash it using an app (Personally i use [NFC tools](https://play.google.com/store/apps/details?id=com.wakdev.wdnfc) which is availble for both android and iphone.  

Using your app of choice, flash the chip with this NFC command:  
`A2:03:E1:10:6D:00,A2:04:03:04:D8:00,A2:05:00:00:FE:00`  

Then you can write a url on it using the app! After that, people
can scan your card with their phone (assuming its on and nfc is enabled) and it will open the written website!

## Links
[EasyEda Pro project](https://oshwlab.com/cheetahdoespcb/project_jrpucpxz)  
[Pixl project](https://pixl.hackclub.com/explore/#project=293)  
[Github repo](https://github.com/CheetahDoesStuff/ch0card)  

### Do you think this is cool? Check out some of my other projects!
**Hardware**  
[USBuddy!](https://github.com/CheetahDoesStuff/USBuddy) - A small usb hub, for your keychain!  
[ExrPad v1](https://github.com/CheetahDoesStuff/ExrPad-v1) - A macropad with keys, a rotary encoder and a screen!  

**Software**  
[Raytracer](https://github.com/CheetahDoesStuff/Raytracer) - A CPU raytracer to render predefined scenes  
[Wrix](https://github.com/CheetahDoesStuff/wrix) - A simple chat room with HackClub auth  
[Kiln](https://github.com/CheetahDoesStuff/kiln) - A simple url shortener  
[Pesto](https://github.com/CheetahDoesStuff/pesto) - A pastebin clone  
[xv0](https://github.com/CheetahDoesStuff/xv0) - An operating system written in rust, from scract

Check out this and more on [my github](https://github.com/CheetahDoesStuff)!