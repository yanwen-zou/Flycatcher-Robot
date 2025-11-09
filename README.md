# Flycatcher-Robot

> 愛すべきお客様に、ハートフルな今日と、最高の笑顔を。

<div style="text-align: center;">
  <img src="img/Flycatcher_Robot.jpg" style="width: 80%;"/>
</div>

This project is a replica of the Flycatcher Robot from the anime *Apocalypse Hotel*, designed as an open-source desktop-level quadruped robot. 

The majority of the hardware in this project consists of available standard items with links or 3D-printing parts. The CAD Model, BOM List, and assembly notes are provided.

## CAD Model

<div style="display: flex; justify-content: space-between;">
  <img src="img/CAD_1.png" style="width: 48%;"/>
  <img src="img/3D_Printing.jpg" style="width: 48%;"/>
</div>
Check the STL/STEP files [here](https://github.com/yanwen-zou/Flycatcher-Robot/tree/main/model).


It is recommended to print using PLA and with tree support.

## BOM List

### Mechanical Parts

| Part Name      | Link                               | Price   | Notes               |
| -------------- | ---------------------------------- | ------- | ------------------- |
| M2*10 Screws   | [Link](#)                          | ¥XX.XX  | For assembly        |
| Knurled Nuts   | [Link](#)                          | ¥XX.XX  | For thigh-body connection |
| 3D Printed Parts | [Link](#)                         | ¥XX.XX  | Self-printing required |
| ...            | ...                                | ...     | ...                 |

### Electronics

| Part Name      | Link                               | Price   | Notes               |
| -------------- | ---------------------------------- | ------- | ------------------- |
| ZhiLing 16-channel Servo Board | [Link](#)        | ¥XX.XX  | Used as the main control board |
| Battery        | [Link](#)                          | ¥XX.XX  | Choose based on your needs |
| Control Wires  | [Link](#)                          | ¥XX.XX  | For connecting servos and the control board |
| ...            | ...                                | ...     | ...                 |

Note: For the electronics, you can choose different control methods based on your needs.

## Assembly Notes

1. Most screws used in the assembly are M2*10.
2. Due to the complexity of the mechanism and the precision of 3D printing, the head and body connection currently uses hot melt glue for attachment. It is recommended not to install the head until control logic debugging is complete. Feel free to modify the design based on the current model for a more refined joint mechanism or easier disassembly and contribute your changes!
3. The thigh-to-body connection parts require the insertion of two knurled nuts, which can be easily done using needle-nose pliers and a small hammer.
4. Similar to step 2, the leg shell is also attached using hot melt glue, so it is recommended to install it last.

## Wiring and Control

We use the ZhiLing 16-channel servo control board as the main control board for this project. This is just a reference. Follow the official documentation to connect the servo wires to the control board and define the interfaces in the software. It is important to note that for the four servos controlling the wheels, their wires need to be extended.

The joystick is used to control the robot in this project. Similarly, you can find in the official documentation how to map joystick buttons to control signals for each or multiple servos.

