# Jaco2-CodeSys-projects
Current repository includes two CodeSys projects implemented in order to be used along with [Jaco2-ROS-TCPIP-pkgs](https://github.com/mdiamanti/Jaco2-ROS-TCPIP-pkgs) and [Jaco2-ROS-CAN-pkgs](https://github.com/mdiamanti/Jaco2-ROS-CAN-pkgs) respectively. The aim of `raspberry_tcp_ip.project` and `raspberry_can.project` is to develop a HMI (Human Machine Interface), or else a graphical user interface, that enables remote communication and control of Kinova Jaco<sup>2</sup> 6 DOF robotic arm.

## Technical Specifications
`raspberry_tcp_ip.project` and `raspberry_can.project` CodeSys projects are based on the microcomputer **Raspberry Pi 3 Model B**. Raspberry Pi plays the role of the programmable logic controller of a small scale industrial control scheme that controls the movement of a 6 DOF robotic arm. For this reason, Raspberry Pi was turned after a "Soft PLC" by using the license [CODESYS Control for Raspberry Pi SL](https://store.codesys.com/codesys-control-for-raspberry-pi-sl.html). More information about the system requirements and the installation of the license can be found in the link above and the official page of CODESYS Store. 

The main idea behind each project is summed up by the following images:

### raspberry_tcp_ip.project
A connection between the Raspberry Pi microcomputer and the PC that runs the robot simulation is established using the TCP/IP protocol, as shown below. There are two ways to establish such a connection: 
   1. Using a crossover Ethernet cable
   2. Using a patch Ethernet cable and a switch</br> 

![tcpip_idea - smaller](https://user-images.githubusercontent.com/39567867/43639191-15b12f0a-9724-11e8-8f65-8b7669e956fa.png)

### raspberry_can.project
In order to establish a CANbus connection between a Raspberry Pi and a PC, there is need for extra hardware that extends the capabilities of our hardware configuration and enables the appropriate CANbus interconnection.
   1. [PiCAN2 CANbus Board](http://skpang.co.uk/catalog/pican2-canbus-board-for-raspberry-pi-23-p-1475.html) was used from the side of Raspberry Pi to provide the CAN interface needed
   2. [PCAN-USB adapter](https://www.peak-system.com/PCAN-USB.199.0.html?&L=1) was chosen to connect the PiCAN2 hat with the PC</br>
   
![can_idea - smaller](https://user-images.githubusercontent.com/39567867/43639220-27745b86-9724-11e8-9461-e5636b725b92.png)

