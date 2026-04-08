# Clinic Appointment & Diagnostics Platform - ER Diagram

This project presents an Entity-Relationship (ER) diagram for a clinic system that manages patients, doctors, appointments, consultations, diagnostic tests, reports and payments.

## Overview

The system is designed to handle the complete clinic workflow, from booking appointments to conducting consultations, prescribing tests, generating reports and managing payments.

## Key Design Points

Appointments and consultations are modeled separately to reflect real-world scenarios where not every appointment results in a consultation.

Patients can book multiple appointments and doctors can attend many patients across different appointments.

Consultations act as the central point where diagnoses are made and diagnostic tests are prescribed.

Multiple tests can be prescribed during a single consultation. Each test instance is tracked separately to manage status and reporting.

Reports are linked to specific prescribed tests, ensuring accurate tracking of results.

Payments are associated with appointments to track transaction details and status.

## Entities

* Patient
* Doctor
* Appointment
* Consultation
* Test
* ConsultationTest
* Report
* Payment

## Notes

The design is normalized, avoids redundancy and supports multiple visits, multiple tests per consultation and proper linkage between reports, consultations and payments.
