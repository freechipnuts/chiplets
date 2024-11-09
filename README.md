<p align="center">
  <img src="static/chipnuts_logo_1.svg" width="200" />
</p>

# Welcome to Chiplets!

Here, we provide great IC and tech content for squirrels 🐿️.

# Chiplets AI SoC Competition

## Overview
The **Chiplets AI SoC Competition** challenges researchers and professionals to design a comprehensive **AI System on Chip (SoC)** optimized for **computer vision applications**. The competition consists of four phases, beginning with **Requirements & Architecture Design**, followed by **Implementation and RTL Design**, **Verification and Validation**, and culminating in **Synthesis, Place & Route (P&R), and Tape-Out**.

In Phase I, participants are expected to define the application requirements themselves, developing a research-backed blueprint that aligns with real-world AI SoC needs in computer vision. The design should be feasible across hardware, software, and firmware domains and enable recent graduates to implement and test the system effectively.

### Considerations for Phase I Design

In Phase I, participants need to consider the following elements while designing their system:

- **Verilog and C-Model**: Include Verilog top module definitions with signals, interfaces, and a detailed C-model down to the protocol level.
- **Compiler, Linux Drivers, and Software Stack**: The solution should come with Linux drivers, test benches, kernel- and user-mode software, and C header files with corresponding C APIs for full integration.
- **Tools and Libraries**: Provide development tools and support for **OpenGL** where relevant, leveraging existing drivers where possible.

To guide the design, participants can explore resources such as:
- [Broadcom SoC Documentation](https://docs.broadcom.com/doc/12358545)
- [Mesa Panfrost Open Source GPU Driver](https://docs.mesa3d.org/drivers/panfrost.html)
- [NVIDIA Deep Learning Accelerator (NVDLA)](https://nvdla.org/hw/v1/hwarch.html)
- [VeriGPU GitHub Repository](https://github.com/hughperkins/VeriGPU)

Additionally, participants are encouraged to examine open-source implementations like AMD’s **Southern Islands ISA** for insights into GPU ISA and **Panfrost** for ARM Mali Midgard GPUs, which leverage a rich ARM software ecosystem.

## Phase I: Requirements
Participants are expected to:
1. **Define application requirements**: Conduct research and propose requirements that align with the demands of a computer vision-focused SoC.
2. **Justify the proposed requirements and design**: Present clear, research-backed reasoning for chosen requirements and how the design meets them.
3. **Break down the system architecture**: Provide a structured approach that fresh graduates in hardware, software, and firmware can follow.
4. **Develop a testing and validation plan**: Create a plan to ensure accuracy and robustness for both RTL and software validation.

## Objectives
1. **Application-Focused Design**: Define and design around a realistic computer vision application.
2. **Justification**: Present a rationale for the requirements and design decisions.
3. **Educational Task Breakdown**: Structure the design into tasks manageable for recent graduates.
4. **Testing and Validation**: Establish a framework for testing and validation.

## Contest Entry Requirements
Each submission should encompass:

### 1. Research & Design Proposal
- **Research**: Conduct comprehensive research on SoC design, focusing on computer vision and AI applications.
- **Design Proposal**: Outline the overall architecture, defining key components, interfaces, and roles.
- **Justification**: Present a clear justification for design choices and architecture, emphasizing compatibility and scalability.

### 2. System Breakdown
- **Task Decomposition**: Break down the design into actionable tasks for software, hardware, and firmware, with documentation including diagrams, explanations, and expected outcomes.
- **Documentation**: Provide detailed task documentation, complete with Verilog and C headers, facilitating understanding and implementation.

### 3. Testing & Validation
- **Testing Protocols**: Develop test protocols for each component, using protocol-level testbenches for RTL validation.
- **Validation Guidelines**: Set forth clear criteria for validation, ensuring the design meets application requirements and is suitable for deployment.

## Judging Criteria
- **Application Relevance**: How effectively the design addresses the participant-defined requirements.
- **Justification Quality**: The clarity and depth of the rationale for design decisions.
- **Task Clarity**: Accessibility of the task breakdown for fresh graduates.
- **Testing & Validation Rigor**: Robustness and clarity of the testing and validation framework.

## Submission Guidelines
- **Format**: Submissions must be in Markdown format, with supporting diagrams in PNG or SVG.
- **Repository**: Submit via GitHub by creating a pull request in the competition repository.
- **Deadline**: [Insert Deadline Date]

## Prize & Recognition
The winning design will receive [insert prize details] and may be featured on our GitHub repository. Additionally, winners may have opportunities to collaborate on further development and deployment.

## Contact

Please submit your team’s information using the form below:

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
    </fieldset>
    <!-- Team Members -->
    <fieldset style="border: 1px solid #ccc; padding: 15px; margin-bottom: 20px;">
        <legend style="font-size: 1.2em; font-weight: bold; margin-bottom: 10px;">Team Members</legend>
        <!-- Repeat for each team member -->
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 2</h3>
            <label for="member-1-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-1-name" name="member-1-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-1-specialization" name="member-1-specialization" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-1-cv" name="member-1-cv" accept=".pdf" required style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 3</h3>
            <label for="member-1-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-1-name" name="member-1-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-1-specialization" name="member-1-specialization" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-1-cv" name="member-1-cv" accept=".pdf" required style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 4</h3>
            <label for="member-1-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-1-name" name="member-1-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-1-specialization" name="member-1-specialization" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-1-cv" name="member-1-cv" accept=".pdf" required style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <div class="team-member" style="margin-bottom: 20px;">
            <h3 style="font-size: 1.1em; font-weight: bold;">Team Member 5</h3>
            <label for="member-1-name" style="display: block; margin-bottom: 5px;">Name:</label>
            <input type="text" id="member-1-name" name="member-1-name" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-specialization" style="display: block; margin-bottom: 5px;">Specialization:</label>
            <input type="text" id="member-1-specialization" name="member-1-specialization" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;"><br>
            <label for="member-1-cv" style="display: block; margin-bottom: 5px;">CV (PDF only):</label>
            <input type="file" id="member-1-cv" name="member-1-cv" accept=".pdf" required style="padding: 8px; margin-bottom: 10px;"><br>
        </div>
        <!-- Repeat similar blocks for Team Members 2-5 -->
    </fieldset>
    <!-- Additional Info -->
    <fieldset style="border: 1px solid #ccc; padding: 15px; margin-bottom: 20px;">
        <legend style="font-size: 1.2em; font-weight: bold; margin-bottom: 10px;">Additional Information</legend>
        <label for="desired-application" style="display: block; margin-bottom: 5px;">Target Application (e.g., Computer Vision, NLP):</label>
        <select id="desired-application" name="desired-application" required style="width: 100%; padding: 8px; margin-bottom: 10px; border: 1px solid #ccc; border-radius: 4px;">
            <option value="Computer Vision">Computer Vision</option>
            <option value="Natural Language Processing">Natural Language Processing</option>
            <option value="Speech Recognition">Speech Recognition</option>
            <option value="Robotics">Robotics</option>
            <option value="Other">Other</option>
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

**Join us in shaping the future of computer vision technology with cutting-edge AI SoC design!**

---
