# Gateway Agent Pattern

This repository contains the source code and pseudocode developed for the paper "_Gateway Agent Pattern for Asset Integration: A Reference Implementation_". It provides the reference implementations of the Gateway Agent Pattern (GAP), a design pattern that decouples the control logic of an agent from the protocol-specific communication required to interact with an industrial asset.

## Repository structure

The repository is organized into three main folders:

- [JADE](https://github.com/GCIS-UPV-EHU/GatewayAgentPattern/tree/main/JADE): This folder contains the code related to the reference implementation of the GAP in JADE (Java Agent DEvelopment Framework). The folder is divided by asset communication protocol:
  - `JADE_MQTT`: implementation for MQTT-based assets.
  - `JADE_OPCUA`: implementation for OPC UA-based assets.
  - `JADE_ROS`: implementation for ROS-based assets.

- [SPADE](https://github.com/GCIS-UPV-EHU/GatewayAgentPattern/tree/main/SPADE): This folder contains the code related to the reference implementation of the GAP in SPADE (Smart Python Agent Development Environment). The folder is divided by asset communication protocol:
  - `SPADE_OPCUA`: implementation for OPC UA-based assets.
  - `SPADE_ROS`: implementation for ROS-based assets.

- [Pseudocode](https://github.com/GCIS-UPV-EHU/GatewayAgentPattern/tree/main/Pseudocode): Platform-independent pseudocode of the GAP. It includes the generic gateway manager, gateway agent, and `StructMessage` command structure, as well as the data-oriented and connection-oriented gateway variants. Protocol-specific examples for MQTT, OPC UA, and ROS are available in the `Examples` folder.

The JADE and SPADE folders contain the platform- and protocol-specific adaptations of the generic structure defined in the `Pseudocode` folder.
