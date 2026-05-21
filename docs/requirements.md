# Requirements

## Stakeholders

| Stakeholder | Role |
|---|---|
| Entrepreneurs & small business owners | Primary users — explore areas, analyze gaps, receive recommendations |
| Residents | Submit surveys reporting missing services |
| Property agents & landlords | Publish and manage commercial rental listings |
| City planners & local authorities | Use gap analysis for urban planning (secondary users) |

---

## Functional Requirements

| ID | Requirement |
|---|---|
| FR01 | Display available commercial rental spaces with detailed property information |
| FR02 | Show rental locations on an interactive map |
| FR03 | Analyze neighborhoods and identify missing service types |
| FR04 | Generate service gap reports for selected areas |
| FR05 | Send personalized alerts when new listings match user preferences |
| FR06 | Allow residents to submit surveys about missing services |
| FR07 | Provide a shared rental option for multiple small businesses |
| FR08 | Display a dashboard with charts and KPIs |
| FR09 | Allow users to contact property agents directly |
| FR10 | Provide future growth forecasts based on demographic data |
| FR11 | Allow users to save/bookmark rental listings |
| FR12 | Send push notifications for saved listing price changes |

---

## Non-Functional Requirements

| ID | Category | Requirement |
|---|---|---|
| NFR01 | Usability | Simple enough for non-technical users without training |
| NFR02 | Performance | Search results load within 3 seconds under normal conditions |
| NFR03 | Scalability | Supports expansion to new cities without architectural changes |
| NFR04 | Security | User data stored securely with access controls |
| NFR05 | Availability | 99% uptime during business hours |
| NFR06 | Accuracy | Gap analysis based on verified, up-to-date data |
| NFR07 | Compatibility | Supports both iOS and Android |

---

## Use Cases

### UC01 – Analyze Neighborhood Data
- **Actor:** Entrepreneur
- **Goal:** View service gaps and opportunities in a selected area
- **Flow:** Select area on map → system retrieves data → gap report generated → user views results

### UC02 – Search for Commercial Rental Spaces
- **Actor:** Entrepreneur
- **Goal:** Find available rental spaces matching filters
- **Flow:** Enter filters → system returns listings → user views details and map

### UC03 – Submit Resident Survey
- **Actor:** Resident
- **Goal:** Report missing services in their neighborhood
- **Flow:** Open survey → answer questions → submit → data feeds into gap analysis
