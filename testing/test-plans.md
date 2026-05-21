# Test Plans

## Strategy

- **Unit testing** — each feature tested in isolation
- **Integration testing** — features tested together
- **System testing** — full end-to-end flow

Techniques: Black-box testing, Equivalence Partitioning, Boundary Value Analysis, Decision Table Testing.

---

## Test Plan 1 – Login

**Precondition:** User has a registered account

| ID | Scenario | Test Data | Expected Result | Pass/Fail |
|---|---|---|---|---|
| TC01 | Login with correct credentials | Valid email + password | User logs in successfully | Pass |
| TC02 | Login with wrong password | Wrong password | Error message displayed | Pass |

---

## Test Plan 2 – Search for Commercial Rental Spaces

**Precondition:** User is logged in; listings exist in database

| ID | Scenario | Test Data | Expected Result | Pass/Fail |
|---|---|---|---|---|
| TC01 | Valid filters | Location: Al-Jamiah, Price: 25k–47k, Category: Retail | Matching listings displayed | Pass |
| TC02 | No filters | Empty | Prompt to enter at least one filter | Pass |
| TC03 | No results | Location: Unknown, Price: 0 | "No rentals match" + nearby suggestions | Pass |
| TC04 | Invalid format | Price: "yz", Category: "Castle" | Validation error, search blocked | Pass |
| TC05 | View property details | Valid listing selected | Full property data and map shown | Pass |
| TC06 | Bookmark a property | Valid listing | Added to bookmarks | Pass |
| TC07 | Contact agent | Valid listing | Contact option opens | Pass |
| TC08 | Server error | Server offline | "System retrieval failed, try again later" | Pass |

---

## Equivalence Partitioning

| Input | Class | Example | TC |
|---|---|---|---|
| Location | Valid | "Al-Jamiah" | TC01 |
| Location | Invalid | "Unknown" | TC03 |
| Location | Empty | "" | TC02 |
| Price | Valid | 25,000–47,000 | TC01 |
| Price | Invalid | "yz" | TC04 |
| Category | Valid | "Retail" | TC01 |
| Category | Invalid | "Castle" | TC04 |

---

## Boundary Value Analysis

| Field | Lower | Just Below | Exact | Just Above |
|---|---|---|---|---|
| Price | 0 | -1 (invalid) | 0 | 1 |
| Price | Upper limit | UpperLimit-1 | UpperLimit | UpperLimit+1 (invalid) |
| Size | 1 sqm | 0 (invalid) | 1 sqm | 2 sqm |

---

## Decision Table

| Rule | Location | Price | Category | Outcome |
|---|---|---|---|---|
| R1 | Valid | Valid | Valid | Results shown |
| R2 | Empty | Empty | Empty | Show all listings |
| R3 | Valid | Valid | Unmatched | No results found |
| R4 | Invalid | Invalid | Invalid | Validation error |
