# User Registration API Documentation

## Endpoint: `/users/register`

### Method: POST

### Description
This endpoint is used to register a new user. It validates the input data, hashes the user's password, creates a new user in the database, and returns a JSON Web Token (JWT) along with the user details.

### Required Data
-`fullname` (object):
- `fullname.firstname` (string): The first name of the user. Must be at least 3 characters long.
- `fullname.lastname` (string): The last name of the user. Must be at least 3 characters long.
- `email` (string): The email address of the user. Must be a valid email format.
- `password` (string): The password for the user. Must be at least 6 characters long.


### example resoponse
- `user` (object):
- `fullname` (object).
  - `firstname` (string): user's first name must be (minimum 3 charters).
  - `lastname` (string): user's last name (minimum 3 characters).
  
  - `email` (string): user's email adress (must be valid email).
  
  - `password` (string): user's password (minimum 6 characters)
   - `token` (string): JWT Token
