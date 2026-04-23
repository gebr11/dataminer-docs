---
uid: Nokia_Altiplano_Solution_Components
---

# Nokia Altiplano Solution Components

## Nokia Altiplano Manager

The **Nokia Altiplano Manager** serves as the central orchestrator of the solution. It is responsible for managing queries and processing files. This component operates in two distinct roles:

### Master Role
- Only one element is required.

- Contains the core configuration.

- Distributes the data processing load across the system.

### Slave Role
- One or multiple elements can be deployed.

- Handles portions of the data processing.

- Manages assigned Optical Line Terminals (OLTs).

For further details, refer to the official [connector documentation](https://docs.dataminer.services/connector/doc/Nokia_Altiplano_Manager.html)

## Nokia Altiplano REST Interface

The **Nokia Altiplano REST Interface** is responsible for executing REST API requests to the Altiplano API. Its primary functions include:

- Ensuring REST communication with the Altiplano API.
- Retrieving API data and storing it in files for each executed request.
- Allowing multiple elements to be created to distribute request loads, while respecting vendor-imposed request limits.

For further details, refer to the official [connector documentation](https://docs.dataminer.services/connector/doc/Nokia_Altiplano_REST_Interface.html)

## Nokia Altiplano Kafka Analyzer

The **Nokia Altiplano Kafka Analyzer** processes Kafka files and performs the following tasks:

- Separates information contained in Kafka files.

- Generates individual files per OLT.

- Reports processed information back to the Altiplano Manager (Slave Role) for OLT management.

- Supports multiple elements to distribute the file processing workload.

For further details, refer to the official [connector documentation](http://docs.dataminer.services/connector/doc/Nokia_Altiplano_Kafka_Analyzer.html)

## Nokia Altiplano OLT

The **Nokia Atiplano OLT** consolidates all REST API and Kafka information into a single component. Its responsibilities include:

- Aggregating OLT data received from both REST and Kafka sources.

- Distributing data by type (Boards, PON, Hardware, Uplink, and Alarms).

- Providing monitoring capabilities across all OLT-related information.

For further details, refer to the official [connector documentation](https://docs.dataminer.services/connector/doc/Nokia_Altiplano_OLT.html)