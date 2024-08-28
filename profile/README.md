# Welcome to Open Commissioning

![OC_Demo.png](images%2FOC_Demo.png)

**Open Commissioning** is open source project for virtual commissioning.
The goal is to provide an open platform for low level virtual commissioning.

Here's why:
+ Collaborate and use Knowledge-Sharing Culture
+ Develop state-of-the-art solution for virtual commissioning
+ Avoid vendor lock

Commissioning is based on [Unity](https://unity.com/) and [TwinCAT](https://www.beckhoff.com/en-en/products/automation/twincat/). 
From one side Unity provides modern physics engine with 3D editor which allows to create interactive 3d environment, from other side TwinCAT is used as simulation unit that is able to emulate bus systems and behaviour models of actuators and sensors close to real time.

On the basis of this technology chain, it is possible to realise a Soft-/Hardware-in-the-loop simulation with PLC, with the main focus on achieving no code difference between virtual and real commissioning.

# Description
## 1. Packages
The Open Commissioning has main parts: 
1. [Unity Package](https://github.com/OpenCommissioning/Unity_Core): Scripts, Tools and Asset for creating virtual model and environment within Unity Editor.
2. [TwinCAT Library](https://github.com/OpenCommissioning/TC_Standard): Pre-built behavior models for actors, sensors and various industrial devices.
3. [Assistant](https://github.com/OpenCommissioning/Assistant): This application orchestrates the Unity and TwinCAT sides, and provides an interface for connecting to external industrial systems.

> [!NOTE]
> You can find more detailed information in the corresponding package sources.

## 2. Concept
The simulation is divided into two main parts, each of which runs in an environment best suited to the respective tasks:
 * **Unity Project**: 
In Unity project with the help of the Open Commissioning package the virtual machine is created. 
The kinematic chain and calculation of the physics is achieved with functions provided by Unity Engine and PhysX.
 * **TwinCAT Project**: 
On the TwinCAT side, the behavioural function blocks for each actuator and sensor of the virtual machine are mapped and called in a PLC task. 
The cycle time of 1 ms on an isolated core enables real-time simulation with coupled controller and provides a stable environment for Soft-/Hardware-in-the-loop simulation.
 * **Assistant**: The Assistant is used as an engineering tool and enables the use of various features such as project generation, configuration scanning, etc., which can be extended with the SDK.
In addition, the Assistant handles communication between TwinCAT, Unity and third-party interfaces and serves as a bridge for data connectivity.

The abstract structure of the system is shown in the following image.
![OS_System](./images/OC_Base_dark.png#gh-dark-mode-only)
![OS_System](./images/OC_Base_light.png#gh-light-mode-only)

# Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

We extend our gratitude to all our numerous contributors who create plugins, assist with issues and pull requests, and respond to questions on Discord and GitHub Discussions.

Refine is a community-driven project, and your contributions continually improve it.

> [!NOTE]  
> Further information on the contribution can be found in the individual subsections of the open commissioning.

# Credits
This open source project is initiated and supported by [SpiraTec AG](https://www.spiratec.com/en/).

:handshake: Credits for third-party software components and developers:

1. Used in Unity Package:
   * [Beckhoff ADS](https://github.com/Beckhoff/ADS) - Beckhoff protocol to communicate with TwinCAT devices
   * [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes/) - NaughtyAttributes is an extension for the Unity Inspector
   * [UniTask](https://github.com/Cysharp/UniTask/) - Provides an efficient allocation free async/await integration for Unity
   * [ookii-dialogs-winforms](https://github.com/ookii-dialogs/ookii-dialogs-winforms/) - A class library for Windows Forms applications providing several common dialogs
   * [ShellFileDialogs](https://github.com/daiplusplus/ShellFileDialogs/) - File Open, File Save and Folder Browser dialogs

2. Used in TwinCAT Library:
   * [Beckhoff ADS](https://github.com/Beckhoff/ADS) - Beckhoff protocol to communicate with TwinCAT devices
   * [TcUnit](https://github.com/tcunit/TcUnit) - TwinCAT unit testing framework

3. Used in Assistant:
   * [Beckhoff ADS](https://github.com/Beckhoff/ADS) - Beckhoff protocol to communicate with TwinCAT devices
   * [TcPnScanner](https://github.com/TcHaxx/TcPnScanner) - Tool written in C#/.NET, that scans for Profinet packets on a network interface

# License
Open Commissioning components are distributed under the BSD 3-Clause License.
> [!NOTE]  
> This package contains third-party software components that are subject to the licence(s) specified in the individual subsections of the open commissioning.

# Contact
For help and support, please contact us on [Discord](https://discordlink), GitHub Discussions or by [email](https://spiratec.com/contact/opencommissoning).







