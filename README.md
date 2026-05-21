# MaqsadRentalSWE

A data-driven real estate support system that helps entrepreneurs identify optimal commercial rental locations by analyzing neighborhood service gaps and community needs.

> Built as part of a project for course CPCS351 – Software Engineering (First Semester 2025)  
> King Abdulaziz University | Faculty of Computing and Information Technology.

---

## The Problem

In many cities, services are unevenly distributed across neighborhoods — some areas are saturated with the same type of business (e.g. multiple cafés side by side), while others are missing essential services like pharmacies, nurseries, or grocery stores. Entrepreneurs often make location decisions based on guesswork, leading to failed investments and underserved communities.

## What Maqsad Does

Maqsad bridges the gap between available rental listings and actual community needs. Instead of just showing *what's available*, it tells investors *what's needed* — and where.

### Core Features

| Feature | Description |
|---|---|
| Rental Availability | Browse commercial spaces with detailed info and map access |
| Service Gap Analysis | Identifies missing business types per neighborhood |
| Personalized Alerts | Notifies users when new listings match their preferences |
| Resident Surveys | Residents report missing services, feeding into the analysis |
| Shared Rental Option | Multiple small businesses can share one space |
| Future Growth Forecasting | Predicts upcoming commercial needs using demographic data |
| Interactive Smart Map | Green = high potential, Yellow = medium, Red = saturated |
| Contact Agent Button | Direct communication with property agents |

---

## System Architecture

Maqsad uses a **Three-Tier Architecture**:
Presentation Layer   →   Mobile UI, maps, dashboards, surveys
Application Layer    →   Business logic, notifications, analytics engine
Data Layer           →   Listings DB, survey data, demographic datasets, map APIs

---
| File | Contents |
|---|---|
| `docs/requirements.md` | Functional & non-functional requirements, use cases, stakeholders |
| `docs/architecture.md` | System design, subsystems, architectural decisions |
| `testing/test-plans.md` | Test plans, equivalence partitioning, BVA, decision tables |
| `diagrams/` | UML activity, state, and sequence diagrams |

---

## Research & Validation

A survey was conducted with entrepreneurs and residents to validate the problem:

- **80%** reported difficulty choosing the right business location
- **60%** cited too many similar businesses as the main obstacle
- **53%** mentioned high rental prices
