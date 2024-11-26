# Welcome to Open Commissioning

![OC_Demo.png](images%2FOC_Demo.gif)

**Open Commissioning** is an open source framework for virtual commissioning.
The goal is to provide an open platform for testing and commissioning of PLC code using a virtual model.

The project is based on [Unity](https://unity.com/) and [TwinCAT](https://www.beckhoff.com/en-en/products/automation/twincat/). 
Unity provides a modern 3D Editor with a physics engine to create an interactive 3D environment and physics simulation. TwinCAT is used as a simulation unit that is able to emulate industrial bus systems and behaviour models of actuators and sensors close to real time.
These two platforms are connected to form the model for virtual commissioning

On the basis of this technology chain, it is possible to realize a Soft-/Hardware-in-the-loop simulation with a PLC, focusing on achieving no code difference between virtual and real commissioning.

# Why?
The project is initiated by a dedicated team with 15+ years of experience in automation projects and virtual commissioning across automotive, logistics and other industries. Having worked extensively with various tools and vendor-locked solutions, it is now the time to establish an open framework for virtual commissioning.

The key objectives are:

* Developing and using a state-of-the-art open virtual commissioning solution
* Collaborating and using knowledge-sharing culture
* Avoiding vendor lock and boosting your automation workflow

# Concept
The Open Commissioning framework is built on three core technologies:
 * **[Unity Package](https://github.com/OpenCommissioning/OC_Unity_Core)**:
   Geometry, kinematics and product transport are replicated in a Unity scene with suitable sensors and actuators in order to reproduce the mechanic behaviour of a real machine.
 * **[TwinCAT Library](https://github.com/OpenCommissioning/OC_TwinCAT_Core)**:
All actuators, sensors and other industrial devices are listed in the TwinCAT project according to the hierarchical structure from the Unity scene and linked to control signals.
The TwinCAT Project can run on isolated cores with 1 ms cycle time and provides a stable environment for Soft-/Hardware-in-the-loop simulations.
 * **[Assistant Application](https://github.com/OpenCommissioning/OC_Assistant)**: The Assistant application is used as an engineering tool and features various functions such as project generation and configuration scanning. It also handles communication between TwinCAT and third-party interfaces and serves as a bridge for data connectivity, which can be extended via plugins.

![OS_System](./images/OC_Overview_dark.png#gh-dark-mode-only)
![OS_System](./images/OC_Overview_light.png#gh-light-mode-only)

> [!NOTE]
> More detailed information can be found in the corresponding repositories.

# Contributing
Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement". Don't forget to give the project a star! Thanks again!

We extend our gratitude to all our numerous contributors who create plugins, assist with issues and pull requests, and respond to questions in GitHub Discussions.

Check our [contribution guide](CONTRIBUTING.md).

Open Commissioning is a community-driven project, and your contributions continually improve it.

> [!NOTE]  
> Further information about contributing can be found in the corresponding repositories.

# Credits for third-party software components and developers :handshake:

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
Open Commissioning Project is distributed under the BSD 3-Clause License.
> [!NOTE]  
> This package contains third-party software components that are subject to the licence(s) specified in their repositories.

# Initiative
This open source project is initiated and supported by [SpiraTec AG](https://www.spiratec.com/en/).

<img src="./images/spira_logo_light.png#gh-light-mode-only" width="200"/>
<img src="./images/spira_logo_dark.png#gh-dark-mode-only" width="200"/>

_**SpiraTec AG** is a globally active company for industrial engineering and high-tech solutions for digital transformation in the process industry, specializing in engineering, robotics, automation, and industrial IT systems. With a team across 40+ locations, we deliver end-to-end solutions, from consulting and system engineering to commissioning and optimization._

# Contact
- **Public Discussions**:  
  For general questions, feedback, or public topics, feel free to start a discussion in the [Discussions](https://github.com/orgs/OpenCommissioning/discussions) section

- **Personal Support & Project Enquiries**:  
  For personal assistance, support, or project-related enquiries, please mail to  [opencommissioning@spiratec.com](mailto:opencommissioning@spiratec.com)
