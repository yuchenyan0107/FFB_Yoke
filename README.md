# FFB_Yoke

## Overview
A 3D printable Force-Feedback Yoke for flight

Big thanks to Aggressorblue and other people from the VPForce Discord community. He integrated 8020 and Gantry into this design.

https://makerworld.com/en/models/1763788-ffb-yoke-case-revised-for-2080-gantry#profileId-1876684

More information regarding the electronic part and TelemFFB can be found in VPforce's documentation:

https://docs.vpforce.eu/community-projects/ffb-yoke/

I also made my own FFB software, FSFFB, largely inspired by the TelemFFB. It is currently for experimental purposes and overall a simplified version compared to TelemFFB, but with some features better tuned, for example, trim following and AP following support, and stall buffeting.
The goal of the FSFFB project is to use advanced aerodynamic methods (e.g., VEM) to build a realistic control loading model, while keeping the computational cost relatively low, which allows real-time simulation.

https://github.com/yuchenyan0107/FSFFB

**It's forbidden to sell any part or kit of this project, whether or not it is profitable, without my agreement.**

Modifications are welcome, but the only way to publicly distribute modified files (if you are going to distribute) is to make them publicly available and non-profitable.

## Key features

- Dual-axis FFB using VPforce 57BLF03 motors (pitch and roll axes)
- Linear rail gantry system (smooth Y-axis travel)
- Belt-driven mechanics with adjustable tension
- 3D printable components (PETG-CF/ABS recommended)
- Compatible with Honeycomb Alpha yoke handle (with adapter)
- Open-source design with active community development
- Reasonably priced DIY project for FFB yoke enthusiasts

## Component list

https://docs.google.com/spreadsheets/d/1nBpdCx0DOBi1BcTt7vbbc8EsOH5HXZhTVgTmGyhsMfY/edit?gid=0#gid=

| Category | Part | Spec | Qty/Note | UnitPrice |
| --- | --- | --- | --- | --- |
| center shaft | steel shaft | D 16mm, L 350mm | 1 | 3 |
| center shaft | STHWR 16 |  | 2 | 5 |
| center shaft | shaft clamp | 16mm | 1 | 3 |
| bearings | 608 |  | 2 | 0.50 |
| bearings | MR16287 |  | 1 | 3 |
| bearings | 6808 |  | 1 | 2 |
| linear rails | MGNR12 | 300mm | 2 | 5 |
| linear bearing | MGN12 C |  | 4 | 3 |
| pulleys | HTD 5M 12T | width 15mm, inner D 8mm | 2 | 2 |
| pulleys | HTD 5M belt | 750mm | 1 | 2 |
| pulleys | HTD 5M belt | 335mm | 1 | 1 |
| electric | potentiometer |  | 10k ohm | 1 |
| electric | emergency stop |  | 16mm | 2 |
| electric | 16 AWG |  |  | 1 |
| electric | micro JST XH | 2, 3, 5 pin & wire |  | 2 |
| electric | ALPS 8 way |  |  | 2 |
| Screws | M3*10 | M4*10 | M8*50 |  |
| Insert | M4 OD6 L6 | M3 OD5 L4 |  | 2 |

## Assembly Process Overview

**Important:** Before printing any parts, calibrate your printer regarding both the overall dimension and hole tolerance. Otherwise, the parts may not fit together.
When I built this with my Bambulab A1, I needed to set +0.6% for the x-axis, +0.3% for the y-axis, and -0.1mm for the holes.

Steps to install linear rails and bearings on the Y-axis gantry:

1. Screw two case bottom plates
2. Install two linear rails on the bottom plate; don’t tighten the screws.
3. Install bearing blocks on the linear rails (use the plastic guide rail while installing the bearing to prevent damage!)
4. Install the x_assembly bottom plate (without other parts) to the bearing blocks. Don’t make the screws very tight yet.
5. Slide the module on the linear rails back and forth while gradually tightening the screws on the linear rail and the bearing blocks. So that there’s minimal stress on the system
6. Unmount the bearing blocks and the x assembly plate from the linear rails, then finish the x-assembly
7. Install the x_assembly back to the linear rails, use the place guide rail to help with the installation.

Steps to assemble the Y-axis belt part to get good tension and smoothness

1. Mount the motor with 4 M6 bolts. Don't tighten them completely, because the motor needs to be moved backwards a little bit
2. Get the pulleys and belt installed. The belt doesn't need to be super tight at this moment. Just clamp it at a position 1 tooth before it's tensioned
3. Install the case plates (front, left side, back)
4. Use 2 M4 bolts to push the motor backwards to tension the belt. While tensioning the belt, move the gantry to feel the force needed to move it. The belt should be relatively tight, while not making too much additional friction, 
5. Tighten 4 of the M6 bolts that hold the motor

## Gallery

![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/front.png "front view")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/side.jpg "picture from the side")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/top_side.webp "picture from the side")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/belt_tensioner.jpg "Y_motor_belt")

## Notes regarding VPforce setup and software

**Simulator Compatibility:**

- **MSFS:** Full TelemFFB support, trim following works with A2A aircraft (Comanche verified)
- **Advanced Airliner Add-ons in MSFS:** TelemFFB trim/AP following is not yet supported for PMDG, TFDI, and similar complex aircraft. Most of the modern airliners don't have trim following anyway.
- **X-Plane:** TelemFFB support available
- **DCS World:** DirectInput FFB support (and TelemFFB added to it). It works great with the C-130.

**Motor Range Considerations:**

- Yoke travel range exceeds 360° motor rotation
- **Critical:** Yoke must be positioned near center when powered on
- Motor range mapping accounts for extended yoke travel angles
- Does not require exact centering, but should be approximately centered on startup

!!! important "Power-On Position"
    Position yoke approximately in center position before powering on system. Yoke travel range corresponds to more than 360° of motor rotation, requiring centered startup for proper calibration.

**VKB/Virpil/Thrustmaster Grips:**

- Not applicable (yoke-specific design, not joystick grip compatible)
