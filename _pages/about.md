---
layout: about
title: about
permalink: /
subtitle: 

profile:
  align: right
  image: genesys-logo.jpg
  image_circular: false # crops the image to make it circular
  more_info:

news: true  # includes a list of news items
latest_posts: false  # includes a list of the newest posts
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/genesys_workflow.jpg" class="img-fluid rounded z-depth-1" center=true %}
    </div>
</div>
<div class="caption">
    An overview of the GeneSys workflow.
</div>

_GeneSys_ is an innovative solution designed to seamlessly integrate accelerators into the software infrastructure, offering a holistic approach to system design. 
It is specifically engineered to produce complete acceleration systems for emerging deep learning models with minimal human intervention. 
_GeneSys_ marks a significant advancement in the realm of open-source deep learning hardware, presenting an all-in-one solution for the efficient generation of deep learning accelerators, complete with a cutting-edge compiler and user-friendly APIs.
Next, we briefly list the key features of _GeneSys_.

**Comprehensive Solution:** _GeneSys_ offers an end-to-end compilation stack, a parameterizable DNN accelerator generator, RTL verification testbenches and regression suite with synthetic and state-of-the-art DNN benchmarks (including transformers like BERT and GPT2), FPGA implementation framework, OpenCL-compliant Linux drivers, and a software simulator for quick profiling and insights.

**Multi-target Compilation Stack:** The Codelet compiler converts ONNX models into an intermediate representation (IR) and performs architecture specific optimizations for various configurations.
It further supports multiple backends, giving users flexibility in deploying tailored accelerators.

**Accelerator Architecture:** The GeneSys accelerator features a systolic array for operations such as GeMM and convolution, along with a closely coupled specialized SIMD unit for operations such as softmax, pooling, and activation.
It is highly parameterizable and synthesizable.

**Holistic Evaluation:** _GeneSys_ offers a holistic approach to evaluation, verification, and debugging for efficient design space exploration, encompassing hardware and compiler optimizations.

**ONNX Compatibility:** _GeneSys_ utilizes the Open Neural Network Exchange (ONNX) format to specify deep learning models, ensuring interoperability across various programming environments. It can compile Pytorch/Tensorflow-generated models into the accelerator.

**Minimal Python APIs:** _GeneSys_ provides minimal Python APIs for seamless integration into end-to-end applications, streamlining the development process.

**AWS F1 FPGA Compatibility:** _GeneSys_ is compatible with AWS F1 instances available in the public cloud, enabling users to run end-to-end deep neural networks on these FPGA instances, enhancing its versatility and accessibility.

<!-- OLD FRONT PAGE -->
<!-- _GeneSys_ is a programmable deep learning acceleration system generator.
The core computation engines in _GeneSys_ are a systolic array (for operations such as convolution) and SIMD engine (for operations such as ReLU and pooling). _GeneSys_ is parametrizable, and it is possible to automatically generate hardware with different numbers of processing elements, on-chip buffer configurations, and memory bandwidths.
The generated accelerator acts like a co-processor connected to the host via the PCIe bus.
The target workloads for the accelerator are computer vision and transformers-based models. -->
