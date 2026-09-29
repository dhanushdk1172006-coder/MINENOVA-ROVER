#MineNova – Predictive AI-Powered Autonomous Mine Rescue & Communication Rover

🚀 Project Overview
MineNova is a predictive AI-powered autonomous mine rescue and communication rover developed for the Smart India Hackathon 2026.
The project addresses underground mine safety through autonomous exploration, real-time hazard monitoring, risk-aware navigation, survivor localization, and resilient communication.
MineNova aims to help rescue teams understand underground conditions before entering potentially dangerous areas. Instead of selecting routes based only on distance, the system is designed to consider hazards, terrain, survivor information, and communication connectivity.
Core concept: The rover maps the mine and understands its risks.


🎯 Problem Statement
Problem Statement ID: 26039
Problem Statement Title: AI-Powered Underground Mine Safety, Monitoring and Rescue System
Theme: Smart Automation
Category: Hardware
Team Name: MineNova
Team ID: 132254
Hackathon: Smart India Hackathon 2026


💡 Proposed Solution
MineNova integrates robotics, artificial intelligence, sensor fusion, autonomous navigation, acoustic localization, and wireless communication into a mobile mining rescue platform.
The system is designed to:
Explore underground tunnels autonomously.
Map tunnel geometry and detect obstacles.
Monitor environmental hazards.
Identify safer routes using hazard-aware path planning.
Detect and estimate the direction of possible trapped-survivor sounds.
Use thermal and visual sensing to assist survivor detection.
Predict potential communication loss and support timely relay deployment.
Present mine conditions through a Digital Safety Twin.


✨ Key Features
1. Autonomous Exploration
LiDAR and IMU-based SLAM support underground mapping, localization, and navigation through tunnels and debris-strewn terrain.
2. Edge Sensor Fusion
The system combines gas, terrain, acoustic, thermal, and communication information to develop a broader understanding of underground conditions.
3. Predictive Hazard AI
Risk-aware planning is designed to consider hazardous regions when selecting routes, helping the rover prefer safer paths rather than simply the shortest paths.
4. Survivor Localization
A four-microphone array using Time Difference of Arrival (TDOA), together with thermal and night-vision imaging, supports the detection and localization of possible survivors.
5. Resilient Communication
Wireless communication monitoring uses Received Signal Strength Indicator (RSSI) trends to identify possible connectivity degradation and support relay deployment before communication is lost.
6. Digital Safety Twin
A live digital representation of the mine is designed to display mapping, hazards, possible survivor locations, and communication status in one view.
7. Rugged Rover Design
The proposed mechanical design uses six-wheel rocker-bogie mobility for traversing uneven surfaces, rocks, debris, and inclines.
8. Safety-Conscious Electronics
The design proposes a sealed enclosure, battery management, thermal and current monitoring, sealed connectors, and isolated low-voltage wiring. Actual mine deployment requires appropriate safety validation and certification.


🏗️ System Architecture
MineNova is organized into the following functional modules:
Perception Layer: RGB camera, thermal camera, night-vision camera, LiDAR, microphones, and environmental sensors.
Sensor Processing Layer: Processes sensor measurements and combines information from different sources.
Mapping and Localization Layer: Uses LiDAR and IMU-based SLAM for underground mapping and localization.
AI and Hazard Assessment Layer: Analyzes available sensor information to assess hazards and support risk-aware decisions.
Navigation Layer: Plans routes and adjusts movement based on obstacles and estimated risk.
Survivor Detection Layer: Uses acoustic and thermal/visual information to assist survivor localization.
Communication Layer: Uses Wi-Fi mesh for video/data and LoRa for low-rate telemetry.
Digital Safety Twin: Presents the mine map, hazard information, survivor indications, and connectivity status.


🔩 Hardware Components
Component
ESP32
👥 Team Information
Project: MineNova
🔗 Project Links
3D Design: https://skfb.ly/pNTs9
📚 Research References
DARPA SubT / ACHORD (2022) — Communication-aware subterranean exploration and deployable radios.
Consult the original publications and add complete bibliographic details and verified links before formal submission.


⚠️ Disclaimer
MineNova is a prototype in development intended to support underground mine safety assessment and rescue operations. Its detection, navigation, communication, and hazard-monitoring capabilities require systematic testing and validation. It must not replace certified safety equipment, trained rescue personnel, or established emergency procedures.
MineNova — Mapping the Mine. Understanding the Risks. Supporting Safer Rescue.

Team Name: MineNova
Project Drive: https://drive.google.com/drive/folders/1ZgWAYJHKlp5gCZV6qoxJmjRh4jmFEmYU
Underground Mine UGV (2025) — Underground mapping, thermal sensing, air-quality monitoring, SLAM, and AI.
Team ID: 132254
Purpose
GitHub Repository: https://github.com/dhanushdk1172006coder/MINENOVA/tree/main
Mine Rescue Robotics Review (2026) — Review of mine-rescue robotics, autonomy, sensing, communication, and safety requirements.
Event: Smart India Hackathon 2026
Project Website: https://soosaiarul-07.github.io/minenova/#


Wireless Mesh Rescue Robot (2026) — Mine-rescue robotics using mesh communication, multi-parameter sensing, and deployable relays.
Department: [Enter department]
Project Video: https://youtu.be/jXeFdArsQ_o
Institution: [Enter institution name]
Rover control and sensor interfacing
Raspberry Pi 4/5
Edge computing, SLAM, and AI processing
YDLIDAR X2
LiDAR-based mapping and obstacle detection
IMU
Motion measurement and localization support
RGB camera
Visual monitoring
Thermal camera
Thermal imaging for survivor-search assistance
Night-vision camera
Visibility in low-light environments
Four-microphone array
Acoustic localization using TDOA
Gas sensors
Prototype environmental gas monitoring
Motor driver and encoders
Motor control and motion feedback
Wi-Fi mesh
Video and data communication
LoRa module
Low-rate telemetry
LiFePO₄ battery and BMS
Power supply and battery monitoring
Communication relays
Connectivity support in underground environments
Prototype gas sensors: MQ-4, MQ-7, and MH-Z19B, as specified in the project presentation.
Deployment consideration: Real mine deployment requires a certified intrinsically safe multi-gas monitoring solution appropriate to the mine environment. Prototype sensors are not a substitute for certified mine-safety equipment.


💻 Software and Technologies
Python
Computer vision and image processing
YOLOv8-nano for lightweight object detection
LiDAR and IMU-based SLAM
Acoustic signal processing
Time Difference of Arrival (TDOA)
Sensor fusion
Risk-aware path planning
RSSI trend analysis
Embedded control using ESP32
Edge AI processing using Raspberry Pi
Wireless mesh communication and LoRa telemetry
The final software stack should reflect the technologies actually implemented and tested in the prototype.


⚙️ Working Principle
The rover enters the underground environment using remote-controlled or autonomous operation.
LiDAR and IMU data support mapping and localization in GPS-denied tunnels.
Environmental sensors collect readings for selected gases and other monitored conditions.
Sensor information is processed to build an estimate of the surrounding environment and potential hazards.
The navigation module uses the resulting risk map to support route selection and obstacle avoidance.
Four microphones collect sound from different directions. TDOA processing estimates the direction of possible survivor sounds.
Thermal and visual sensing assists in identifying potential survivors.
RSSI trend analysis monitors communication quality and supports proactive relay deployment.
The Digital Safety Twin brings together map, hazard, survivor, and communication information for the operator.
Rescue teams use the collected information to support assessment and rescue planning.


🛡️ Safety and Reliability
MineNova is designed with underground safety challenges in mind:
GPS-denied navigation using LiDAR and IMU-based SLAM.
Hazard-aware route planning.
Environmental monitoring and real-time alerts.
Communication-loss awareness and relay support.
Rugged mobility for uneven underground terrain.
Sealed electronics and battery monitoring.
Modular sensing, computing, and communication architecture.
The proposed design is not certified for operation in explosive mine atmospheres. Appropriate engineering validation and mine-specific certification are required before real-world deployment.


📊 Feasibility and Viability
Dual-tier computing: ESP32 handles control and sensor interfacing, while Raspberry Pi supports edge computing and AI workloads.
Modular design: Sensor, computing, and communication modules are intended to be replaceable.
Communication strategy: Wi-Fi mesh supports video/data, while LoRa supports low-rate telemetry.
Autonomous navigation: LiDAR and IMU-based SLAM support navigation where GPS is unavailable.
Reusable communication relays: Relays are intended to be recoverable and reusable after missions.
Scalable platform: The architecture is intended to support multiple mine-rescue missions.
Preliminary Design Targets
The project presentation identifies the following targets:
Battery runtime: 3–4 hours.
Wi-Fi mesh communication: approximately 100 metres per hop target.
Relay-deployment trigger: RSSI trend monitoring, with approximately −80 dBm indicated as a reference threshold.
Estimated bill of materials: ₹70,000–₹90,000.
These are preliminary project targets and estimates, not independently validated performance results.


🌍 Impact and Benefits
For Mine Operators
Supports preliminary underground risk assessment.
May help reduce avoidable operational downtime.
Provides a modular platform for mine monitoring.
For Rescue Teams
Supplies hazard and route information before entry.
Supports the search for possible trapped workers.
Provides information about underground connectivity.
For Miners and Workers
Supports continuous monitoring of selected environmental conditions.
Aims to improve situational awareness during mining operations.
For Regulators
The proposed Digital Safety Twin can support organized recording of hazard readings, maps, and incident timelines.
Broader Applications
The platform concept may be adapted for search and rescue, tunnel and subway inspection, and other confined-space monitoring tasks, subject to application-specific redesign and validation.


🔬 Research Gap and Innovation
Existing research and robotic platforms demonstrate capabilities such as underground mapping, autonomous exploration, environmental sensing, survivor detection, and communication support.
MineNova focuses on combining these capabilities at the decision-making level.
Its proposed innovation is the integration of:
Hazard-aware route selection.
Survivor-related information.
Terrain and tunnel mapping.
Communication-quality prediction.
Proactive communication-relay management.
A unified Digital Safety Twin.
The objective is to move from isolated sensing functions toward coordinated, risk-aware rescue assistance.


🧪 Development Status
Current status: Prototype in progress.
The project presentation describes a development approach involving core rover control, sensing, communication integration, and simulation-based validation of SLAM and hazard-aware path planning.
Actual completion and testing status should be updated as development progresses.


Future Enhancements

Improve autonomous navigation in complex underground environments.
Validate survivor localization accuracy under different noise conditions.
Test hazard-aware planning using realistic mine scenarios.
Improve communication reliability in obstructed tunnels.
Integrate certified mine-safety sensors for deployment-oriented development.
Conduct controlled field trials and measure performance.
Develop and validate the Digital Safety Twin interface.
Improve autonomous navigation in complex underground environments.
Validate survivor localization accuracy under different noise conditions.
Test hazard-aware planning using realistic mine scenarios.
Improve communication reliability in obstructed tunnels.
Integrate certified mine-safety sensors for deployment-oriented development.
Conduct controlled field trials and measure performance.
Develop and validate the Digital Safety Twin interface.