# Delivery 2: Software Architecture

This directory contains the second delivery (**Delivery 2**) of the **Stripe (Payment Processing)** platform project for the Cloud Computing course.

---

## Main Document Content

The core software architecture document is located here: [📄 groupN5_Delivery2.pdf](./groupN5_Delivery2.pdf). 

It details the internal design of the system, organized into the following key sections:

* **System Context & Architecture Diagrams:** C4 models showing external interactions (Level 1) and internal service decomposition and trust zones (Level 2).
* **Service Catalog:** Detailed specifications for the 11 independent services (e.g., Payment Orchestrator, Ledger Service, Tokenization Service), including their responsibilities, APIs, data ownership, and scaling drivers.
* **Data Architecture:** Data ownership models, storage strategies (relational vs. NoSQL), entity-relationship mapping, consistency requirements, and transaction boundaries (avoiding distributed ACID transactions).
* **Communication Architecture:** Synchronous vs. asynchronous communication matrices, highlighting the use of the Transactional Outbox pattern, event-driven propagation, and latency budgets (P95).
* **Architecture Decision Records (ADRs):** 6 documented decisions explaining the rationale behind choosing coarse-grained services, Event-Driven architecture (EDA), CQRS, and Orchestrated Sagas.
* **Requirements Traceability:** A comprehensive mapping of the Delivery 1 functional requirements to their responsible architectural services.

---

## Diagrams

All architecture diagrams used in the document are available as source files in the [`diagrams/`](./diagrams/) directory.

These include the editable sources (or exported image assets/links if designed in Canva, Draw.io, or PlantUML) for:
* System Context Diagram
* Service Decomposition and Interaction Topology Diagram
* Data Flow and Storage Trust Zones Diagram
* Entity-Relationship (Data Model) Diagram
* Communication (Synchronous/Asynchronous) Flow Diagram
