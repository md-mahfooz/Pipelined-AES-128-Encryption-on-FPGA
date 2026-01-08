# Pipelined AES-128 Encryption on FPGA

This repository presents an implementation of the **AES-128 encryption algorithm using a pipelined hardware architecture**, designed for efficient deployment on FPGA platforms.

The design focuses on improving throughput by overlapping multiple AES rounds using pipelining, making it suitable for high-speed and resource-aware cryptographic applications.

---

## Overview

- Implements **AES-128 encryption** as defined by the Rijndael standard
- Uses a **fully pipelined architecture** to increase encryption throughput
- Designed using **hardware description language (HDL)** for FPGA deployment
- Suitable for studying performance trade-offs between latency, area, and throughput in cryptographic hardware

---

## Design Highlights

- Modular implementation of AES stages:
  - SubBytes
  - ShiftRows
  - MixColumns
  - AddRoundKey
- Pipeline registers inserted between rounds to enable concurrent processing of multiple data blocks
- Key expansion logic integrated into the encryption pipeline
- Parameterized and structured design for clarity and extensibility

---

## Evaluation

- Functional correctness verified through simulation
- Throughput and timing performance analyzed for FPGA execution
- Design emphasizes hardware efficiency while maintaining AES compliance

---

## Repository Structure

The repository contains:
- AES core modules
- Key expansion modules
- Testbench files for verification
- FPGA-related configuration files

---
