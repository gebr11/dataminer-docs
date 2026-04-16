---
uid: Nokia_Altiplano
---

# Nokia Altiplano Solution

The **Nokia Altiplano Solution** is designed around a comprehensive **data ingestion and administration layer** that centralizes control, coordination, and distribution across the platform. 

At the core of this architecture is the *Nokia Altiplano Manager*, which functions as the primary orchestrator. It manages communication between interfaces and downstream consumers, ensuring efficient data flow, workload distribution, and seamless integration of solution components.

## Architecture Overview:

The solution is composed of four primary components:
- [Nokia Altiplano Manager] (xref:Nokia_Altiplano_Solution_Components#nokia-altiplano-manager)

- [Nokia Altiplano REST Interface] (xref:Nokia_Altiplano_Solution_Components#nokia-altiplano-rest-interface)

- [Nokia Altiplano Kafka Analyzer] (xref:Nokia_Altiplano_Solution_Components#nokia-altiplano-kafka-analyzer)

- [Nokia Altiplano OLT] (xref:Nokia_Altiplano_Solution_Components#nokia-altiplano-olt)


> [!IMPORTANT]
> Before installing this solution, ensure that you meet all [prerequisites](xref:Nokia_Altiplano_Solution_Installation#prerequisites).
