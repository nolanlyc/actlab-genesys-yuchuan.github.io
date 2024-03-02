---
layout: page
permalink: /compiler/
title: compiler
description: 
nav: true
nav_order: 3
---

The compiler for _GeneSys_ starts with an ONNX description of a neural network and generates an intermediate representation (IR) in the form of a fractalized dataflow graph (f-DFG).
The f-DFG is a dataflow graph where each vertex contains a sub-f-DFG representing the operation as a series of sub-operations of finer granularities.
This enables flexible compilation to different architectures by providing the compiler with access to many granularities of computation, a necessary feature given the diverse ecosystem of DNN accelerators.
Once generated from an ONNX file, the f-DFG is mapped to a series of parameterized operation kernels called codelets.
The operation kernels are then transformed and optimized by applying an architecture description (Architecture Covenant Graph) to the compilation process, which constrains kernel parameters based on hardware attributes such as memory size, bandwidth, and operation capabilities.
Once the kernel parameters are evaluated, each statement in the kernel is used to generate sequences of instructions defined by the Architecture Covenant Graph.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/genesys_compiler_flow.jpg" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    An overview of the GeneSys compilation workflow. 
</div>
