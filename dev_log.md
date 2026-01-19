## 2024/12/24:
I have decided to use Onshape as the main platform to share CAD files. This is for a multitude of reasons:
- Solidworks: Great, but barely any hobbyists have access to it (v. expensive licence, no free options).
- Fusion: Great, but unfortunately its workflow is significantly different to Onshape/Inventor/Solidworks WRT assemblies and other factors. I don't know it well enough to make high-quality models quite frankly.
- Onshape: Great, only downside is it's 100% cloud-based, so no native file format exports (only STEP/STL/etc).

As I have used both Onshape and Solidworks extensively, I will be proceeding with Onshape to better facilitate open-source development and modifications! As it is free for hobbyists to use, I will host the project there and export STEP models to this repository.

## 2024/12/31:
Significant progress has been achieved on the CAD front!

- link

The keyboard is now essentially at the stage where I must consider the logistics of how everything works together/connects/is wired/is flashed/where boards are mounted/how boards are mounted.

At this stage, I do *not* have LED indicators or digital displays to show layer information etc etc. Nor do I have any capacity for module expansions for mice etc. I definitely want these in the future!

Wiring Diagram + Pro Micro wiring ideas:

![image](https://github.com/user-attachments/assets/c0bebc20-9476-48ce-8f25-5d49259b93cc)

![image](https://github.com/user-attachments/assets/e114a9fe-7350-46a6-863f-9d5e23d94a9a)

![image](https://github.com/user-attachments/assets/a63e2151-dd35-46a4-bf7f-bb1377fc8c9b) ![image](https://github.com/user-attachments/assets/d768d07a-7470-444f-a9ca-2aad14a6648e)

## 2025/01/03
Looks like UHK is also copying Dygma's thumb cluster design now!
![image](https://github.com/user-attachments/assets/0eeba1a4-3271-4a6e-bd69-98038079450b)
Well, good designs should be imitated/modified! But will mine be better or worse...?

Also firmware/keymaps/layers/microcontroller pins work is being done, albeit in my qmk fork. I might copy it over here later when it's more mature.

In the meantime, here's a CAD update:

Overall:
![2025_13:32:54](https://github.com/user-attachments/assets/9dd47040-1fee-4582-89a2-83b8d14b90ae)

Sectional:
![image](https://github.com/user-attachments/assets/868d9ced-273a-415c-878d-cdb43549efc9)


## 2025/01/06
Just figured out how the pins on the pro micro are meant to go... It turns out al the calculators and QMK tools are using the on-board controller's pin names, not the pinouts of the actual boards. If we consider the ATMEGA32U4-MU's pinout mapped to the pro micro's physical pins, we get:

![image](https://github.com/user-attachments/assets/92243c2a-ca1c-40a6-a3c9-37ab01c71637)

Much easier!

## 2025/01/07
Did a lot of research today WRT I2C vs UART serial connections, and which is better for connecting the keyboard halves. Decided on UART serial.

Drafted up a few (incorrect) base wiring diagrams and ordered a lot of new parts (reset switch, switches, screws, etc).

## 2025/01/12
Printed off some test pieces 2 days ago and test fitted the pro micro an audio jack until they fitted. No reset button yet, so that will remain to be seen.

Also I *forgot about the magnets* connecting the two halves! Not sure if I have any 4x2mm circular magnets left, will have to order them tomorrow.

Printed off left and right plates in PLA today. Will make first keyboard iteration using just these, but will upgrade to metal in future I think.

Photos to come.

## 2025/03/09
Yeah, kinda gave up making a log lol.
rip

## 2026/01/19
Classic me got a bit distracted.
Anyawy.
Got a bit too clever and lost my keyboard.json file, and wiring diagrams. I guess this is what happens when you forget about a project for a year. Ah well.

