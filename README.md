# SafeVault – Secure Application

## Project Overview

SafeVault is a secure web application developed using C# and ASP.NET Core. The project demonstrates secure coding practices, user authentication, authorization, input validation, and protection against common web application vulnerabilities.

The main objective is to protect user information and prevent security threats such as SQL Injection and Cross-Site Scripting (XSS).

## Project Objectives

- Implement secure input validation.
- Prevent SQL Injection attacks.
- Implement user authentication.
- Apply Role-Based Access Control (RBAC).
- Identify and resolve security vulnerabilities.
- Generate and execute automated security tests.
- Use Microsoft Copilot to assist with secure coding and debugging.

## Technologies Used

- C#
- ASP.NET Core
- SQL Server / SQLite
- Microsoft Copilot
- Visual Studio
- Git and GitHub
- NUnit / xUnit

## Security Features

### 1. Input Validation

The application validates user input before processing it.

- Checks required fields.
- Validates username and email formats.
- Rejects unexpected input.
- Applies appropriate input sanitization.

### 2. SQL Injection Prevention

Parameterized SQL queries are used to prevent malicious input from changing database commands.

All database queries should use secure parameter handling rather than direct string concatenation.

### 3. Authentication

The application implements secure authentication features:

- User registration.
- User login.
- Password hashing.
- Credential verification.
- Protected user sessions.

### 4. Authorization and RBAC

Role-Based Access Control ensures that users can only access resources permitted by their assigned roles.

The application supports:

- Administrator access.
- Regular user access.
- Restricted access to protected resources.

### 5. Cross-Site Scripting (XSS) Prevention

The application uses input validation and output encoding to protect against malicious scripts submitted through user input.

### 6. Security Testing

Automated security tests are used to verify:

- Input validation.
- SQL Injection prevention.
- XSS protection.
- Authentication functionality.
- Authorization permissions.
- Role-based access restrictions.

## Vulnerabilities Identified and Fixes Applied

| Vulnerability | Fix Applied |
|---|---|
| SQL Injection | Parameterized SQL queries |
| Cross-Site Scripting | Input handling and output encoding |
| Weak Password Storage | Secure password hashing |
| Unauthorized Access | Authentication checks |
| Privilege Escalation | Role-Based Access Control |

## Microsoft Copilot Assistance

Microsoft Copilot was used as a development assistant throughout the project.

It assisted with:

1. Generating secure input validation code.
2. Suggesting parameterized SQL queries.
3. Implementing authentication and authorization.
4. Developing Role-Based Access Control.
5. Identifying potential SQL Injection and XSS vulnerabilities.
6. Suggesting security test cases.
7. Debugging and improving application code.

Copilot-generated suggestions were reviewed and tested before implementation.

## Running the Project

### Prerequisites

- Visual Studio.
- .NET SDK.
- Git.
- Required project dependencies.

### Build the application

```bash
dotnet restore
dotnet build
```

### Run the application

```bash
dotnet run
```

Open the local URL displayed in the terminal.

### Run security tests

```bash
dotnet test
```

## Project Structure

```text
SafeVault/
│
├── SafeVault/
│   ├── Controllers/
│   ├── Models/
│   ├── Services/
│   ├── Security/
│   ├── Data/
│   └── Program.cs
│
├── SafeVault.Tests/
│   ├── InputValidationTests.cs
│   ├── SqlInjectionTests.cs
│   ├── AuthenticationTests.cs
│   ├── AuthorizationTests.cs
│   └── XssTests.cs
│
├── README.md
├── SECURITY_SUMMARY.md
└── .gitignore
```

*The folder structure should be adjusted to match the actual project files.*

## Conclusion

The SafeVault project demonstrates the importance of secure software development. Through input validation, SQL Injection prevention, authentication, authorization, RBAC, and security testing, the application aims to protect user data and improve application security.

Microsoft Copilot supported the development and debugging process by providing suggestions for secure coding practices and vulnerability remediation.

## Author

SafeVault Security Project

## License

This project is intended for educational purposes.
