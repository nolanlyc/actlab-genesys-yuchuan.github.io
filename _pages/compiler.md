---
layout: page
permalink: /compiler/
title: compiler
description: 
nav: true
nav_order: 3
---

The compiler for GeneSys starts with an ONNX description of an ML algorithm and generates an intermediate representation (IR) in the form of a simultaneous-recursive dataflow graph (sr-DFG).
The sr-DFG is a recursively defined dataflow graph which enables simultaneous access to all levels of operation granularity for flexibly compiling to different architectures.
Once generated from an ONNX file, the sr-DFG is transformed to a series of parameterized operation kernels.
The operation kernels are then transformed and optimized by applying an architecture description to the compilation process, which constrains kernel parameters based on hardware attributes such as memory size, bandwidth, and operation capabilities.
Once the kernel parameters are evaluated, each statement in the kernel is used to generate sequences of instructions defined by the architecture abstraction.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/genesys_compiler_flow.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An overview of the GeneSys compilation workflow. 
</div>
