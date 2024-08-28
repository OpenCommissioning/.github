# Welcome to Open Commissioning

![OC_Demo.png](images%2FOC_Demo.png)

**Open Commissioning** is an open source framework for virtual commissioning.
The goal is to provide an open platform for test and commission PLC code using a virtual model.

Project is based on [Unity](https://unity.com/) and [TwinCAT](https://www.beckhoff.com/en-en/products/automation/twincat/). 
From one side Unity provides modern 3D Editor with physics engine which allows to create interactive 3D environment, from other side TwinCAT is used as simulation unit that is able to emulate bus systems and behaviour models of actuators and sensors close to real time.

On the basis of this technology chain, it is possible to realise a Soft-/Hardware-in-the-loop simulation with PLC, with the main focus on achieving no code difference between virtual and real commissioning.

Here's why:
   * Develop and use state-of-the-art open virtual commissioning solution
   * Collaborate and use Knowledge-Sharing Culture
   * Avoid vendor lock and boost your automation workflow

# Description
## 1. Packages
The Open Commissioning has three main parts: 
1. [Unity Package](https://github.com/OpenCommissioning/Unity_Core): Scripts, Tools and Asset for creating virtual model and an environment within Unity Editor.
2. [TwinCAT Library](https://github.com/OpenCommissioning/TC_Standard): Pre-built behavior models for actors, sensors and various industrial devices.
3. [Assistant](https://github.com/OpenCommissioning/Assistant): Application orchestrates the Unity and TwinCAT sides, and provides an interface for connecting to external industrial systems.

> [!NOTE]
> More detailed information can be found in the corresponding sub repositories

## 2. Concept
The virtual commissioning project consists of the following parts:
 * **Unity Project**:
   The geometry, kinematics and material flow of the machine are replicated in a unity scene and parameterised with suitable sensors and actuators in order to reproduce the behaviour of the real machine.
 * **TwinCAT PLC Project**:
All actuators, sensors and other industrial devices are listed in the TwinCAT project according to the hierarchical structure from Unity Scene and linked to control signals.
The TwinCAT Project will run on isolated cores with 1 ms cycle time and provides a stable environment for Soft-/Hardware-in-the-loop simulation.
 * **Assistant**: The Assistant is used as an engineering tool and enables the use of various features such as project generation, configuration scanning, etc., which can be extended with the SDK.
In addition, the Assistant handles communication between TwinCAT, Unity and third-party interfaces and serves as a bridge for data connectivity.

![OS_System](./images/OC_Base_dark.png#gh-dark-mode-only)
![OS_System](./images/OC_Base_light.png#gh-light-mode-only)

# Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

We extend our gratitude to all our numerous contributors who create plugins, assist with issues and pull requests, and respond to questions on Discord and GitHub Discussions.

Refine is a community-driven project, and your contributions continually improve it.

> [!NOTE]  
> Further information on the contribution can be found in the corresponding sub repositories

# Credits
This open source project is initiated and supported by [SpiraTec AG](https://www.spiratec.com/en/).

:handshake: Credits for third-party software components and developers:

1. Used in Unity Package:
   * [Beckhoff ADS](https://www.nuget.org/packages/Beckhoff.TwinCAT.Ads) - Beckhoff protocol to communicate with TwinCAT devices
   * [NaughtyAttributes](https://github.com/dbrizov/NaughtyAttributes/) - NaughtyAttributes is an extension for the Unity Inspector
   * [UniTask](https://github.com/Cysharp/UniTask/) - Provides an efficient allocation free async/await integration for Unity
   * [ookii-dialogs-winforms](https://github.com/ookii-dialogs/ookii-dialogs-winforms/) - A class library for Windows Forms applications providing several common dialogs
   * [ShellFileDialogs](https://github.com/daiplusplus/ShellFileDialogs/) - File Open, File Save and Folder Browser dialogs

2. Used in TwinCAT Library:
   * [Beckhoff ADS](https://www.nuget.org/packages/Beckhoff.TwinCAT.Ads) - Beckhoff protocol to communicate with TwinCAT devices
   * [TcUnit](https://github.com/tcunit/TcUnit) - TwinCAT unit testing framework

3. Used in Assistant:
   * [TcPnScanner](https://github.com/TcHaxx/TcPnScanner) - Tool written in C#/.NET, that scans for Profinet packets on a network interface
   * [Beckhoff ADS](https://www.nuget.org/packages/Beckhoff.TwinCAT.Ads) - Beckhoff protocol to communicate with TwinCAT devices
   * [TCatSysManagerLib](https://www.nuget.org/packages/TCatSysManagerLib) - TwinCAT System Manager Library

# License
Open Commissioning framework is distributed under the BSD 3-Clause License.
> [!NOTE]  
> This package contains third-party software components that are subject to the licence(s) specified in the corresponding sub repositories

# Contact
For help and support, please contact us on [Discord](https://discordlink), GitHub Discussions or by [email](opencommissoning@spiratec.com).







