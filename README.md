# Freelancing Service Platform - Backend

A Spring Boot REST API backend for a freelancing service platform that connects customers with tech experts.

## Features

- Customer and Tech Expert registration and login
- Role-based user management
- JWT-based authentication
- Service category management
- Tech Experts can create and manage services
- Customers can browse available services
- Customers can submit service requests
- Tech Experts can review service requests
- Tech Experts can send service proposals
- Customers can approve or deny expert proposals
- Customer wallet management
- Razorpay payment integration
- Service request status tracking
- User profile management
- RESTful APIs
- MySQL database integration

## Tech Stack

### Backend

- Java
- Spring Boot
- Spring Security
- Spring Data JPA
- Maven
- REST APIs
- JWT Authentication

### Database & Services

- MySQL
- Razorpay Payment Gateway

## Project Structure

```text
src/
├── main/
│   ├── java/com/freelancing/
│   │   ├── dao/
│   │   ├── dto/
│   │   ├── entity/
│   │   ├── exception/
│   │   ├── filter/
│   │   ├── interceptor/
│   │   ├── pg/
│   │   ├── service/
│   │   ├── utility/
│   │   └── FreelancingBackendApplication.java
│   │
│   └── resources/
│       ├── application.properties
│       └── log4j2-spring.xml
│
└── test/
    └── java/com/freelancing/
        └── FreelancingBackendApplicationTests.java
```

## Running the Project Locally

### 1. Start the Backend

On Windows, run:

```bash
.\mvnw spring-boot:run
```

The backend will run at:

```text
http://localhost:8080
```

## Application Flow

```text
Customer
   ↓
Register / Login
   ↓
Browse Services
   ↓
Request Service
   ↓
Tech Expert Reviews Request
   ↓
Expert Sends Proposal
   ↓
Customer Approves / Denies
   ↓
Service Request Status Updated
```

## Payment Flow

```text
Customer
   ↓
Add Money to Wallet
   ↓
Razorpay Payment Gateway
   ↓
Payment Confirmation
   ↓
Wallet Balance Updated
   ↓
Customer Can Approve Expert Proposal
```

## API Modules

The backend provides REST APIs for:

- User authentication
- User registration
- User profile management
- Service management
- Service categories
- Service requests
- Expert proposals
- Wallet management
- Payment processing

## Author

Utkarsh Upadhyay
