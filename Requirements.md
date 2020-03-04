[x] Implement a basic authentication middleware to use for protecting endpoints.
[x] The GET /api/things endpoint should remain public.
[x] The GET /api/things/:thing_id endpoint should be protected by basic auth.
[x] The GET /api/things/:thing_id/reviews endpoint should be protected by basic auth.
[x] The POST /api/reviews endpoint should be protected by basic auth and automatically assign a user_id.
[x] The thingful-client should store the base64 encoded credentials when the login form is submitted.
[x] The base64 encoded credentials should be sent in requests to protected endpoints.
[] If a user attempts to view the login form when they're already logged in, they should be redirected to the thing list page.
[] If a user tries to view reviews for a thing, they should be redirected to the login form page.
[x] You should implement the logout button functionality to clear the token in local storage.
[x] You should update your database seeding data to use hashed passwords. Generate the hashed passwords using bcrypt.
[] You'll also need to update your basic-auth middleware to use bcryptjs to compare the password in the basic token with the hash stored in the database.