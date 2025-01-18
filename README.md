![Chipnuts Logo](chipnuts_logo_placeholder.png)
# Welcome to chiplets !!

here we provide great IC and tech content for squirrels ;) 

# Computer Vision Research & Design Competition


## Overview
This competition invites researchers and professionals to create a comprehensive system design for a computer vision application. The aim is to develop a design that meets the application requirements, with clear justifications and a structured breakdown, enabling fresh graduates to implement and test the system. This competition emphasizes practical, real-world computer vision solutions that are feasible for implementation in hardware, software, and firmware domains.

Participants will be expected to:
1. Conduct research and create a design fulfilling the specified application requirements.
2. Provide a strong justification for why their proposed design meets these requirements.
3. Break down the high-level system design into actionable tasks suitable for fresh graduates from software, hardware, and firmware branches.
4. Develop a comprehensive testing and validation plan that competing students can follow for their RTL testbenches and software validation.
5. Design a complete software stack required to execute an end-to-end workload on the target ASIC, enabling the translation of high-level models from frameworks like PyTorch and TensorFlow into instructions compatible with the programming interface exposed by the ASIC.

## Target Application:
Computer vision applications are varied and include essential tasks such as **object detection**, **image segmentation**, **motion tracking**, **scene reconstruction**, and **anomaly detection**, among others. Each of these applications requires specific neural network operations that demand high processing efficiency and low latency to be effective in real-time. Therefore, an ASIC chip designed for computer vision must support a diverse set of operations that enable these applications to run smoothly and accurately. The chip must also demonstrate its capability by performing competitively on the **[MLPerf Inference Benchmark](https://arxiv.org/pdf/1911.02549)**.

The foundational operations that need hardware acceleration on such a chip include **convolutions** and **depthwise separable convolutions**, as they are critical for feature extraction in Convolutional Neural Networks (CNNs). This support is essential, given that convolutions are computation-intensive but crucial for detecting patterns, edges, and textures across applications like object detection and face recognition. Additionally, **attention mechanisms** found in **Vision Transformers** [[1]](https://arxiv.org/abs/2010.11929) (ViTs) are increasingly used in state-of-the-art models, as they improve performance on complex recognition and classification tasks by allowing the model to focus on important image regions. These mechanisms rely on efficient matrix multiplication and memory management, both of which should be optimized on the chip.

To handle common neural network architectures, the ASIC should also support batch normalization and activation functions (such as ReLU, Swish, and GELU) to enable fast, smooth training and inference cycles. Pooling layers and residual connections are also necessary, as they facilitate hierarchical feature extraction and allow for deeper networks, which are common in advanced applications. Moreover, many computer vision applications, such as real-time object detection and semantic segmentation, also require the chip to handle **upsampling** and **downsampling** operations, which allow the network to focus on different spatial resolutions.
The ultimate goal is to Domenstorate that the design asic chip can compete on Vision tasks on MLPerf Inference Benchmark


Since many computer vision applications are deployed in resource-constrained environments, the chip must also support quantization and mixed-precision arithmetic. These techniques reduce the model size and enhance power efficiency, which is particularly advantageous for edge applications like autonomous vehicles and surveillance systems. By incorporating these capabilities, the ASIC can deliver high performance, and energy efficiency, ensuring it meets the diverse needs of modern computer vision tasks across a wide range of devices and platforms.
## Objectives
1. **Application-Focused Design**: Create a research-backed design for a computer vision application that addresses specified application requirements.
2. **Justification**: Provide a well-supported explanation for how and why this design meets the requirements.
3. **Educational Task Breakdown**: Break down the design into structured tasks that fresh graduates in software, hardware, and firmware can understand and implement.
4. **Testing and Validation Plan**: Develop a robust testing and validation plan to guide implementation and ensure quality.
5. **Compelte Software Stack Specs**

## Contest Submission Guidelines

The final expected deliverable for the contest is a document composed of 3 main sections which are:

### 1. Research & Design Proposal
- **Research**: Participants are expected to conduct in-depth research on state of the art SoC design targeting computer vision. They are allowed to choose an already existing designs that meet the requirements. In addition, they have their space for innovation and creativity to build upon the state of the art. In the latter case, a justification based on thorough analysis is further required; this effort is taken into consideration when evaluating a contest entry. Accordingly, the first section should provide a brief literature review of chip architecting efforts that have been made.
- **Design Proposal**: The next subsection represents a conclusion on the previous subsection. It can either select one of the previous papers as a candidate paper for the participant's proposal or it can be an innovation of the participants where they can modify the design to yield better figure of merits for the design.
- **Justification**: The final subsection of the first section is the justification for slecting the candidate paper and/or the innovative modifications introduced by the participant. It has to be based on an elaborate comparison between the references used by the participants.

### 2. System Breakdown
- **Task Breakdown**: Decompose the design into manageable tasks, providing clarity and direction for fresh graduates in software, hardware, and firmware.
- **Documentation**: Create detailed documentation of the tasks, including diagrams, explanations, and expected outcomes.

### 3. Testing & Validation
- **Testing Plan**: Outline a comprehensive testing plan that specifies testing protocols for different components.
- **Validation Plan**: Define validation criteria and methods to ensure that the design meets application requirements.
- **Implementation Guidelines**: Provide guidelines for RTL testbench development and software tests, enabling fresh graduates to verify their implementations against specified benchmarks.
### 4. Software Stack
- **Spported Frameworks**: Models from Popular Frameworks such as (TensorFlow, PyTorch) should be supported allowing for seamless compilation and deployment on specialized hardware.
- **Graph and Operator Optimizer**: The graph optimizer performs general optimizations like operator fusion and partial evaluation, with extensions for workload-specific improvements such as quantization, data layout transformations, and maximizing data reuse. The operator optimizer automates workload scheduling, optimizing computation tiling, parallelism, and operator partitioning to maximize hardware efficiency.
- **JIT Compiler and Runtime**: Enables cooperative execution of deep learning workloads between a CPU host and the accelerator.

## Judging Criteria
- **Application Relevance**: How effectively the design addresses the specified computer vision application requirements.
- **Justification Quality**: The depth and clarity of the justification provided for the design.
- **Clarity of Breakdown**: The clarity and accessibility of the task breakdown for fresh graduates.
- **Testing & Validation Rigor**: The robustness and clarity of the testing and validation plan.

## Submission Guidelines
- **Format**: All submissions must be in Markdown format with supporting diagrams as PNG or SVG.
- **Repository**: Participants should submit their work through GitHub by creating a pull request in the competition repository.
- **Deadline**: [Insert Deadline Date]

## Prize & Recognition
The winning design will receive [insert prize details] and will be highlighted on our GitHub repository. Participants may also gain opportunities for collaboration on further development and implementation.

## Contact
<form action="https://formsubmit.co/assale02@protonmail.com" method="POST" enctype="multipart/form-data" style="max-width: 800px; margin: 0 auto; padding: 20px; border: 1px solid #ddd; border-radius: 8px; background-color: #f9f9f9;">
    <input type="hidden" name="_captcha" value="false">
    <!-- Team Information -->
    <fieldset style="border: 1px solid #ccc; padding: 15px; margin-bottom: 20px;">
        <legend style="font-size: 1.2em; font-weight: bold; margin-bottom: 10px;">Team Information</legend>
        <label for="team-name" style="display: block; margin-bottom: 5px;">Team Name:</label>
        <input type="text" id="team-name" name="team-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
        <label for="team-leader-name" style="display: block; margin-bottom: 5px;">Team Leader's Full Name:</label>
        <input type="text" id="team-leader-name" name="team-leader-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
        <label for="email" style="display: block; margin-bottom: 5px;">Team Leader's Email Address:</label>
        <input type="email" id="email" name="email" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
        <label for="affiliation" style="display: block; margin-bottom: 5px;">Team Leader's Affiliation (Organization/University):</label>
        <input type="text" id="affiliation" name="affiliation" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
        <label for="leader-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
        <input type="file" id="leader-cv" name="Leader CV" accept=".pdf"  style="padding: 8px; margin-bottom: 10px;"><br>
    </fieldset>
    <!-- Team Members -->
    <fieldset style="border: 1px solid #ccc; padding: 15px; margin-bottom: 20px;">
        <legend style="font-size: 1.2em; font-weight: bold; margin-bottom: 10px;">Team Members</legend>
        <!-- Repeat for each team member -->
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 2</h3>
            <label for="member-1-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-1-name" name="member-1-name"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-1-specialization" name="member-1-specialization"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-1-cv" name="member-1-cv" accept=".pdf"  style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 3</h3>
            <label for="member-2-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-2-name" name="member-2-name"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-2-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-2-specialization" name="member-2-specialization"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-2-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-2-cv" name="member-2-cv" accept=".pdf"  style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 4</h3>
            <label for="member-3-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-3-name" name="member-3-name"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-3-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-3-specialization" name="member-3-specialization"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-3-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-3-cv" name="member-3-cv" accept=".pdf"  style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 5</h3>
            <label for="member-4-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-4-name" name="member-4-name"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-4-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-4-specialization" name="member-4-specialization"  style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-4-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-4-cv" name="member-4-cv" accept=".pdf"  style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <!-- Repeat similar blocks for Team Members 2-5 -->
    </fieldset>
    <!-- Additional Info -->
    <fieldset style="border: 1px solid #ccc; padding: 15px; margin-bottom: 20px;">
        <legend style="font-size: 1.2em; font-weight: bold; margin-bottom: 10px;">Additional Information</legend>
        <label for="desired-application" style="display: block; margin-bottom: 5px;">Target Application (e.g., Computer Vision, NLP):</label>
        <select id="desired-application" name="desired-application" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;">
            <option value="Computer Vision">Computer Vision</option>
        </select><br>
        <label style="display: inline-flex; align-items: center; margin-bottom: 10px;">
            <input type="checkbox" name="terms" required style="margin-right: 8px;">
            I agree to the terms and conditions.
        </label><br>
    </fieldset>
    <!-- Submit Button -->
    <button type="submit" style="background-color: #4CAF50; color: white; padding: 12px 24px; border: none; border-radius: 4px; cursor: pointer;">
        Submit Your Entry
    </button>
</form>
---

**Join us in shaping the future of computer vision technology!**
