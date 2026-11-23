# Measurement Reliability and Evidence-Aware Wi-Fi Sensing

## 1. Why Reliability Matters

Human movement can change the wireless propagation channel.

However, observing channel variation does not automatically establish that a physical movement quantity can be measured accurately.

A useful mobility measurement requires evidence that the reported result is supported by the available observations and experimental conditions.

WiMoCSI investigates the physical and measurement-related limits of reliable Wi-Fi sensing.

## 2. Motion Detection and Physical Measurement

Motion detection and mobility estimation are distinct tasks.

Motion detection asks whether wireless observations provide evidence of movement.

Mobility estimation attempts to infer a physical quantity, such as walking speed.

A signal may contain sufficient evidence to detect movement without providing sufficient information for a reliable walking-speed estimate.

WiMoCSI studies this distinction using controlled simulation and experimental measurements.

## 3. Physical Observability

Observability concerns whether the measurements contain enough information to distinguish the physical quantities being investigated.

In wireless sensing, observability depends on factors such as propagation geometry, the measured channel, motion, and available measurement diversity.

Different physical movements may produce similar wireless observations.

This creates fundamental limitations that cannot necessarily be resolved by changing the estimator.

WiMoCSI investigates observability as an important component of trustworthy mobility sensing.

## 4. Numerical Recoverability

Even when a parameter is theoretically distinguishable, recovering it from finite and imperfect measurements may be difficult.

Numerical recoverability depends on factors including:

- Sensitivity to measurement perturbations
- Numerical conditioning
- Model mismatch
- Sampling characteristics
- Noise
- Estimator assumptions

A physically meaningful channel model does not guarantee a stable numerical estimate.

WiMoCSI therefore distinguishes physical information availability from practical estimation performance.

## 5. Simulation and Measurement Evidence

Physics-based simulation provides controlled conditions and prescribed motion references.

Real commodity Wi-Fi recordings include additional influences from hardware, acquisition procedures, and the physical environment.

Simulation and measurement should be evaluated as complementary sources of evidence rather than treated as interchangeable.

Differences between them may identify limitations in the propagation model, measurement model, or inference procedure.

## 6. Independent Reference Measurements

Reliable experimental evaluation requires reference information obtained independently of the wireless estimator.

For walking-speed experiments, independent timing or video-derived motion references can support quantitative comparisons.

Evaluation should report the experimental conditions and the definition of the physical quantity being estimated.

For example, estimating movement periodicity is not necessarily equivalent to estimating walking speed.

## 7. Acquisition Conditions

Commodity Wi-Fi CSI measurements may be influenced by:

- Packet loss
- Irregular sampling
- Timestamp uncertainty
- Phase instability
- Noise and interference
- Frequency and bandwidth selection
- Antenna configuration
- Device-dependent signal processing

These effects can influence both the available information and estimator performance.

WiMoCSI investigates selected acquisition-related limitations as part of its reliability research.

## 8. Generalization and Failure Modes

Performance obtained in one experimental configuration does not establish performance across different walking conditions or environments.

Estimator assumptions may hold under selected conditions and fail under others.

A scientifically useful evaluation should distinguish:

- Successful estimates under specified conditions
- Rejected or unavailable estimates
- Incorrect accepted estimates
- Conditions outside the evaluated operating range

WiMoCSI treats such failures as important research findings rather than excluding them from the scientific account.

## 9. Evidence-Aware Abstention

A sensing system should not always be required to output a numerical estimate.

When available evidence is insufficient, withholding an estimate may be more appropriate than reporting an unsupported value.

However, abstention does not itself demonstrate measurement accuracy.

Evaluation should consider both the reliability of accepted estimates and the proportion of measurements for which an estimate is produced.

WiMoCSI investigates these concepts in the context of wireless mobility sensing.

## 10. Current Research Status

WiMoCSI has investigated motion detection and walking-speed estimation under controlled conditions.

Selected experiments have demonstrated useful results, while other tests have exposed limitations in estimator generalization.

The research continues to examine the conditions under which physical movement information is observable and practically recoverable.

No claim of universal walking-speed accuracy, clinical reliability, or validated fall detection is made.

## 11. Research Direction

Future reliability investigations may include:

- Broader experimental validation
- Additional environments and movement patterns
- Improved measurement-model characterization
- Robustness to acquisition variability
- Better uncertainty reporting
- Independent testing of estimator generalization
- Clearer definitions of supported operating conditions

The objective is to develop scientifically defensible methods for assessing the reliability of Wi-Fi-based mobility measurements.

## Publication and Implementation Notes

This document describes general research questions and publicly established engineering principles.

It does not disclose unpublished WiMoCSI algorithms, mathematical proofs, estimator thresholds, proprietary implementations, or restricted experimental datasets.

Publication-specific methods and numerical findings will be made available only following appropriate review and authorization.