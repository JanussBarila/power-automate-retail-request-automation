# Retail Store Request Automation PoC

A portfolio proof of concept showing how a structured retail request register can be automated with Microsoft Power Automate.

## Scope

The project starts from an existing Excel table containing store requests. The request-capture mechanism is intentionally out of scope for this version.

## Automated process

1. Read structured requests from Excel.
2. Process only requests with `Status = New`.
3. Route requests by category.
4. Require approval when `Estimated Cost EUR > 500`.
5. On approval, update the request status and notify the relevant department.
6. On rejection, update the request status and stop department routing.

## Categories

- IT
- Equipment
- Marketing
- Maintenance
- Other

## Business value

- Reduces manual forwarding of requests.
- Adds consistent approval controls for higher-cost requests.
- Creates traceable request status.
- Provides a foundation for future SharePoint, Power Apps and Power BI integration.

## Repository structure

- `sample-data/` — anonymized Excel test data
- `power-automate/` — sanitized flow definition and expressions
- `docs/` — process logic and case-study notes
- `tests/` — functional test scenarios

All company names, user identities, tenant identifiers and connection details in this public repository are anonymized.
