# WiMoCSI Research Platform

## 1. Overview

WiMoCSI is a physics-based research platform for investigating human movement sensing through Wi-Fi channel state information (CSI).

The platform combines controlled wireless propagation simulation, commodity Wi-Fi experiments, and quantitative evaluation.

Its central objective is to determine under what conditions Wi-Fi CSI can support reliable measurements of human movement.

WiMoCSI is an active research platform, not a validated clinical monitoring system.

## 2. Two Complementary Research Approaches

WiMoCSI investigates mobility sensing using two complementary approaches.

### A. Physics-Based Virtual Laboratory

The virtual laboratory uses Sionna RT to investigate wireless propagation under controlled simulation conditions.

Researchers can examine how prescribed movement and the radio environment influence the resulting channel response.

The simulation environment supports studies of:

- Indoor propagation geometry
- Transmitter and receiver configurations
- Human movement and scattering
- Multipath contributions
- Frequency-dependent channel behavior
- Sensitivity to modeling assumptions

Simulation provides access to prescribed movement and propagation conditions that can serve as experimental references.

However, simulated channel measurements are not automatically equivalent to CSI acquired from commodity Wi-Fi hardware.

### B. Commodity Wi-Fi Experiments

WiMoCSI also investigates movement using CSI recorded from commodity Wi-Fi equipment, including Intel AX201-based experiments.

Controlled walking measurements allow the researchers to compare wireless observations against independently obtained motion references.

These measurements help investigate:

- Movement-related CSI variation
- Walking-speed estimation
- Acquisition variability
- Hardware-dependent measurement effects
- Differences between simulation and experiment

Experimental observations provide evidence about performance under the conditions actually tested.

They do not automatically establish reliability in other environments or populations.

## 3. Conceptual Research Workflow

The platform follows a general research workflow:

1. Define a physical movement experiment.
2. Obtain simulated or measured wireless channel observations.
3. Examine movement-related CSI variation.
4. Evaluate candidate mobility measurements.
5. Compare results against independent reference information.
6. Assess uncertainty, failure conditions, and limitations.
7. Document reproducible scientific evidence.

This workflow is conceptual and does not describe the private estimator implementation.

## 4. Motion Detection

Motion detection investigates whether observed channel changes provide evidence of human movement.

WiMoCSI has investigated human motion detection in controlled experiments.

Motion detection is distinct from physical parameter estimation and does not by itself establish walking speed, direction, or location.

## 5. Walking-Speed Estimation

Walking-speed estimation aims to infer a physical movement quantity from wireless observations.

WiMoCSI investigates how CSI-based estimates compare with independently obtained walking references.

Experimental findings demonstrate that selected controlled conditions can support useful estimates.

However, performance depends on factors such as propagation geometry, acquisition conditions, motion patterns, and estimator assumptions.

Generalization remains an active research challenge.

## 6. Reliability-Oriented Research

A central feature of WiMoCSI is its attention to the reliability of wireless mobility measurements.

The research investigates questions involving:

- Physical observability
- Numerical recoverability
- Sensitivity to propagation geometry
- Measurement uncertainty
- Acquisition timing
- Packet loss and irregular sampling
- Model mismatch
- Estimator generalization
- Failure detection and abstention

These topics are relevant to determining when wireless observations support a defensible physical measurement.

## 7. Relationship Between Simulation and Real Measurements

Simulation and real measurement provide different forms of evidence.

Simulation enables controlled investigation of physical assumptions and prescribed motion.

Real experiments provide observations influenced by actual hardware, acquisition procedures, and environmental conditions.

Agreement between simulation and experiment may support a model under specified conditions.

Disagreement can reveal missing physical effects, measurement-model limitations, or estimator weaknesses.

WiMoCSI uses this distinction to guide research and validation.

## 8. Current Capabilities and Limitations

Current research capabilities include:

- Physics-based Wi-Fi propagation simulation
- Controlled CSI acquisition and analysis
- Investigation of human motion detection
- Investigation of walking-speed estimation
- Quantitative examination of selected reliability and uncertainty questions

Important limitations include:

- Generalization across environments and walking conditions is unresolved.
- Simulation does not reproduce all commodity hardware effects.
- Walking-speed estimates are not reliable under every tested condition.
- Fall detection and vital-sign monitoring are not validated capabilities.
- Clinical monitoring and emergency-response performance have not been established.

## 9. Future Research Directions

Longer-term investigations may include:

- Improved robustness across environments
- Wider validation of walking-speed estimation
- Longitudinal mobility measurement
- Fall detection research
- Breathing-rate and heart-rate sensing
- Healthy-aging and neurological health applications

These are research objectives rather than current validated product features.

## 10. Public Documentation and Code Availability

This repository provides public scientific documentation and approved research materials.

Detailed research implementation, unpublished algorithms, experimental datasets, and selected configurations remain in private research repositories.

Future releases may include independently reviewed educational examples or publication-specific research artifacts, subject to appropriate approvals.