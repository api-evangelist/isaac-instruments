# ISAAC Instruments (isaac-instruments)

ISAAC Instruments is a Canadian provider of in-cab technology and fleet management for the trucking industry - electronic logging devices (ELD), telematics, hours-of-service (HOS) compliance, driver workflow, messaging, and fuel/performance analytics, delivered as a fully managed hardware-plus-software platform. ISAAC runs an "Open Platform" with a documented API that lets fleets and 80+ integration partners (TMS/dispatch, maintenance, fuel tax, visibility, safety/compliance) share ISAAC data with their chosen vendors.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/isaac-instruments/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/isaac-instruments/refs/heads/main/apis.yml)

## Access Model (Important)

ISAAC's API is **real but partner-gated** - there is no self-serve public developer portal:

- Vendors apply through the **ISAAC partner program** (system integration via API, or an Android app on the in-cab device).
- The **complete API Guide and reference are documented inside the ISAAC InRealTime portal and Client Center**, provisioned to approved partners - not published on a public developer site.
- One capability is explicitly cited in ISAAC's public materials: **exporting drivers' hours-of-service information** (time spent in each duty status and distance traveled) via ISAAC APIs.
- Platform **pricing is contact-sales / request-a-quote** (custom, per-fleet); no public per-truck price is listed.

Because the concrete endpoints, base URLs, request/response schemas, and authentication are not public, the API surface below is **modeled** from ISAAC's public Open Platform description and partner integration categories (`endpointsModeled: true` in `review.yml`). No OpenAPI or AsyncAPI document was fabricated.

## Tags

- Trucking
- Telematics
- ELD
- Fleet Management
- Hours of Service
- Compliance
- Transportation
- Partner API

## Timestamps

- **Created:** 2026-07-04
- **Modified:** 2026-07-04

## APIs (Modeled)

### ISAAC Vehicles API
Fleet vehicles and tractor/trailer assets (identifiers, VIN, unit metadata) used to correlate telematics data.

### ISAAC Drivers API
Drivers and their profile, licensing, and assignment details managed on the ISAAC platform.

### ISAAC Hours of Service (ELD) API
Exports drivers' hours-of-service information captured by ISAAC's ELD - time in each duty status and distance traveled - for compliance, payroll, and TMS workflows. Explicitly cited in ISAAC's public materials.

### ISAAC Positions API
GPS positions and location breadcrumbs used by visibility and tracking partners.

### ISAAC Trips API
Trips, stops, and route/dispatch data flowing between ISAAC and TMS/dispatch partners.

### ISAAC Messaging API
Driver-to-dispatch messaging and in-cab workflow forms exchanged through the ISAAC platform.

### ISAAC Fuel and Performance API
Fuel consumption, idling, and driving-performance metrics used by fuel-tax (IFTA) and coaching partners.

### ISAAC Events API
Vehicle and safety events (fault/diagnostic codes, safety-critical events) surfaced to safety/compliance and maintenance partners.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/isaac-instruments)
- [Website](https://www.isaacinstruments.com/)
- [Documentation - Open Platform](https://www.isaacinstruments.com/platform/seamless-integration/open-platform/)
- [Partner Program](https://www.isaacinstruments.com/platform/seamless-integration/open-platform/join-isaac-become-a-partner/)
- [Plans - Request a Price](https://www2.isaacinstruments.com/request-a-price)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
