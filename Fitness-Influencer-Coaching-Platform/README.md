# Fitness Coaching Platform - ER Diagram

This project presents an Entity Relationship diagram for an online fitness coaching platform managed by influencers/trainers.

## Overview

The system is designed to manage:

* Trainers and clients
* Coaching plans and subscriptions
* Sessions and consultations
* Client check-ins and progress tracking
* Payments for subscriptions

## Key Design Points

* **Unified User System**
  A single `user` entity is used with roles (`CLIENT`, `TRAINER`) to avoid duplication.

* **Plan vs Subscription Separation**
  Plans define coaching programs, while subscriptions track which client purchased which plan and for how long.

* **Session Management**
  Sessions (consultations, live calls, follow-ups) are handled separately from check-ins.

* **Progress Tracking**

  * `check_in` → periodic updates from clients
  * `progress_log` → structured tracking of physical progress

* **Trainer Support**
  Trainers can manage multiple clients and maintain notes using `trainer_note`.

* **Payment System**
  Payments are linked to subscriptions to track transactions and status.

## Entities

* User
* Plan
* Subscription
* Session
* CheckIn
* ProgressLog
* TrainerNote
* Payment

## Notes

The design is normalized, scalable and supports multiple clients per trainer, multiple subscriptions per client and structured progress tracking without mixing concerns.

---
