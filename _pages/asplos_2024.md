---
layout: page
permalink: /tutorials/asplos_2024
title: ASPLOS 2024
description: GeneSys Tutorial | April 28, 2024 | 1:30 PM - 5:00 PM PST | Grande D
nav: false
nav_order: 0
---

# Overview
This tutorial will present a discussion on emerging deep learning models along with a comprehensive walkthrough of our newly developed system, _GeneSys_.
Attendees will gain valuable insights into our cutting-edge technology and its wide-ranging applications in the field of DNN acceleration systems.

# Goals
We aim for attendees to gain a thorough understanding of the functionalities of our innovative system.
They will learn how it can be effectively implemented in various applications and be equipped with the knowledge to harness its potential for their own projects and research in deep learning and DNN acceleration systems.

# Who Should Attend
Researchers and developers interested in deep learning systems, compiler development, and hardware/software design for DNN acceleration systems.

# Logistics
- **Venue:** [ASPLOS 2024](https://www.asplos-conference.org/asplos2024/)
- **Date:** April 28, 2024
- **Time:** 1:30 PM - 5:00 PM PST
- **Registration:** To secure your spot for our tutorial, please sign up for at least a "One-day Workshops/Tutorials Registration". You can register [here](https://whova.com/portal/registration/asplo_202403/).

# Schedule

| Start (EST) | End (EST) | Agenda | Presenter | Resources |
| :---------: | :-------: | :----- | :-------: | :-------: | 
| **1:30 PM** | **1:50 PM** | **Introduction** | Hadi | [slides](https://drive.google.com/file/d/1p0Q790UhU0BNazOf7gDTU9q8qqxPTd8w/view?usp=sharing) |
| | | History and challenges of hardware acceleration <br /> Introduction to _GeneSys_ | | [video](https://youtu.be/pHbY0No3MCU) |
| **1:50 PM** | **2:00 PM** | **Motivation** | Rohan | [slides](https://drive.google.com/file/d/1jNKl7vr2VSOMYfU--JscGImHKzmXJTuz/view?usp=sharing) |
| | | Neural networks and hardware acceleration <br /> Inference pipeline – datacenters and edge <br /> Systems challenges and opportunities <br /> Overview of _GeneSys_ <br /> Example usage of _GeneSys_ in research projects | | [video](https://youtu.be/Z8OYHT1-kmk) |
| **2:00 PM** | **3:00 PM** | **_GeneSys_ Architecture** | Soroush | [slides](https://drive.google.com/file/d/1V3ROnTi7FAZ_Z_1YU9QW9qobb572tRx8/view?usp=sharing) | 
| | | _GeneSys_ NPU overview <br /> Systolic array <br /> On-chip memory architecture and memory interface <br /> Tandem processor <br /> End-to-end neural network execution <br /> ISA | | [video](https://youtu.be/IpW-7lXNiB0) |
| **3:00 PM** | **3:30 PM** | *Afternoon Break* | | | 
| **3:30 PM** | **4:30 PM** | **_GeneSys_ Compiler** | Chris | [slides](https://drive.google.com/file/d/1tSkvlXoaMRwQNYQOldDi65vo1Lj276GA/view?usp=sharing) |
| | | Introduction to compilation <br /> Compilation challenges for DNN accelerators <br /> _f_-DFG frontend <br /> Codelet backend <br /> Compiler overview <br /> Using the compiler and tailoring it to your needs <br /> Realities about end-to-end applications <br /> *FhY:* Cross-domain compilation stack for multi-acceleration | | [video](https://youtu.be/W_L9zNw_NAo) |
| | | *Demo:* Compiling ResNet50, changing tiling, loop order, on-chip buffers, fusing layers | | video coming soon... |
| **4:30 PM** | **5:00 PM** | **_GeneSys_ Uses, Verification, and Software Simulator** | Hanyang | [slides](https://drive.google.com/file/d/1uQec9sBoE3-6rlWfjsw_BzisL47msEsR/view?usp=sharing) |
| | | Example problem: data motion acceleration <br /> Example problem: neuromodulation for brain-implantable devices <br /> Quantization on _GeneSys_ <br /> Python APIs <br /> Software simulator <br /> RTL simulation <br /> Validation with FPGA | | [video](https://youtu.be/Sz-h7kPhqvo) |

# Presenters
- **Hadi Esmaeilzadeh**: Halicioğlu Chair in computer architecture and professor at the University of California, San Diego
- **Soroush Ghodrati**: System Architect at Apple
- **Rohan Mahapatra**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Hanyang Xu**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Christopher Priebe**: Ph.D. student in computer science and engineering at the University of California, San Diego
