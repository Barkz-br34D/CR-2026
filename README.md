# CR-2026
Modernise a CR-10/s with as little money as possible with me!

This is my CR-10 that can compete with just about every bedslinger that was released in the last 3 years.

It is still a work in progress, and I take a very heavy function over form stance when it comes to personal projects. This one has been months in development, building, printing, and long nights.

Let’s start from the bottom.
Electronics:
BTT SKR Mini E3 V3 -TMC2209 Drivers 
Stock Creality Bed MOSFET
Raspberry Pi Zero2W
Factory Steppers (Except the Extruder (42-20) because its Direct Drive)
Factory Thermistors and Heaters
Factory Power Supply
BLTouch

Hardware:
Triangle labs DDE-R Direct Drive Kit
E3D V6 Hot end
Custom All-in-one (to suit my requirements)
Linear Rail X Axis W/cable chain
Printed Y Tensioner

My CR-10 uses a few very modern features including Klipper, KAMP bed mesh, sensorless homing and adaptive purge. I use Fluidd to control everything from my phone, and with OrcaSlicer I can send prints directly to the printer. The biggest headache is always the printer configuration. Telling Klipper what I want it to do and when.

V1.0 Let’s Get Started. Installing an SKR Mainboard, an all-metal Hot-end, a BLTouch and a fang cooler. Still marlin firmware and Bowden tube. Pretty basic stuff and It worked but I couldn’t print more than 80mm/s… not fast enough.
V1.1 Better Control. After fighting with the hot end, I pulled the trigger on the triangle labs Direct Drive extruder with a Bondtech BMG extruder and e3d V6 hot end (which is what you see on the printer now). This let me push more filament and crack the mighty 100mm/s (very unreliably and only on very basic geometry)
V1.2 Digitise Me. Installed the Pi and Klipper. That was not fun. 4 failed installs of Moonraker and countless printer config changes later I had it running but couldn’t get any better results in speed or quality. But I could print from Orca and see live temp, progress and command the printer form my phone. 
V1.3 Linear Rail. This was way more of headache than it should’ve been. A hot end mount made for a carriage that wasn’t made to go on a linear rail. Good times and great drilling. This took a measure 8 times, drill one hole, slot said hole because I was off by 0.6mm, measure 4 more times and drill the other 3 and pray. It worked. Smooth like butter. 
V2.0 The All-in-One. This was a huge step. Designed my own AIO box and mounts to suit my space. Keeping the form factor as small as possible whilst re-using as much as possible. I think I ended up reusing about half the bolts from the control box and only had to remake the Mains power wires and MOSFET wires. Its not pretty and I’ve made revisions but haven’t printed them yet as I’m waiting for V3.0.

V2.1 Modernise Me. This is where I pulled out all the stops. I had a reliable CR-10 printing 150mm/s on V-wheel Y/Z axis and 12V power… but its not enough. Sensorless homing, Kamp bed mesh and adaptive purge. What these do, in order: No more end stop clicks and faster homing (homing the whole printer in 10s or less is its already close to home); Kamp bed mesh relies on a saved bed mesh for the entire bed, and only meshes the printing area, meshing in a few seconds for benchy; adaptive purge keeps the nozzle pressure exactly where it needs to be right before the first layer goes down, cleaner first layer, better adhesion and less filament loss to the orca 150mm purge line.

THE FUTURE
V2.2 Linear Rod Y axis. Two 12mm linear rods for the Y axis and a belt upgrade for all the speed and smoothness. Along with looking pretty sweet.
V3.0 Electronics upgrade. I will be utilising a K1 Max bed with custom Y carriage, faster heating, lighter and the same print volume. As well as a VORON Stealthburner toolhead and Phaetus Rapido ceramic hot end. All on a 24V PSU. 

V3.1 The final Edition; Make it Pretty, Make it Industrial, Make it Bulletproof.

All this amounts to about 300mm/s and never having to watch a first layer ever again. Link Below for Parts, My Config, and more in-depth info about what and why. 
