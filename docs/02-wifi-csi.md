# Wi-Fi CSI, Multipath Propagation, and Human Motion Sensing

## 1. Introduction

Wi-Fi sensing investigates how wireless channel measurements change when people or objects move within a radio environment.

Unlike conventional Wi-Fi communication, where the objective is reliable data transmission, wireless sensing uses information contained in the channel response to investigate environmental changes.

WiMoCSI studies these changes using physics-based simulation and controlled commodity Wi-Fi measurements.

## 2. Channel State Information

Channel state information (CSI) describes aspects of the wireless propagation channel between transmitting and receiving antennas.

In OFDM systems, the channel can be represented across multiple frequency subcarriers.

For subcarrier k at measurement time t, a simplified received-signal model is:

Y(k,t) = H(k,t)X(k,t) + N(k,t)

where:

- X(k,t) is the transmitted signal.
- Y(k,t) is the received signal.
- H(k,t) is the frequency-domain channel response.
- N(k,t) represents measurement noise and interference.

CSI estimates provide information about channel amplitude and phase across subcarriers and time.

Practical CSI measurements may also contain hardware-dependent and acquisition-dependent distortions.

## 3. Indoor Multipath Propagation

Indoor wireless propagation involves multiple paths created by reflection, scattering, diffraction, and other propagation mechanisms.

A conceptual frequency-domain channel model is:

H(f,t) = sum_p a_p(t) exp(-j 2 pi f tau_p(t))

where:

- p identifies a propagation contribution.
- a_p(t) represents its complex amplitude.
- tau_p(t) is its propagation delay.
- f is the radio frequency.

This is a simplified model used to explain multipath behavior. It is not a specification of WiMoCSI's private implementation.

The received channel is formed by the superposition of propagation contributions, which can interfere constructively or destructively.

## 4. How Human Movement Changes CSI

When a person moves through a wireless environment, their body can influence the propagation channel.

Movement may alter:

- Propagation path lengths
- Reflection and scattering contributions
- Relative phases of multipath components
- Received amplitude patterns
- Temporal characteristics of the measured channel

These variations may provide information about human motion.

However, different movements and geometries can generate similar channel observations.

Therefore, human motion cannot generally be inferred uniquely from arbitrary CSI measurements.

## 5. Motion Detection Versus Mobility Measurement

Motion detection asks whether the observed channel contains evidence of movement.

Mobility measurement attempts to estimate a physical quantity associated with that movement.

Examples include walking speed, displacement, or movement periodicity.

These are different inference problems.

A channel may exhibit movement-related variation without providing sufficient information for accurate walking-speed estimation.

WiMoCSI investigates these distinctions using controlled experiments and physical modeling.

## 6. Physics-Based Simulation

Physics-based wireless simulation can help researchers isolate the effects of geometry, propagation, antenna configuration, and prescribed human motion.

WiMoCSI uses Sionna RT as part of its research simulation environment.

Simulation provides controlled reference conditions but cannot automatically be assumed to reproduce every characteristic of real commodity Wi-Fi hardware.

Comparisons between simulation and measurement must therefore account for model assumptions and implementation differences.

## 7. Commodity Wi-Fi Measurements

Real CSI measurements depend on the properties of the wireless hardware and acquisition system.

Potential sources of variability include:

- Antenna configuration
- Frequency and bandwidth
- Sampling and packet timing
- Packet loss
- Clock and phase instability
- Noise and interference
- Device-specific signal processing
- Environmental changes

WiMoCSI investigates selected aspects of these effects using controlled measurements, including Intel AX201-based experiments.

## 8. Observability and Recoverability

A central sensing question is whether a physical movement parameter can be determined from the available channel observations.

Observability concerns whether the measurements contain information that distinguishes different physical states or parameters.

Recoverability also depends on numerical conditioning, measurement uncertainty, model mismatch, and the estimator being used.

These concepts help explain why a visible signal variation does not necessarily yield a reliable physical measurement.

## 9. Reliability and Uncertainty

Reliable mobility sensing requires more than a numerical estimate.

A responsible measurement process should consider:

- Independent reference measurements
- Experimental conditions
- Measurement uncertainty
- Numerical stability
- Validation across conditions
- Failure modes
- Conditions requiring rejection or abstention

WiMoCSI investigates these questions as part of its research into evidence-aware wireless mobility measurements.

## 10. Research Scope and Limitations

WiMoCSI has demonstrated selected motion-sensing and walking-speed estimation results under controlled conditions.

Generalization across environments, walking conditions, and acquisition settings remains under investigation.

The platform has not established clinical performance for fall detection, vital-sign monitoring, or emergency response.

## References

1. Ma, Y., Zhou, G., and Wang, S. (2019). WiFi sensing with channel state information: A survey. *ACM Computing Surveys*. https://doi.org/10.1145/3310194

2. Hoydis, J., et al. (2023). Sionna RT: Differentiable ray tracing for radio propagation modeling. *IEEE GLOBECOM Workshops*. https://arxiv.org/abs/2303.11103

These references provide general technical background on CSI-based sensing and physics-based radio propagation. They do not document WiMoCSI's unpublished implementation.