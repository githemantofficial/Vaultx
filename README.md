# Vaultx
Secure file management platform built with Spring Boot, PostgreSQL, AWS S3, JWT authentication, and Docker.


VaultX is a secure file management platform that allows authenticated users to upload, manage, and share files through a REST API.

The backend is built with Java 21 and Spring Boot 3, with PostgreSQL used for user and file metadata and AWS S3 used for storing the actual files. Authentication and authorization are handled using Spring Security and JWT.

Features
User authentication and authorization
JWT-based security
File upload and deletion
File metadata management
AWS S3 file storage
File sharing
RESTful APIs
Input validation and global exception handling
Swagger/OpenAPI documentation
Unit testing with JUnit and Mockito
Docker support
Tech Stack
Technology	Purpose
Java 21	Backend development
Spring Boot 3	REST API and application framework
Spring Security	Authentication & authorization
JWT	Stateless authentication
PostgreSQL	Database and file metadata
AWS S3	File storage
JPA / Hibernate	Database interaction
Maven	Build & dependency management
Docker	Containerization
Swagger / OpenAPI	API documentation
JUnit & Mockito	Testing
Architecture
Client
  |
  | REST API
  v
Spring Boot
  |
  +-- Spring Security + JWT
  +-- Controller
  +-- Service
  +-- Repository
  |
  +----------+-----------+
  |                      |
  v                      v
PostgreSQL              AWS S3
Metadata                Actual Files

PostgreSQL stores users, roles, file metadata, and shared-link information, while the actual files are stored in AWS S3.

API Documentation

Swagger/OpenAPI is used to document and test the REST APIs.

When running locally:

http://localhost:8080/swagger-ui
Running Locally
Prerequisites
Java 21
Maven
PostgreSQL
AWS account with an S3 bucket
Docker (optional)
