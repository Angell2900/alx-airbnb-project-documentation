# Airbnb Clone - Backend Requirements

## 1. User Authentication
- API Endpoints:
  - POST /api/users/register
  - POST /api/users/login
- Input: username, email, password
- Output: success/failure, auth token
- Validation: email format, password ≥ 8 characters
- Performance: response < 500ms

## 2. Property Management
- API Endpoints:
  - POST /api/properties/add
  - PUT /api/properties/update
  - DELETE /api/properties/delete
- Input: property details (name, location, price)
- Output: success/failure, property ID
- Validation: required fields, price > 0
- Performance: response < 1s

## 3. Booking System
- API Endpoints:
  - POST /api/bookings/create
  - DELETE /api/bookings/cancel
- Input: user ID, property ID, booking dates
- Output: booking confirmation or cancellation
- Validation: date availability, no overlapping bookings
- Performance: response < 1s
