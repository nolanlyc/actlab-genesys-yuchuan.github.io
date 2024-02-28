---
layout: page
permalink: /home/micro_2023 # NOTE: MICRO 2023 tutorial link is different to ensure legacy support because MICRO 2023 workshop/tutorial webpage links to .../home/micro_2023 instead of .../tutorials/micro_2023
title: MICRO 2023
description: GeneSys Tutorial | October 29, 2023 | 1:00 PM - 5:00 PM EDT | Harbour Salon A
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
- **Venue:** [MICRO 2023](https://microarch.org/micro56/index.php)
- **Date:** October 29, 2023
- **Time:** 1:00 PM - 5:00 PM EDT
- **Registration:** To secure your spot for our tutorial, please sign up for at least a "One-Day Workshop/Tutorial" with October 29, 2023 as your preferred date of attendance. You can register [here](https://microarch.org/micro56/attend/register.php).

# Schedule

| Start (EST) | End (EST) | Agenda | Presenter | Resources |
| :---------: | :-------: | :----- | :-------: | :-------: | 
| **1:00 PM** | **1:30 PM** | **Introduction** | Hadi | [slides](https://drive.google.com/file/d/1E8Nxq5RPDpJ-WdlaAwh6_UkjYBydnXuk/view?usp=sharing) |
| | | DNNs, LLMs, and hardware acceleration | | [video](https://youtu.be/8yxQDh4l_4M) |
| | | Need for open-source toolchain | | " |
| | | GeneSys overview | | [video](https://youtu.be/SjjT7Vpl14s) |
| | | Potential use cases | | " |
| **1:30 PM** | **1:50 PM** | **_GeneSys_ Architecture** | Rohan | [slides](https://drive.google.com/file/d/1HPd8SXfWXGB0kghUW_ZJxC5kvaqaShP8/view?usp=sharing) | 
| | | Systolic array | | [video](https://youtu.be/ZcIiuOYtepo) |
| | | SIMD array | | " |
| | | On-chip memory architecture and memory interface | | " |
<!-- Not in the slides or video! -->
<!-- | | | ISA | | | -->
| | | Tiled execution | | [video](https://youtu.be/0BbQONPVFyE) |
| **1:50 PM** | **2:30 PM** | **_GeneSys_ Verification** | Lavanya | [slides](https://drive.google.com/file/d/1xCwBLS6qwOU3qSmTj65pPdOrC9lPvhEE/view?usp=sharing) |
| | | RTL simulation | | |
| | | Hardware emulation | | |
| | | FPGA implementation and synthesis | | |
| | | Python driver | | |
| | | *Interactive Activity:* Configuring GeneSys 16x16; observe it is 16x16; run a single layer | | |
| | | *Interactive Activity:* Configuring GeneSys 4x4; observe it is 4x4; run same layer | | |
| | | *Demo:* FPGA | | |
| **2:30 PM** | **4:00 PM** | **Compiler and Programming Model** | Chris | [slides](https://drive.google.com/file/d/1HM5_2ne8TZROW2Uq0JsTb31fPGdWd85b/view?usp=sharing) |
| | | Compiler overview | | [video](https://youtu.be/3mQ5tgiq1BM) |
| 3:00 PM | 3:30 PM | *Coffee break* | | |
| | | *Interactive Activity:* Compiling ResNet50, changing tiling, loop order, on-chip buffers, fusing layers | | |
| | | *Interactive Activity:* Compiling BERT | | | 
| | | Adding a new layer | | [video](https://youtu.be/zTAlpBVifVM) |
| | | Compiling to a new target architecture | | " |
| **4:00 PM** | **4:30 PM** | **Runtime and Drivers** | Hanyang | [slides](https://drive.google.com/file/d/1Tc3jDQUbMBjJZesZvIcJi_C9XLjTPJIR/view?usp=sharing) |
| | | Overview | | |
| | | APIs | | |
| | | OpenCL runtime | | |
| | | Example use cases | | |
| **4:30 PM** | **5:00 PM** | **Performance Profiling on _GeneSys_** | Hanyang | [slides](https://drive.google.com/file/d/1oy48z4ujWjmKxZUqDCITaBrHKVBUpoFy/view?usp=sharing) |
| | | *Interactive Activity:* Running BERT transformer block with different tiling, loop order, on-chip buffers, fusing layers | | |
| | | *Interactive Activity:* Analyzing logs | | |
| | | *Interactive Activity:* Using performance counters to investigate layer | | |

<!-- OLD BULLET-LIST SCHEDULE -->
<!-- - **Introduction** ([slides](https://drive.google.com/file/d/1E8Nxq5RPDpJ-WdlaAwh6_UkjYBydnXuk/view?usp=sharing))
  - DNNs, LLMs, and Hardware Acceleration
  - Need for an Open Source Toolchain
  - _GeneSys_ Overview
    - Compiler, Runtime, and Parameterizable Accelerator
    - Simulator, FPGA Implementation, and ASIC Tapeout
  - Potential Use Cases
    - Datacenters
    - Edge
    - Brain-Implantable Devices
- **_GeneSys_ Architecture** ([slides](https://drive.google.com/file/d/1HPd8SXfWXGB0kghUW_ZJxC5kvaqaShP8/view?usp=sharing))
  - Architecture Overview
    - Systolic Array
    - SIMD Array
    - On-Chip Memory Archiecture and Memery Interface
      - Programmable AXI Interface Implementation
   - Performance Counters
   - High-level Workflow and Software Pipelining
   - Configurable Parameters
   - *Interactive Activity* - Configuring _GeneSys_
   - Simulator Overview
   - FPGA Implementation and Synthesis
   - *Interactive Activity* - Run a layer with two different configurations using Vivado infrastructure
- **_GeneSys_ Architecture Hardware Verification, Configuration, and Implementation** ([slides](https://drive.google.com/file/d/1xCwBLS6qwOU3qSmTj65pPdOrC9lPvhEE/view?usp=sharing))
  - Verification Infrastructure
  - FPGA Implementation and ASIC Synthesis
  - Running _GeneSys_ on FPGA
  - *Interactive Activity* - 4x4 emulation on AWS
  - *Interactive Activity* - 16x16 emulation on AWS
- **Codelet Compiler and Programming Model** ([slides](https://drive.google.com/file/d/1HM5_2ne8TZROW2Uq0JsTb31fPGdWd85b/view?usp=sharing))
  - Programming Stack and Compilation
  - Compiler Overview
    - Input: ONNX Model
    - Input: Architecture Covenant Graph
    - Input: Codelets
    - Codelet Instantiation
    - Codelet Optimization
    - Code Generation
    - Output: Accelerator Binaries
  - *Interactive Activity* - Compiling ResNet50 with various tiling configurations, loop orders, on-chip buffer use, and layer fusion 
  - *Interactive Activity* - Compiling BERT
  - Adding a New Layer
  - Compiling to a New Target Architecture
- **Runtime and Drivers** ([slides](https://drive.google.com/file/d/1Tc3jDQUbMBjJZesZvIcJi_C9XLjTPJIR/view?usp=sharing))
  - Overview
  - APIs
  - OpenCL Runtime
  - Example Use Cases
- **Performance Profiling on _GeneSys_** ([slides](https://drive.google.com/file/d/1oy48z4ujWjmKxZUqDCITaBrHKVBUpoFy/view?usp=sharing))
  - *Interactive Activity* - Running a transformer block from BERT with various tiling configurations, loop orders, on-chip buffer use, and layer fusion
  - *Interactive Activity* - Analyzing the logs
  - *Interactive Activity* - Using performance counters to investigate layer performance
- **On-going development and Concluding Remarks** -->

# Presenters
- **Hadi Esmaeilzadeh**: Halicioğlu Chair in computer architecture and professor at the University of California, San Diego
- **Rohan Mahapatra**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Hanyang Xu**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Lavanya Karthikeyan**: Lead Design Engineering at Cadence Design Systems
- **Christopher Priebe**: Ph.D. student in computer science and engineering at the University of California, San Diego
