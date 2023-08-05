# Simple 32-bit RISC Processor with Single Cycle and Pipeline Implementation

This GitHub repository contains the code and documentation for a simple 32-bit RISC processor with eight 32-bit general-purpose registers (R0 through R7). The processor architecture includes a program counter (PC), a special-purpose 20-bit register capable of addressing up to 2<sup>20</sup> (1,048,576) instructions. All instructions in this processor are 16 bits long and can be categorized into four formats: R-type, I-type, B-type, and J-type.

## Table of Contents

1. [Introduction](#introduction)
2. [Features](#features)
3. [Instruction Formats](#instruction-formats)
4. [Phases](#phases)
5. [Building the Processor](#building-the-processor)
    - [Single Cycle Processor](#single-cycle-processor)
    - [Pipeline Processor](#pipeline-processor)
6. [Getting Started](#getting-started)

## Introduction

This project aims to implement a simple 32-bit RISC processor that includes the essential features of a RISC architecture, such as a limited set of instructions, a few general-purpose registers, and a streamlined instruction pipeline for improved performance.

## Features

- 32-bit RISC processor
- Eight 32-bit general-purpose registers (R0 through R7)
- 20-bit program counter (PC)
- Support for up to 2<sup>20</sup>  (1,048,576) instructions
- Four instruction formats: R-type, I-type, B-type, and J-type
- Single cycle implementation
- Pipeline implementation

## Instruction Formats

1. R-Type:
    - Opcode (5 bits)
    - Source Register (RS) (3 bits)
    - Destination Register (RD) (3 bits)
    - Target Register (RT) (3 bits)
    - Function Code (Funct) (2 bits)

2. I-Type:
    - Opcode (5 bits)
    - Source Register (RS) (3 bits)
    - Destination Register (RD) (3 bits)
    - Immediate Value (IMM) (5 bits)

3. B-Type:
    - Opcode (5 bits)
    - Destination Register (RD) (3 bits)
    - Immediate Value (IMM) (8 bits)

4. J-Type:    
    - Opcode (5 bits)
    - Immediate Value (IMM) (11 bits)

## Phases

The project is divided into two main phases:

1. Building a Single Cycle Processor: In this phase, the processor is designed to execute instructions in a single clock cycle. Each instruction fetch, decode, execute, and write-back stages are completed within a single clock cycle.
    
2. Building a Pipeline Processor: The pipeline processor extends the single cycle implementation by dividing the instruction execution into multiple stages, allowing for higher instruction throughput. The key pipeline stages include instruction fetch (IF), instruction decode (ID), execution (EX), memory access (MEM), and write-back (WB).    

## Building the Processor

### Single Cycle Processor

The single cycle processor implementation can be found in the `single_cycle` directory. Follow the instructions provided in the `README.md` file within that directory to build and simulate the single cycle processor.

### Pipeline Processor

The pipeline processor implementation can be found in the `pipeline` directory. Refer to the `README.md` file within that directory for detailed instructions on building and simulating the pipeline processor.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository to your local machine.
2. Review the documentation to understand the processor's architecture and instruction set.
3. Choose which implementation (single cycle or pipeline) you want to work with.
4. Install the logisim software for simulating digital logic circuits.


---

Thank you for your interest in this simple 32-bit RISC processor project! If you have any questions or need further assistance, please don't hesitate to reach out.
