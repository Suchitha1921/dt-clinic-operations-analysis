# Task 1: Clinic Inventory Statistical Audit

## Problem Context

Small and mid-sized clinics typically manage medicine inventory through manual
entries without barcode systems. In such environments, inventory mismatches are
common due to missed entries, incorrect quantities, delayed updates, and high
patient load during peak hours.

Performing full inventory reconciliation daily is impractical and adds
operational friction. However, undetected errors lead to revenue leakage,
stock-outs, and loss of trust in data.

The objective, therefore, is not perfect reconciliation, but early detection
of error patterns using lightweight, daily statistical checks.

---

## How Inventory Moves Inside a Clinic

A typical inventory flow in a clinic follows this pattern:

- Opening stock is recorded
- Purchases are added manually
- Medicines are dispensed during consultations
- Sales or consumption are entered by staff
- Closing stock is updated in the system

Errors usually occur within this flow due to time pressure and manual handling.

---

## High-Risk Points for Inventory Errors

Inventory mismatches are most likely to occur in the following situations:

- Peak OPD hours when staff prioritize speed over entries
- Emergency dispensing without immediate billing
- Partial tablet or strip sales
- Delayed or incorrect purchase entry
- Manual corrections done retrospectively
- High-value or fast-moving medicines handled by multiple staff

These are routine, real-world scenarios rather than exceptional cases.

---

## Proposed Daily Statistical Micro-Audits

Instead of full reconciliation, the clinic can run small daily micro-audits
designed to detect anomalies early.

Proposed checks include:

- Randomly selecting 5 medicines per day for physical stock verification
- Rotating focus between high-value and fast-moving medicines
- Flagging items with stock reduction but zero recorded sales
- Identifying sudden drops or spikes compared to recent usage patterns
- Logging mismatches for review without assigning blame

These checks are quick, repeatable, and do not disrupt daily operations.

---

## Impact on SOP Discipline and Compliance

Regular micro-audits create awareness that inventory is being monitored
consistently, even if lightly. This leads to:

- Improved attentiveness during data entry
- Reduced habit of postponing entries
- Early correction of small errors before accumulation
- Greater confidence in inventory data over time

Most importantly, this approach improves discipline without increasing the
doctor’s workload or introducing fear-based controls.
