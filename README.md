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