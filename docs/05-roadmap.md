# WiMoCSI Research Roadmap

## Overview

WiMoCSI investigates whether commodity Wi-Fi CSI can support reliable human movement measurements for future mobility-monitoring applications.

The roadmap distinguishes demonstrated research capabilities, ongoing investigations, and longer-term objectives.

It does not represent a commercial product release schedule or a claim of clinical readiness.

## 1. Physics-Based Wireless Simulation

Status: Implemented research capability; validation ongoing.

WiMoCSI uses physics-based propagation simulation to investigate how human movement influences wireless channel observations.

Current research considers the effects of propagation geometry, multipath behavior, movement, and modeling assumptions.

Further validation is required to characterize agreement with real commodity Wi-Fi measurements across broader conditions.

## 2. Human Motion Detection

Status: Demonstrated under selected controlled experimental conditions.

WiMoCSI has investigated the detection of human movement through changes in Wi-Fi channel observations.

Future research will examine robustness across additional environments, movement patterns, and measurement configurations.

Motion detection is not equivalent to reliable walking-speed measurement or fall detection.

## 3. Walking-Speed Estimation

Status: Demonstrated under selected conditions; generalization unresolved.

Controlled experiments have investigated walking-speed estimation using commodity Wi-Fi CSI and independent motion references.

Results under selected experimental conditions support continued investigation.

However, recent evaluations have also identified limitations in estimator generalization.

A major research objective is to distinguish unavailable physical information from limitations introduced by the estimation procedure.

## 4. Simulation-to-Measurement Comparison

Status: Active research.

WiMoCSI investigates how physically simulated wireless channel behavior compares with real CSI measurements.

Research challenges include hardware effects, measurement-model assumptions, and environmental differences.

The objective is to develop better-supported relationships between simulation evidence and experimentally observed behavior.

## 5. Reliability and Measurement Uncertainty

Status: Active research.

Research directions include:

- Physical observability
- Numerical recoverability
- Acquisition timing and irregular sampling
- Packet loss and measurement perturbations
- Model mismatch
- Estimator generalization
- Uncertainty reporting
- Evidence-aware rejection and abstention

The long-term objective is to identify the conditions under which a physical mobility estimate is scientifically defensible.

## 6. Reproducibility and Scientific Reporting

Status: Ongoing.

WiMoCSI emphasizes documented experimental conditions, independent reference measurements, and explicit reporting of limitations.

Public scientific materials will be released following appropriate review.

The underlying research implementation and restricted experimental datasets are not currently public.

## 7. Longer-Term Research Directions

Potential future investigations include:

- Longitudinal mobility monitoring
- Fall detection
- Heart-rate and breathing-rate sensing
- Aging-in-place applications
- Senior living environments
- Mobility research related to Alzheimer's disease and related dementias

These objectives require additional technical and, where appropriate, clinical validation.

They are not established capabilities of the present research platform.

## 8. Scientific Development Principles

WiMoCSI development is guided by several principles:

1. Distinguish physical observability from estimator performance.
2. Compare wireless measurements with independent references.
3. Report both successful and unsuccessful evaluations.
4. Characterize uncertainty and operating conditions.
5. Avoid treating simulation as equivalent to hardware measurements.
6. Preserve reproducible research evidence.
7. Avoid clinical claims without appropriate validation.

## Roadmap Updates

This roadmap will be updated as research findings are validated, publications become available, and new experiments are completed.

Milestones do not imply that any particular clinical or commercial application has been established.