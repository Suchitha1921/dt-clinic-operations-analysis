# Task 2: Patient Care & Communication System Design

## Problem Context

Clinics often rely on informal communication channels, especially WhatsApp, to
handle patient follow-ups, reminders, and queries. Over time, this leads to
communication overload, delayed responses, and unnecessary doctor involvement
in non-clinical tasks.

The challenge is to maintain care quality while minimizing interruptions and
protecting the doctor’s time.

---

## Patient Message Classification Framework

Patient communication can be broadly classified into two categories:

### Automated Communication
- Appointment reminders
- Follow-up reminders
- Prescription refill notifications
- Lab report availability messages
- Standard care instructions

### Human-in-the-Loop Communication
- New or worsening symptoms
- Complications after treatment
- Emergency-related concerns
- Queries requiring medical judgment

This classification ensures that automation handles routine communication,
while critical cases receive appropriate human attention.

---

## Google Sheet as a Control System

A Google Sheet can act as a simple control center for patient communication.

Key columns may include:
- Patient ID
- Last visit date
- Follow-up due date
- Message category
- Automation status
- Escalation flag
- Assigned staff member

The sheet acts as a decision layer rather than a messaging tool.

---

## Workflow Design

The proposed workflow is as follows:

1. Patient data is exported from the HMS
2. Data is updated in the Google Sheet
3. The sheet determines whether communication is automated or manual
4. Routine messages are sent automatically or by staff
5. Only escalated cases reach the doctor
6. All actions are logged for visibility

This workflow reduces chaos while preserving accountability.

---

## Optional Automation Layer

If required, this system can be enhanced using:
- Google Apps Script for triggers
- Messaging APIs for automated notifications

These enhancements are optional and can be introduced gradually as the clinic
matures operationally.
