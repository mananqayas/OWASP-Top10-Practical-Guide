# Fixing Broken Access Control
Here are the strategies to fix broken access control:

1. **Implement Propert Access Policies**
- Use **role-based access control (RBAC)** or **attribute-based access control (ABAC)**.
- Enforce **principle of least privilege** (users should only have the necessary access).
2. **Server-Side Authorization**
- Always enforce access control checks on the server, not just on the client.
- Validate user permissions for each request.
3. **Secure Direct Object References**
- User **random or hased IDs** instead of sequential ones.
- Check if the authenticated user has permission before serving the resource.
4. **Enforce Session Expiry & Logout Mechanisms**
- User **short-lived sessions** and re-authentication for sensitive operations.
5. **Restrict API Access**
- Use **(OAuth, JWT, API Keys)** for authentication.
- Implement **rate limiting** and **monitor API logs** for suspicious activities.
6. **Security Testing & Audits**
- Perform **regular penetration testing**.
- Use **automated security scanning tool**.
- Conduct **code reviews** to identify improper access controls.

## Demo

After implementing mitigation strategies on both frontend and backend API, our application is not working

### Run the docker compose file

Using the docker compose command run:

`docker compose up`

*docker-compose file is in the same directory.*

Vist the frontend app at:

[http://localhost:5173/](http://localhost:5173/)

![](/Broken_Access_Control/Fixed_Broken_Access_Control/download.gif)