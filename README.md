# WiMoCSI

## Physics-Based Wi-Fi Sensing for Reliable Mobility Monitoring

WiMoCSI is a research platform originating from doctoral research at Portland State University. It investigates how commodity Wi-Fi channel state information (CSI) can support human motion detection and walking-speed measurement, with a long-term focus on healthy aging and privacy-conscious monitoring.

## Why WiMoCSI?

Changes in everyday mobility can provide important information for research into aging, falls, and cognitive health.

Wi-Fi sensing offers an opportunity to study human movement without cameras or body-worn sensors. However, reliable measurement requires understanding how wireless propagation, movement, hardware, and signal processing interact.

WiMoCSI investigates not only what movement can be measured using Wi-Fi CSI, but also when those measurements can be trusted.

## Research Approach

WiMoCSI combines two complementary approaches:

### Physics-Based Simulation

The platform uses Sionna RT to investigate human movement and indoor wireless propagation under controlled simulation conditions.

### Commodity Wi-Fi Experiments

Controlled experiments use commodity Wi-Fi CSI measurements, including Intel AX201 recordings, to investigate movement-related channel variations and walking-speed estimation against independent reference measurements.

## Research Areas

- Human motion detection
- Walking-speed estimation
- Physics-based wireless propagation modeling
- CSI measurement reliability
- Numerical recoverability and uncertainty
- Robustness to acquisition conditions
- Mobility monitoring for healthy aging

## Scientific Status

Human motion detection and walking-speed estimation have been demonstrated under selected controlled experimental conditions.

Reliable generalization across walking conditions, environments, and acquisition settings remains an active research challenge.

Fall detection, heart-rate monitoring, breathing-rate monitoring, and clinical applications are longer-term research directions. These capabilities have not been clinically validated through WiMoCSI.

## Documentation

Explore the WiMoCSI research documentation:

- [Research Motivation and Healthy Aging](docs/01-motivation.md)
- [Wi-Fi CSI and Human Motion Sensing](docs/02-wifi-csi.md)
- [Research Platform Architecture](docs/03-platform.md)
- [Measurement Reliability and Evidence-Aware Sensing](docs/04-reliability.md)
- [Research Roadmap](docs/05-roadmap.md)
- [Research Publications](publications/README.md)
## Publications

Research publications and approved scientific materials will be documented in the publications directory.

## Code and Data Availability

The underlying research implementation, selected configurations, and experimental datasets are not publicly released at this stage.

This public repository is intended for scientific documentation, approved research materials, and future educational resources.

## Research Context

WiMoCSI originated through doctoral research at Portland State University, informed by the broader scientific literature on mobility, aging, and longitudinal health monitoring.

## Disclaimer

WiMoCSI is an experimental research platform. It is not a medical device and is not intended for clinical diagnosis, emergency response, or patient monitoring.

## Project Links

- Research website: [wimocsi.com](https://wimocsi.com)
- Publications: See publications directory
- Technical documentation: See docs directory