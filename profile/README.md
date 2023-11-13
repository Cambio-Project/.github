# Cambio-Project

# Goal
The Cambio-Project encompasses a collection of tools designed for Chaos Engineering. Its purpose is simulating and analysing the transient behavior of a microservice systems in resilience scenarios.

## Overview

![dispel_overview](https://github.com/Cambio-Project/.github/assets/77619091/9767110d-0b95-44df-9b2c-3a52e8e32bcf)


The  DiSpel components are eight tools with different responsibilites.

| **Component** | **Short Description** |
|---------------|-----------------------|
| [TransVis frontend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-backend/tree/master) & [TransVis backend](https://github.com/Cambio-Project/conversational-transient-behavior-visualization-frontend/tree/master)  | TransVis visualizes the transient behavior (i.e. QoS over time) of a microservice system. Additionally offers a chatbot for interactive analysis. |
| [TQPropRefiner](https://github.com/Cambio-Project/transient-behavior-requirement-refiner)   | The TQPropRefiner is a tool for the refinement of the temporal ocmponent of a generic PSP. |
| [SAE Tool](https://github.com/Cambio-Project/software-architecture-extraction)   |  The SAE tool uses event traces of a microservice application to create an architectural model. |
| [TL-Tea](https://github.com/Cambio-Project/TL-Tea)   | TL-Tea parses and converts LTL and MTL patterns into tree structures, that can be evaluated and improved. |
| [PSP Wizard](https://github.com/Cambio-Project/PSPWizardExtended)   | The PSPWizard allows for the machine-assisted creation of Property Specification Patterns (PSPs). |
| [RESIRO](https://github.com/Cambio-Project/hazard-elicitation)   |  RESIRIO is a chatbot approach for helping developers to create resilience scenarios. |
| [MiSim](https://github.com/Cambio-Project/MiSim)   | MiSim simulates a microservice system with customizable capacities, loadbalancing strategies, network delays and other real-world factors. |
| [TBVerifier](https://github.com/Cambio-Project/transient-behavior-verifier)    | The TBVerifiers enables monitoring the transient behavior of a microservice system after the injection of an anomaly.
