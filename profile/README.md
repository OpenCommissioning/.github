# Welcome to Open Commissioning

**Open Commissioning** is open source project for virtual commissioning based on Unity and TwinCAT.
The goal is to provide an open platform for virtual commissioning with PLC (Soft-/Hardware-in-the-Loop simulation).

Here's why:
+ Collaborate and use Knowledge-Sharing Culture
+ Develop state-of-the-art solution for virtual commissioning
+ Avoid vendor lock

# Description
## 1. Packages
The Open Commissioning Project has main parts: 
1. **Unity Package**: Scripts, Tools and Asset for creating virtual model and environment within Unity Editor.
2. **TwinCAT Library**: Pre-built behavior models for actors, sensors and various industrial devices.
3. **Assistant**: This application orchestrates the Unity and TwinCAT sides, and provides an interface for connecting to external industrial systems.

For full documentation, visit:
1. [Unity Package](https://github.com/OpenCommissioning/Unity_Core)
2. [TwinCAT Library](https://github.com/OpenCommissioning/TC_Standard)
3. [Assistant](https://github.com/OpenCommissioning/Assistant)

## 2. Concept
The simulation is divided into two main parts, each of which runs in an environment best suited to the respective tasks:
 * **Unity Project**: 
In Unity project with the help of the Open Commissioning package the virtual machine is created and simulated. 
The kinematic chain and calculation of the physics is achieved with functions provided by Unity Engine and PhysX.
 * **TwinCAT Project**: 
On the TwinCAT side, the behavioural function blocks for each actuator and sensor of the virtual machine are mapped and called in a PLC task. 
The cycle time of 1 ms on an isolated core enables real-time simulation with coupled controller and provides a stable environment for Soft-/Hardware-in-the-loop simulation.
 * **Assistant**: The Assistant is used as an engineering tool and enables TwinCAT project generation based on the configuration from the Unity model. Data exchange between Unity and TwinCAT is realised using ADS. 
In addition, the Assistant manages communication between TwinCAT and third-party interfaces and serves as a bridge for data connectivity.

The structure of the system is shown in the following illustration.

![OS_System](./images/OC_Base_dark.png#gh-dark-mode-only)
![OS_System](./images/OC_Base_light.png#gh-light-mode-only)

You can find more detailed information in the corresponding package sources.

# Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

Fork the Project
1. Create your Feature Branch (git checkout -b feature/AmazingFeature)
2. Commit your Changes (git commit -m 'Add some AmazingFeature')
3. Push to the Branch (git push origin feature/AmazingFeature)
4. Open a Pull Request


We extend our gratitude to all our numerous contributors who create plugins, assist with issues and pull requests, and respond to questions on Discord and GitHub Discussions.

Refine is a community-driven project, and your contributions continually improve it.

# License
Open Commissioning components are distributed under the MIT License. 

See LICENSE.txt for more information.

# Credits
This open source project is initiated by [SpiraTec AG](https://www.spiratec.com/en/)

# Contact
For help and support, please contact us on Discord, GitHub Discussions or by email.







