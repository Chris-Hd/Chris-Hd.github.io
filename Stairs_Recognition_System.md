# Stairs Recognition System  
**Final Year Project – Electrical & Electronics Engineering**

## Overview  
This project focuses on helping people safely navigate stairs by detecting whether a staircase is going up or down and identifying the final step. The system is designed to assist people who have difficulty recognizing the end of stairs, including visually impaired users, and to support devices that need to move safely on staircases.

## Problem  
Many people struggle to detect when stairs end, which can cause accidents. This is especially dangerous for:
- Visually impaired individuals  
- Elderly people  
- Smart devices or robots that move on stairs  

The goal was to build a system that:
- Identifies upstairs vs. downstairs  
- Detects the last step  
- Works in real environments  

## My Role  
This was a solo project. I handled the entire process:
- System design  
- Hardware integration  
- Dataset creation  
- Model training  
- Software development  
- FPGA programming  
- Debugging and testing  

## Technologies Used  

### Hardware
- Raspberry Pi 4  
- Altera Cyclone V FPGA  
- Camera module  
- Laptop (GPU used for training)  

### Software & Platforms
- TensorFlow  
- PyScripter (Python IDE)  
- Intel Quartus  
- Linux (on Raspberry Pi)  

### Programming Languages
- Python  
- VHDL  

## System Description  
The system uses a camera to capture images of stairs. A deep learning model processes the images to:
- Identify if the stairs are going up or down  
- Detect the last step  

The Raspberry Pi runs the trained model, while the FPGA handles filtering and hardware-level processing. Communication between the Raspberry Pi and FPGA is handled through custom logic.

## What Worked Well  
- The system could detect stairs most of the time  
- It worked on real staircases, not just in lab conditions  
- It could distinguish between upstairs and downstairs  
- It could detect the last step some of the time  

## Challenges  
- The original plan was to run the deep learning model on the FPGA, but due to time limits this was not completed. Instead, the model ran on the Raspberry Pi and a filter was implemented on the FPGA.  
- Training required a large labeled dataset. One of the project goals was to create my own dataset, which took a lot of time and limited how much data I could use.  
- Communication between the Raspberry Pi and FPGA had a bug where some bits were shifted in time. I debugged the VHDL code and fixed the timing issue.  

## What I Learned  
- End-to-end system development: from idea to working device  
- Hardware–software integration  
- FPGA debugging and timing analysis  
- Deep learning model training and dataset creation  
- Problem-solving under time constraints  
