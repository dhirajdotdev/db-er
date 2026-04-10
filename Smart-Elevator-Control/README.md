# Smart Elevator Control System  - ER Diagram

This project presents an Entity-Relationship (ER) diagram for a smart elevator control platform designed for large buildings such as corporate towers, malls, airports and residential complexes.

## Overview

The system manages multiple buildings, elevators, floor requests, ride assignments, elevator status, maintenance tracking and ride history in a structured and scalable way.

## Key Design Points

Buildings contain multiple floors and elevator shafts and each shaft contains one elevator.

Elevators can serve multiple floors and floors can be served by multiple elevators using a mapping structure.

Floor requests are generated from different floors and tracked with statuses such as pending, assigned and completed.

Each request is assigned to an elevator and results in a ride record that stores start and end timestamps.

Elevator status is tracked separately to represent real-time states like idle, moving, or maintenance.

Maintenance is modeled as a separate entity to maintain historical records without affecting elevator configuration.

Ride logs are stored independently to support analytics and performance monitoring.

## Entities

* Building
* Floor
* Shaft
* Elevator
* ElevatorFloor
* Request
* Ride
* Maintenance

## Notes

The design is normalized, avoids redundancy and supports multi-building environments, multiple elevators per building, flexible floor servicing, efficient request handling, ride tracking and maintenance history management.
