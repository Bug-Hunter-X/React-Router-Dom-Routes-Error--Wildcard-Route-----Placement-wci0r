# React Router Dom Routes Error: Wildcard Route '*' Placement

This repository demonstrates a common error in React Router Dom v6 when using the wildcard route `*`.  The issue arises when the wildcard route is not placed as the last route within the `<Routes>` component.

Placing the wildcard route before other routes prevents those routes from ever being matched. This is because the wildcard route matches any path.

**How to reproduce:**
1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Navigate to `/about`. You'll find that the NotFound component renders instead of the About component.

**Solution:**
Move the wildcard route to the end of your route definitions within the `<Routes>` component.