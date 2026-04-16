---
uid: Nokia_Altiplano_Solution_Installation
---

# Nokia Altiplano Solution Installation

## Prerequisites

Before installing the Nokia Altiplano Solition, ensure that the following requirements are met:

- The DataMiner version installed must be *Main Release 10.6.0.0 – 16985 CU1* or a more recent release.

- [Install the **Nokia Altiplano** solution](#installing-the-nokia-altiplano-solution).

- Perform the [Initial Configuration Requirements](#initial-configuration-requirements).

## Install the Nokia Altiplano solution

To deploy the Nokia Altiplano Solution, follow the steps below:

1. Open the **Catalog** and locate the *Nokia Altiplano Solution*.

2. Click the *Deploy* button

3. Choose the target **DataMiner System** and confirm the deployment. 
    - The solution package will be automatically pushed to the selected system.

Upon successful deployment, the following four DataMiner elements will be created within the Nokia Altiplano view:

- Altiplano Manager – Master

- Altiplano Manager – Slave

- Altiplano REST Interface

- Altiplano Kafka Analyzer

## Initial Configuration Requirements

Before operating the Nokia Altiplano Solution, several configuration steps must be completed to ensure proper functionality and data flow. The following sections outline the required initial setup.

### Configure REST Interface Credentials

To establish communication with the Altiplano API, credentials must be configured for the REST Interface. 

Refer to the [Nokia Altiplano REST Interface - Initialization Section] (https://docs.dataminer.services/connector/doc/Nokia_Altiplano_REST_Interface_Technical.html) for detailed instructions.

### Configure Import/Export Settings

Each Nokia Altiplano Element requires proper Import/Export configuration to ensure that generated files are stored in the correct location. Perform the following steps:

1. Navigate to the Configuration page of each Altiplano Element

2. Under System Credentials, set the following parameters:
    - *System Username*
    - *System Password*

3. Define the directory paths:
    - *Import Directory*
    - *Export Directory*

4. Specify the directory type for each path:
    - *Import Directory Type*
    - *Export Directory Type*
        - Options: **Local** or **Remote**

### Configure OLTs per Slave Element

For each Altiplano Manager operating in the Slave role, Optical Line Terminals (OLTs) must be assigned to ensure proper monitoring and data distribution. Complete the following steps:

1. Navigate to the Slave OLTs page.

2. Select Add OLT from the top‑right corner of the page.

3. Provide the following information:
    - *OLT Name*
    - *Element ID* of the corresponding OLT element

