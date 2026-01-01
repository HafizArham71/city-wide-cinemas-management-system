# City Cinema Management System (Java, Arrays Only)

A city-wide cinema management system built from scratch in Java using only arrays.  
This project models real-world cinema operations while strictly avoiding Java Collections, focusing on clean object-oriented design, encapsulation, and multi-class collaboration.

The system manages multiple cities, cinemas, screens, and seats, and supports booking, cancellation, reporting, and seat discovery.

---

## Why This Project Matters

Most student projects rely heavily on Java Collections.  
This project intentionally avoids them to demonstrate strong fundamentals, clear data modeling, and disciplined system design.

It shows how to:
- Design systems using primitive data structures
- Control state safely through encapsulation
- Coordinate multiple classes without frameworks

---

## Key Features

- Fully preloaded data using arrays
- Multiple Pakistani cities with realistic cinema names
- Jagged two-dimensional seat layouts
- Enum-based seat classification
- Booking and cancellation with validation
- Duplicate booking rejection
- Availability tracking and reporting
- City-wide VIP seat discovery
- Compact and detailed display outputs

---

## Core Entities

### Seat
- Human-readable seat ID (for example: 3-007)
- Enum-based type: REGULAR, PREMIUM, VIP, RECLINER
- Price derived from seat type
- Availability tracking
- Safe booking and cancellation operations
- Clear toString output

---

### Screen
- Represents a physical auditorium
- Backed by a jagged Seat two-dimensional array
- Automatically assigns seat types by row
- Prices derived from seat type
- Supports seat lookup, booking, and cancellation
- Provides layout and detailed seat displays

---

### Cinema
- Represents a cinema branch
- Manages multiple screens using arrays
- Manual array resizing where required
- Forwards seat operations to screens
- Computes cinema-level statistics
- Single-line summary via toString

---

### CityCinema
- Represents a city containing multiple cinemas
- Uses arrays only, with manual resizing
- Relays booking and cancellation across levels
- Computes city-wide aggregates
- Discovers the first available VIP seat in the city

---

## Pricing Policy

REGULAR: 500 PKR  
PREMIUM: 750 PKR  
VIP: 1000 PKR  
RECLINER: 1200 PKR  

Prices are visible in program output and derived automatically.

---

## Preloaded Cities and Cinemas

Karachi:
- Atrium Saddar
- Nueplex DHA

Lahore:
- CineStar Township
- CineStar Gulberg

Islamabad:
- Centaurus Megaplex

All data is created at startup using arrays. The program never starts empty.

---

## Demo Workflows

- Display seating layouts for each city
- Book a seat by ID
- Reject duplicate bookings correctly
- Cancel a booking and verify state changes
- Search for the first available VIP seat in a city
- Validate seat behavior independently

---

## How to Run

Build the project by typing:
build

Run the project by typing:
run

---

## Classes Included

- Seat
- Screen
- Cinema
- CityCinema
- SeatDemo
- ScreenDemo or CinemaDemo

---

## Technical Constraints

- Java Collections are not used
- Only arrays are allowed
- Manual resizing implemented where needed
- No external libraries
- No frameworks

---

## Summary

This project demonstrates:
- Core Java fundamentals
- Object-oriented design
- Data modeling without abstractions
- Discipline in constrained environments
