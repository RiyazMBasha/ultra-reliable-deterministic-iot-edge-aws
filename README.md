# Ultra-Reliable, Deterministic IoT and AI-Driven Smart City Pipeline on AWS

## Overview
This repository contains the full implementation, experimental evaluation, and analysis
of a deterministic IoT edge–cloud pipeline deployed on AWS infrastructure.

The work evaluates three progressively advanced system configurations:
- Case 1: Baseline pipeline with no deterministic control
- Case 2: Static deterministic batching at the edge
- Case 3: AI-driven adaptive edge control

## Project Phases

This research is structured into progressive experimental phases:

**Phase 0 — Pipeline Validation**
- End-to-end device → edge → cloud communication
- MQTT-based telemetry flow verification
- Timestamp instrumentation across all layers

**Phase 1 — Baseline Measurement**
- Measurement of latency and jitter without determinism
- No batching, no adaptation, no intelligence
- Establishes a non-deterministic reference baseline

**Phase 2 — Static Deterministic Control**
- Fixed batching and flushing at the edge
- Reduction of latency variance under controlled conditions
- Demonstrates partial determinism

**Phase 3 — Adaptive Edge Intelligence**
- AI-inspired adaptive control at the edge
- Dynamic batching and flush decisions
- Balances latency, jitter, and throughput


## Key Contributions
- Real-world deployment on AWS (not simulation-based)
- End-to-end latency and jitter instrumentation across device, edge, and cloud
- Demonstration of adaptive deterministic behavior at the edge
- Comparative analysis of latency, jitter, and predictability across three cases

## Repository Structure
- `thesis/` — Thesis chapters and academic write-up
- `code/` — Device, edge, cloud, and analysis source code
- `results/` — Experimental outputs, summaries, and plots
- `diagrams/` — System architecture and pipeline diagrams
- `configs/` — AWS, MQTT, and environment setup instructions
- `scripts/` — Scripts to reproduce experimental cases

## How to Reproduce Experiments
Refer to `configs/aws_ec2_setup.md` for environment setup and  
use the scripts in `scripts/` to execute Case 1, Case 2, and Case 3.

## Author
Riyaz Basha Mandiyam (M.R.Basha)

## License
MIT License
