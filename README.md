# VisApplication - Visa Application Website for Peaks of the Balkans

Welcome to VisApplication, an open-source project aimed at simplifying the visa application process for adventurers eager to explore the Peaks of the Balkans. This project is not only a tool to serve the hiking community but also a learning journey into the world of software architecture, specifically Domain-Driven Design (DDD), Clean Architecture (CA), and leveraging the capabilities of GPT and C#/.NET.

## Project Objectives
- To provide a seamless interface for users to apply for hiking visas.
- To explore and implement DDD and CA in a real-world application.
- To document the learning process and decisions in a public forum.

## Architecture Overview
The project is structured around Clean Architecture principles, ensuring our domain logic is at the core of the application's design. This approach allows us to create a system that is flexible, testable, and aligned with business goals.

## Unified Modeling Language (UML) Design

> Author's Note
>
> Please be aware that the UML diagrams may evolve during the development process.
> The purpose of this stage is to acquire a broad understanding of the application's architecture.
> Engaging with these diagrams could potentially reveal insights and considerations that were not initially apparent.

If you want to learn more about the different type of UML diagrams visit the [blog at creately.com](https://creately.com/blog/diagrams/uml-diagram-types-examples/)

### Structure Diagrams

**Profile Diagram**

Defines stereotypes and tagged values that extend the base UML model to create a domain-specific language. Use it to understand custom extensions made to standard UML to fit the project's needs.

<details>
    <summary>Profile Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/profile_diagram.png" alt="Profile Diagram">
    </div>
</details>


**Domain Model Diagram**

Provides a high-level view of the conceptual model, illustrating the main entities, their attributes, and relationships within the domain. This diagram helps to clarify the real-world constructs and their interconnections, setting a foundational understanding that informs more detailed system modeling.

<details>
    <summary>Domain Model Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/domain_model_diagram.png" alt="Domain Model Diagram">
    </div>
</details>

**Package Diagram**

Illustrates the organization and dependencies of different packages within a system. Read this diagram to see the system's modular structure and how high-level components are grouped.

<details>
    <summary>Package Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/package_diagram.png" alt="Package Diagram">
    </div>
</details>


**Component Diagram**

Describes the organization and interconnections of components within a system. It provides a high-level view of the system's building blocks and how they interact to provide functionality.

<details>
    <summary>Component Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/component_diagram.png" alt="Component Diagram">
    </div>
</details>

**Deployment Diagram**

Shows the physical deployment of artifacts on nodes, detailing the system's hardware and the middleware linking software components. Understand this to see how the system will be physically deployed across different machines.

<details>
    <summary>Deployment Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/deployment_diagram.png" alt="Deployment Diagram">
    </div>
</details>

**Composite Structure Diagram**

Outlines the internal structure of a class or a component, including its sub-parts and the interactions between them. Use this to grasp the detailed wiring and collaboration between parts of the system.

<details>
    <summary>Composite Structure Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/composite_structure_diagram.png" alt="Composite Structure Diagram">
    </div>
</details>


**Class Diagram**

Represents the static structure of the system, showing classes, their attributes, methods, and relationships. Interpret this to understand the blueprint of the system and how its data and behavior are defined.

<details>
    <summary>Class Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/class_diagram.png" alt="Class Diagram">
    </div>
</details>

**Object Diagram**

Depicts objects and their relationships at a specific point in time, giving a snapshot of the system's state. Look at this diagram to see examples of how classes and objects relate in practice.

<details>
    <summary>Object Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/structure/object_diagram.png" alt="Object Diagram">
    </div>
</details>

### Behavioral Diagrams

**Use Case Diagram**

Shows the interactions between users (actors) and use cases, where a use case represents a unit of useful functionality. Use this to identify the functions the system should perform from an external point of view.

<details>
    <summary>Use Case Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/use_case_diagram.png" alt="Use Case Diagram">
    </div>
</details>

**Activity Diagram**

Models the workflow and business processes in the system, illustrating the flow from one activity to another. This diagram helps you understand the sequence and conditions for how the system operates.

<details>
    <summary>Activity Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/activity_diagram.png" alt="Activity Diagram">
    </div>
</details>

**State Machine Diagram**

Describes the state changes that an object goes through in response to events, with each transition reflecting a change in the object's state. Use this to track the lifecycle of key entities within the system.

<details>
    <summary>State Machine Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/state_machine_diagram.png" alt="State Machine Diagram">
    </div>
</details>

**Sequence Diagram**

Displays the sequence of messages exchanged between objects and processes over time to carry out a specific function. Read this to follow the flow of control and communication between system components for particular scenarios.

<details>
    <summary>Sequence Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/sequence_diagram.png" alt="Sequence Diagram">
    </div>
</details>

**Communication Diagram**

Shows the interactions between objects or parts based on their relationships and the messages they exchange. It provides an alternative to sequence diagrams, focusing on object collaboration.

<details>
    <summary>Communication Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/communication_diagram.png" alt="Communication Diagram">
    </div>
</details>


**Interaction Overview Diagram**

<details>
    <summary>Interaction Overview Diagram (click to expand)</summary>
    <div style="text-align: center;">
      <img src="docs/uml/behavioral/interactive_overview_diagram.png" alt="Interaction Overview Diagram">
    </div>
</details>

## GPT Conversations

Within the VisApplication project, GPT serves as a tool for ideation and problem-solving. It aids in the architectural design and decision-making process through interactive conversations. Here’s how it contributes to the project:

- **Design Brainstorming**: By discussing various architectural approaches and patterns, GPT helps in exploring different design solutions for the application.
- **Clarifying Concepts**: Conversations with GPT offer clarification on complex topics related to Domain-Driven Design (DDD), Clean Architecture (CA), and other software engineering principles.
- **Decision Documentation**: Dialogues with GPT are used to question and justify decisions, forming a documented trail that supports the rationale behind architectural choices.
- **Learning Enhancement**: Engaging with GPT enables a deeper understanding of .NET and C# concepts, assisting in keeping the project aligned with current best practices.

These conversations with GPT are documented and made accessible, offering insights into the thought processes behind the system’s design:

- [GPT README](docs/gpt/0-README.md): An overview of the GPT-assisted conversations shaping VisApplication.
- [Project Setup](docs/gpt/1-project_setup.md): Insights into setting up the project, as informed by GPT discussions.
- [Software Architecture and System Design](docs/gpt/2-software_architecture_and_system_design.md): A record of discussions shaping the software architecture and system design.
- [UML Design](docs/gpt/3-UML_design.md): A collection of UML diagrams inspired by conversations with GPT, illustrating the system's structure.


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.