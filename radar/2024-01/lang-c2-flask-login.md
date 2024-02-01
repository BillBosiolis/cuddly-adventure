---
title:      "Flask-Login"
ring:       trial
quadrant:   languages-and-frameworks
tags:       [server]
---

Flask-Login is an extension for Flask that provides user session management. It handles the common tasks of logging in, logging out, and remembering users' sessions over extended periods of time.

Flask-Login keeps track of the logged in user by storing its unique identifier in Flask's user session, a storage space assigned to each user who connects to the application. Each time the user navigates to a new page, Flask-Login retrieves the ID of the user from the session, and then loads that user into memory.

Beyond these basic features, Flask-Login provides other functionality such as "remember me" functionality, anonymous user sessions, and user session expiration.

### Usages
