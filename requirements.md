1. ## User Authentication

- Endpoint: POST /api/auth/register

- Inputs: first_name, last_name, email, password

- Validations: Email format, password length > 8

- Output: JWT token

2. ## Property Management

- Endpoint: POST /api/properties

- Inputs: name, description, location, pricepernight

- Permissions: Only authenticated hosts

- Output: Created property object

3. ## Booking System

- Endpoint: POST /api/bookings

- Inputs: property_id, start_date, end_date

- Validations: Availability check, date range

- Output: Booking confirmation + total price
