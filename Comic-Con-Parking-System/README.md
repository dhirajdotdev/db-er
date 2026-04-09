# Comic-Con Parking System  - ER Diagram

This project presents an Entity-Relationship (ER) diagram for a multi-zone parking system designed for a large event like Comic-Con.

## Overview

The system manages vehicle entry and exit, parking spot allocation, ticket generation, parking sessions and payments across multiple zones and levels within the venue.

## Key Design Points

Vehicles are categorized by type (bike, car, SUV, EV) and parking spots are assigned based on compatibility and availability.

Parking spots are organized into zones and levels and can also be reserved for specific categories such as VIPs, staff, exhibitors, cosplayers, or EV charging.

Each vehicle entry creates a parking session that records entry and exit timestamps, along with the assigned parking spot.

Tickets are issued for each parking session and linked one-to-one for tracking purposes.

Parking spots can be reused across multiple sessions and vehicles can enter the facility multiple times during the event.

Payments are linked to parking sessions to track parking fees and transaction status.

## Entities

* Vehicle
* VehicleType
* Zone
* ParkingSpot
* SpotCategory
* Ticket
* ParkingSession
* Payment

## Notes

The design is normalized, avoids redundancy and supports real-world requirements such as multiple visits per vehicle, reusable parking spots, reserved categories and accurate tracking of parking sessions, availability and payments.
