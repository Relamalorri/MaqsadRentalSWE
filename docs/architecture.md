# Architecture

## System Type

Maqsad is an **interactive, data-driven decision support system**. It continuously responds to user inputs, updates maps in real time, sends instant notifications, and processes analytics dynamically.

---

## Three-Tier Architecture
Presentation Layer   →   Mobile UI, maps, dashboards, surveys
Application Layer    →   Business logic, notifications, analytics, recommendations
Data Layer           →   Listings DB, survey data, demographics, map APIs

---
### Layer Responsibilities

**Presentation Layer**
- Mobile app (iOS and Android)
- Interactive color-coded map
- Dashboard with charts and KPIs
- Resident survey forms

**Application Layer**
- Search, filtering, and recommendation logic
- Notification and alert service
- Neighborhood analytics and gap analysis engine

**Data Layer**
- Commercial rental listings database
- Resident survey responses
- Demographic and city expansion datasets
- External map API integration

---

## Subsystems

| Subsystem | Responsibility |
|---|---|
| Entrepreneur Subsystem | Explore areas, analyze gaps, receive recommendations |
| Resident Subsystem | Submit surveys and neighborhood feedback |
| Property Agent Subsystem | Publish and manage rental listings |
| Analytics Subsystem | Neighborhood analysis and gap reports |
| Notification Subsystem | Personalized alerts and push notifications |
| Map Integration Subsystem | Geographic and service data display |

---

## Design Principles

- **Separation of layers** — each tier has a single responsibility
- **Scalability** — new cities added without restructuring
- **Maintainability** — modular subsystems updated independently
- **User-centric** — built for solo entrepreneurs, not enterprise clients
