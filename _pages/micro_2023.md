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
- **Introduction** ([slides](https://drive.google.com/file/d/1E8Nxq5RPDpJ-WdlaAwh6_UkjYBydnXuk/view?usp=sharing))
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
- **On-going development and Concluding Remarks**

# Presenters
- **Hadi Esmaeilzadeh**: Halicioğlu Chair in computer architecture and professor at the University of California, San Diego
- **Rohan Mahapatra**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Hanyang Xu**: Ph.D. student in computer science and engineering at the University of California, San Diego
- **Lavanya Karthikeyan**: Lead Design Engineering at Cadence Design Systems
- **Christopher Priebe**: Ph.D. student in computer science and engineering at the University of California, San Diego
