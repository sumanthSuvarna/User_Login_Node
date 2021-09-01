# User_Login_Node
Senior Full Stack Developer Test

As a full stack engineer, you will be required to work on both backend applications and user
facing front end applications.

Part 1 (Backend):
Write a Node.js application that has the following APIs:
1. GET: /api/users (return list of available users)
2. POST: /api/users (create a new user). User attributes are
a. Name
b. Email (unique)
c. Password
d. Role (admin or user)
3. GET: /api/users/:id (Get a user by ID)
4. Delete: /api/users/:id (Hard delete user)
5. POST: /api/login (send login request, pass username and password, and get JWT token)

Requirement:
- Authorization is required to access the API (use JWT)
- Only user with Admin role can delete user
- Password are hashed when storing, it cannot be decrypt after hash has been done but can verify
the password. I recommend using Bcrypt or any hashing tools you like.
- Create a seed function to create an admin account with credentials of
o Email: admin@voltest.com
o Password: admin!123
o Role: admin

Tools to use:
- Expressjs
- Knexjs
- PostgressDB
- Objectionjs (for ORM)
Good to have:
- Write in Typescript
- Unit test
- CI action to run the test. You can use GitHub action

Part 2 (SPA React js)

1. Login page
2. List user page with actions (delete)
3. Create user page

Notes about SPA:
- Use basic style of your choice
- Delete features only visible to Admin role
- Use React router library to navigate from/to different pages
- Use React hook when applicable
Good to have:
- Write in Typescript
- Unit test
- CI action to run the test. You can use GitHub action
