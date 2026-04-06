# Instagram Thrift Store - ER Diagram

This db presents an Entity Relationship diagram for a small Instagram based thrift and handmade product store.

## Overview

The system is designed to manage:

* Products (thrift and handmade)
* Inventory and stock availability
* Customer information
* Orders and order items
* Payments and shipping status

## Key Design Points

* **Product vs Inventory separation**
  Products store general details, while inventory handles stock, size, color and condition.

* **Thrift vs Handmade support**

  * Thrift items are unique (`is_unique = true`, quantity = 1)
  * Handmade items can have multiple units

* **Order Management**

  * One customer can place multiple orders
  * One order can contain multiple products (via `order_item`)

* **Tracking System**

  * Payment status (paid, pending, failed)
  * Shipping status (pending, shipped, delivered)

## Entities

* Customer
* Product
* Inventory
* Order
* OrderItem
* Payment
* Shipping

## Notes

The design is normalized, avoids redundancy and is structured to support future scaling (e.g. product variants or multiple inventory entries).

---
