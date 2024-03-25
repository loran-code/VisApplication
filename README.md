# VisApplication - Visa Application Website for Peaks of the Balkans

Welcome to VisApplication, an open-source project aimed at simplifying the visa application process for adventurers eager to explore the Peaks of the Balkans. This project is not only a tool to serve the hiking community but also a learning journey into the world of software architecture, specifically Domain-Driven Design (DDD), Clean Architecture (CA), and leveraging the capabilities of GPT and C#/.NET.

## Project Objectives
- To provide a seamless interface for users to apply for hiking visas.
- To explore and implement DDD and CA in a real-world application.
- To document the learning process and decisions in a public forum.

## Architecture Overview
The project is structured around Clean Architecture principles, ensuring our domain logic is at the core of the application's design. This approach allows us to create a system that is flexible, testable, and aligned with business goals.

## GPT Conversations

- [README](docs/gpt/0-README.md)
- [Project Setup](docs/gpt/1-project_setup.md)
- [Software Architecture and System Design](docs/gpt/2-software_architecture_and_system_design.md)

## Requirements

### Functional Requirements:

1. **User Registration and Authentication**:
    - Users must be able to register an account with the system.
    - Users must be able to authenticate with username/email and password.
    - The system should support password recovery and reset functionalities.

2. **Visa Application Submission**:
    - Provide a form for users to submit visa applications, with fields for personal details, travel information, and required documentation.
    - Validate input data for completeness and correctness.

3. **Payment Processing**:
    - Integrate a secure payment gateway for application fees.
    - Support multiple payment methods (credit/debit cards, bank transfers, etc.).
    - Provide users with payment confirmations and receipts.

4. **Application Review and Approval Workflow**:
    - Admin users must be able to review submitted applications.

5. **Status Tracking**:
    - Users should be able to track the status of their visa application in real-time.
    - Implement notifications for status updates.

6. **Help and Support System**:
    - Provide an FAQ section.

### Non-Functional Requirements:

1. **Performance**:
    - The system should handle 100 concurrent users without degradation in performance.

2. **Scalability**:
    - The system must be scalable to accommodate a growing number of users.

3. **Reliability and Availability**:
    - The system should be available with minimal downtime.

4. **Security**:
    - Adhere to best practices for data security, including encryption at rest and in transit.

5. **Maintainability**:
    - Code should be well-documented and adhere to coding standards.
    - The system should be easy to update and maintain.

6. **Usability**:
    - The user interface should be intuitive and accessible, adhering to UX/UI best practices.

7. **Testability**:
    - The system should be designed with testability in mind, with support for automated unit and integration tests.

8. **Compatibility**:
    - Ensure cross-browser compatibility and responsive design for mobile devices.

9. **Deployment**:
    - The system should support continuous integration and deployment practices.

10. **Legal and Regulatory Compliance**:
- Ensure the application complies with legal requirements, such as GDPR for users' privacy and data protection.


## Software Architecture and System Design

### Technologies:
- **Backend**: .NET Core 8 with C#12
- **Frontend**: Blazor Server

### Patterns:
- **Validation and Chain of Responsibility Pattern**: To streamline input validation and ensure each component handles its responsibility without becoming a bottleneck.
- **Decorator Pattern for Handlers**: Implement crossing concerns like logging, validation, and security in a modular way.
- **Unit of Work**: To manage database transactions, ensuring data consistency across operations.
- **CQRS (Command Query Responsibility Segregation)**: To clearly separate read and write operations, enhancing performance and scalability.
- **Outbox Pattern**: To reliably handle event dispatching and ensure eventual consistency in distributed systems.
- **Domain Events**: To facilitate communication between different parts of the application following domain-driven design principles.
- **Repository Pattern**: abstracts the data layer, providing a collection-like interface for accessing domain entities.
- **Factory Method Pattern**: Create objects without specifying the exact class of object that will be created
- **Mediator Pattern**:
 
### Libraries/Tools:
- **Entity Framework Core**: For ORM capabilities.
- **MediatR**: Simplifying in-process messaging between objects.
- **Automapper**: For efficient object-to-object mapping.
- **FluentValidation**: Define and execute validation rules.
- **Database**: Postgres
- **Logging**: Serilog

### Internal Services:
- **[Hangfire](https://www.hangfire.io/)**: Background processing
- **[MassTransit with RabbitMQ](https://masstransit.io/)**: Asynchronous message processing and inter-service communication.
- **[Authentication](https://learn.microsoft.com/en-us/aspnet/core/security/authentication/identity?view=aspnetcore-8.0&tabs=visual-studio) & [Authorization](https://learn.microsoft.com/en-us/aspnet/core/security/authorization/introduction?view=aspnetcore-8.0)**: .NET Individual Authentication, to manage user identities and permissions securely.
- **[API - Minimal API](https://minimal-apis.github.io/)**: Lightweight and fast APIs.
- **[Caching - Redis](https://redis.io/)**: Reduce database load and speed up response times for frequently accessed data.


### External Services:
- **[Payment Integration](https://www.mollie.com/en/)**: Mollie API, for handling a variety of payment services.
- **[Email Service](https://sendgrid.com/en-us)**: SendGrid, for reliable email sending capabilities.

### Testing:
- **Unit Testing**
    - **[xUnit](https://xunit.net/)**: for test definitions
    - **[Moq](https://github.com/devlooped/moq)**: for mocking dependencies.
- **Integration Testing**
    - **[MailDev](https://github.com/maildev/maildev)**: a simple way to test your project's generated email during development, with an easy to use web interface that runs on your machine built on top of Node.js
    - **[TestContainers](https://testcontainers.com/)**: Utilizing TestContainers to create ephemeral testing environments that mimic production setups.

### Version Control and CI/CD:
- **GIT**: Source code management
- **GitHub Actions**: Automate CI/CD pipelines

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.