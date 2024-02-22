---
layout: page
title: DSCS Serverless
description: 
img: assets/img/dscs_serverless_intro.jpg
importance: 1
category: architecture
related_publications: dscs-serverless:asplos:2024
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/dscs_serverless_intro.jpg" title="DSCS Serverless Advancements" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This project devises DSCS-Serverless at the conjunction of three different trends in datacenters: (1) serverless computing in the programming level; (2) storage disaggregation in the system infrastructure level; and (3) domain-specific accelerators in the hardware level.
</div>

# Problem
In serverless computing, the need to store and retrieve results from remote storage in a disaggregated datacenter creates significant overhead due to network access. 
This overhead diminishes the potential acceleration benefits of serverless architecture.

# Insight
The overhead of moving data from remote storage limits the benefits from acceleration for serverless functions in disaggregated datacenters.

# Key Contributions
The *DSCS-Serverless* execution model that leverages a relatively small programmable accelerator within the storage device to accelerate a domain of serverless functions.
A software stack that seamlessly integrates in-storage accelerator with existing serverless models, handling storage-specific challenges such as data placement, scalability, and utilization, along with serverless considerations such as function placement, scalability, and cold starts.

# Abstract
While (I) serverless computing is emerging as a popular form of cloud execution, datacenters are going through major changes: (II) storage dissaggregation in the system infrastructure level and (III) integration of domain-specific accelerators in the hardware level. 
Each of these three trends individually provide significant benefits; however, when combined the benefits diminish. 
On the convergence of these trends, the project makes the observation that for serverless functions, the overhead of accessing dissaggregated storage overshadows the gains from accelerators. 
Therefore, to benefit from all these trends in conjunction, we propose In-Storage Domain-Specific Acceleration for Serverless Computing (dubbed *DSCS-Serverless*). 
The idea contributes a serverless model that utilizes a programmable accelerator embedded within computational storage to unlock the potential of acceleration in disaggregated datacenters. 
Our results with eight applications show that integrating a comparatively small accelerator within the storage (*DSCS-Serverless*) that fits within the storage’s power constraints (25 Watts), significantly outperforms a traditional disaggregated system that utilizes NVIDIA RTX 2080 Ti GPU (250 Watts). 
Further, the work highlights that disaggregation, serverless model, and the limited power budget for computation in storage device require a different design than the conventional practices of integrating microprocessors and FPGAs. 
This insight is in contrast with current practices of designing computational storage devices that are yet to address the challenges associated with the shifts in datacenters. 
In comparison with two such conventional designs that use ARM cores or a Xilinx FPGA, *DSCS-Serverless* provides 3.7x and 1.7x end-to-end application speedup, 4.3x and 1.9x energy reduction, and 3.2x and 2.3x better cost efficiency, respectively.
