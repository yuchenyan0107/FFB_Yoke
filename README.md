# FFB_Yoke
A 3D printable Force-Feedback Yoke for flight

Developed based on VPForce Rhino with 57BLF03 motors, and it should be compatible with other 57 motors.

Parts list and reference price:

https://docs.google.com/spreadsheets/d/1nBpdCx0DOBi1BcTt7vbbc8EsOH5HXZhTVgTmGyhsMfY/edit?gid=0#gid=

| Category | Part | Spec | Qty/Note | UnitPrice |
| --- | --- | --- | --- | --- |
| center shaft | steel shaft | D 16mm, L 350mm | 1 | 3 |
| center shaft | STHWR 16 |  | 2 | 5 |
| center shaft | shaft clamp | 16mm | 1 | 3 |
| bearings | 608 | not being used now | a few | 0.50 |
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


Steps to install linear rails and bearings on Y Y-axis gantry:

1. Screw two case bottom plates
2. Install two linear rails on the bottom plate, don’t tight the screws.
3. Install bearing blocks on the linear rails (use the plastic guide rail while installing the bearing to prevent damage!)
4. Install the x_assembly bottom plate (without other parts) to the bearing blocks. Don’t make then screws very tight
5. Slide the module on the linear rails back and forth while gradually tight the screws on the linear rail and the bearing blocks. So that there’s minimum stress on the system
6. Unmount the bearing blocks and the x assembly plate from the linear rails, then finish the x-assembly
7. Install the x_assembly back to the linear rails, use the place guide rail to help the install.

Steps to assemble the Y-axis belt part to get good tension and smoothness

1. Mount the motor with 4 M6 bolts. Don't tighten them completely, because the motor needs to be moved backwards a little bit
2. Get the pulleys and belt installed. The belt doesn't need to be super tight at this moment. Just clamp it at a position 1 tooth before it's tensioned
3. Install the case plates (front, left side, back)
4. Use 2 M4 bolts to push the motor backwards to tension the belt. While tensioning the belt, move the gantry to feel the force needed to move it. The belt should be relatively tight, while not making too much additional friction, 
5. Tighten 4 of the M6 bolts that hold the motor

![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/front.png "front view")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/side.jpg "picture from the side")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/top_side.webp "picture from the side")
![alt text](https://github.com/yuchenyan0107/FFB_Yoke/blob/main/pictures/belt_tensioner.jpg "Y_motor_belt")

