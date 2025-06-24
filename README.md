This Blogging Application is a full-stack backend platform developed using Spring Boot. It provides secure user authentication, blog post creation, comment handling, and RESTful API integration with Spring Security. It is fully tested and ready for frontend integration (React/Angular).

🔐 Authentication & Security
Implemented Spring Security with JWT Token Authentication.

Users must login/register to access secured endpoints.

Role-based access control (USER, ADMIN).

Stateless session handling with secure API access.

🔧 Features & Functionality
👤 User Authentication
POST /api/auth/register – Register new users.

POST /api/auth/login – Login and get JWT token.

Uses BCryptPasswordEncoder for password hashing.

Token sent in Authorization header:
Authorization: Bearer <JWT_TOKEN>

✍️ Post Management
POST /api/posts – Create a new blog post (Authenticated).

PUT /api/posts/{id} – Update a post.

DELETE /api/posts/{id} – Delete post (only owner/admin).

GET /api/posts – List all posts with pagination and sorting.

GET /api/posts/{id} – View a single post by ID.

💬 Comment System
POST /api/posts/{postId}/comments – Add a comment.

PUT /api/comments/{commentId} – Edit a comment.

DELETE /api/comments/{commentId} – Delete a comment.

Only comment author can edit/delete.

📄 Pagination, Sorting, Filtering
GET /api/posts?page=0&size=5&sort=createdAt,desc

Response includes:

pageNumber

pageSize

totalElements

totalPages

isLastPage

Each post/comment has a unique ID and post number.

🧰 Tech Stack
Backend: Spring Boot, Spring Security, JWT, Spring Data JPA

Database: MySQL / PostgreSQL

Security: JWT, Role-based Access

Tools: Maven, Postman, Swagger UI

REST API: Fully tested endpoints# bloging-application-backend-
this is a bloging application 
