# MeCO Docs

This is a meta repository containing all documentation related to the Medium Cost Open (MeCO) AUV. This is a living 
document that will undergo changes over the life of the project. To access the wiki page, use the following link:

- [MeCO Wiki](https://github.umn.edu/meco-auv/meco-docs/wiki) 

## GitHub Repositories

The MeCO project is spread across multiple GitHub repositories that all belong to the meco-auv GitHub organization. 
Certain repositories are meant to be deployed to certain computers for robot operation. The Dev machine is any x86 computer used for code development,
Jetson is the Jetson Orin NX onboard MeCO, Control Teensy is the Teensy 4.1 onboard MeCO, and OCU is the operational control 
unit, which is the laptop used to connect to MeCO via tether. 

| Repo link                                                          | Description                                                                                                                                                                     | Deployment         |
|--------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-------------------|
| [**meco-docs**](https://github.umn.edu/meco-auv/meco-docs)         | This repository.                                                                                                                                                                | N/A                |
| [**meco-setup**](https://github.umn.edu/meco-auv/meco-setup)       | Meta repository containing scripts and resources to setup and develop the software stack for the MeCO AUV. **Use the script in this repository to clone code for development.** | Jetson & Dev & OCU |
| [**teensy-meta**](https://github.umn.edu/meco-auv/teensy-meta)     | Meta repository containing resources for writing microROS C code for MeCO using the Teensy 4.1 microcontroller.                                                                 | Dev                |
| [**motion**](https://github.umn.edu/meco-auv/motion)               | Teensy ROS2 C code for AUV motion control.                                                                                                                                      | Control Teensy     |
| [**teleop**](https://github.umn.edu/meco-auv/teleop)               | ROS2 C++ package for teleoperating the MeCO AUV.                                                                                                                                | Jetson             |
| [**configuration**](https://github.umn.edu/meco-auv/configuration) | ROS2 package containing custom message types and configuration files related to the MeCO AUV.                                                                                   | Jetson & OCU       |

## Teensy Code Development
Use the [meco-setup](https://github.umn.edu/meco-auv/meco-setup) repository to install necessary dependencies to write 
and upload microROS code to the Teensy 4.1.

Once installed, follow directions in the [teensy-meta](https://github.umn.edu/meco-auv/teensy-meta) repository to launch 
the Arduino IDE, then open the Arduino code in the [motion](https://github.umn.edu/meco-auv/motion) package to upload to the 
Teensy.



## Resources

[Parker Microstrain 3DM-CV7 AHRS Docs](https://s3.amazonaws.com/files.microstrain.com/CV7+Online/Home.htm)
