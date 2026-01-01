# City Cinema Management System (Java, Arrays Only)

A city-wide cinema management system built from scratch in Java using **only arrays**.  
The project models real-world cinema operations while practicing core OOP principles without relying on Java Collections.

This system manages multiple cities, cinemas, screens, and seats, supporting booking, cancellation, reporting, and discovery of available seats.

---

## Core Concepts Demonstrated

- Encapsulation and controlled state changes
- Enum-based seat classification
- Jagged 2D arrays for seating layouts
- Multi-class collaboration
- Manual array resizing (no ArrayList, HashMap, etc.)
- Clear separation of responsibilities

---

## Main Entities

- **Seat**  
  Represents a single seat with ID, type (REGULAR, PREMIUM, VIP, RECLINER), price, and availability.

- **Screen**  
  Physical auditorium backed by a jagged 2D `Seat[][]` array.  
  Handles layout display, seat lookup, booking, cancellation, and counts.

- **Cinema**  
  Aggregates multiple screens under one branch using `Screen[]`.  
  Forwards operations and generates cinema-level reports.

- **CityCinema**  
  Manages multiple cinema branches across a city using `Cinema[]`.  
  Supports city-wide aggregation and VIP seat discovery.

---

## Pricing Policy (Visible in Output)

| Seat Type   | Price (PKR) |
|------------|-------------|
| REGULAR    | 500         |
| PREMIUM    | 750         |
| VIP        | 1000        |
| RECLINER   | 1200        |

---

## Demo Scenarios Included

- Preloaded data for Pakistani cities:
  - Karachi (Atrium Saddar, Nueplex DHA)
  - Lahore (CineStar Township, CineStar Gulberg)
  - Islamabad (Centaurus Megaplex)
- Seat booking and cancellation with validation
- Duplicate booking rejection
- Layout and detailed seat listings
- City-wide VIP seat discovery
- Independent Seat-level demo

---

## How to Run

Build the project:
```bash
build
