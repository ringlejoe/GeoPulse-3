# GeoPulse: Seismic Vibration Sensor

GeoPulse is an advanced seismic vibration sensing platform designed for real-time monitoring and analysis of geophysical signals. Built around the ESP32-S3 microcontroller, it integrates a built-in Li-Po battery charger, USB-C interface, and a 128x64 OLED display for on-device visualization. The device leverages WiFi socket communication for seamless integration with a dedicated desktop application, enabling remote control, signal monitoring, data analysis, and automated report generation. For extended range beyond WiFi capabilities, GeoPulse employs LoRa communication for reliable, long-distance data transmission. GeoPulse supports flexible deployment as a standalone unit or as part of an interconnected cluster communicating through a gateway, enabling scalable network configurations for large-area geophysical monitoring.

## Key Features
- **Core Hardware**: ESP32-S3 microcontroller with integrated WiFi for robust short-range connectivity and LoRa for long-range communication.
- **Power Management**: Built-in Li-Po battery charger and USB-C port for efficient recharging and data transfer.
- **Display**: 128x64 OLED screen for real-time feedback on sensor readings, device status, and network connectivity.
- **Connectivity**: 
  - Socket-based WiFi communication for high-speed integration with a desktop app within WiFi range.
  - LoRa communication for extended range beyond WiFi limits, ensuring reliable data transmission in challenging environments.
  - Cluster-based networking via a gateway for coordinated multi-device operations across large areas.
- **Application Integration**: Desktop software for signal control, real-time monitoring, advanced analysis (e.g., waveform processing, anomaly detection, spectral analysis), and customizable reporting with export options in formats such as PDF and CSV.
- **Deployment Flexibility**: Operates as a standalone device for localized monitoring or in a cluster configuration, interconnected with other GeoPulse units through a central gateway for synchronized data collection, aggregation, and analysis.

GeoPulse is engineered for applications in geophysics, environmental monitoring, structural health assessment, earthquake early warning systems, and industrial vibration analysis. It emphasizes modularity, low power consumption, and scalability to support deployment in diverse field conditions, from single-point sensing to distributed sensor networks in urban, rural, or remote environments.

## Roadmap and Variants
To expand the capabilities of GeoPulse, future iterations will introduce tiered models tailored to varying operational requirements, enhancing range, autonomy, precision, and sensor integration:

1. **GeoPulse Basic**: 
   - WiFi range up to 100m in open space, LoRa for extended connectivity.
   - 500mAh battery for portable, short-duration use.
   - 4GB internal storage for data logging.

2. **GeoPulse Standard**: 
   - WiFi range of 200-300m in open space, LoRa for extended connectivity.
   - 1000mAh battery for enhanced runtime.
   - GPS with <80cm accuracy for location-aware sensing.
   - 64GB storage for increased data capacity.

3. **GeoPulse Max**: 
   - Hybrid connectivity: WiFi up to ~350m, LoRa up to 1km, and RF for additional redundancy.
   - 3000mAh battery for prolonged field operations.
   - High-precision GPS (<2cm accuracy) for precise geolocation.
   - Integrated 128x64 OLED display for enhanced visualization.
   - Tri-axial accelerometer for multi-dimensional motion detection.
   - Temperature and humidity sensors for environmental context.
   - 256GB storage for extensive data logging.

4. **GeoPulse Max-Eco**: 
   - Extends GeoPulse Max with a solar panel for sustainable power harvesting.
   - Optimized for off-grid and remote deployments with minimal maintenance.

These variants maintain backward compatibility with the core ESP32-S3 architecture, desktop app, and cluster-gateway communication protocols (WiFi and LoRa), ensuring seamless upgrades and interoperability. The LoRa integration enhances reliability in low-bandwidth, long-range scenarios, making GeoPulse suitable for remote monitoring applications. Development will prioritize open-source contributions, with schematics, firmware, desktop application code, and communication protocols available in this repository for community collaboration.

## Getting Started
- **Hardware Setup**: Refer to the `/docs/hardware` directory for schematics, assembly instructions, and component lists.
- **Firmware Installation**: Follow the `/docs/firmware` guide to flash the ESP32-S3 with the latest GeoPulse firmware.
- **Desktop Application**: Install the desktop app from `/docs/software` for configuration, monitoring, and data analysis.
- **Cluster Configuration**: See `/docs/networking` for setting up gateway-based clusters and LoRa communication protocols.

## Contribution Guidelines
Enhance GeoPulse's firmware and software. Key areas for collaboration include:
- Optimizing signal processing algorithms for seismic data analysis.
- Enhancing LoRa-based cluster communication for improved reliability and scalability.
- Desktop app features, such as real-time visualization and automated reporting.

