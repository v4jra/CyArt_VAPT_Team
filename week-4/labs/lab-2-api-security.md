# Lab 2 – API Security Testing

## Objective
This lab focused on identifying security flaws in REST and GraphQL APIs based on the OWASP API Top 10.

---

## Scope
- REST API testing
- GraphQL endpoint testing
- Authorization and authentication bypass

---

## Tools Used
- Burp Suite
- Postman
- sqlmap

---

## Enumeration
API endpoints were enumerated manually and through proxy interception. GraphQL introspection and parameter manipulation were tested.

---

## Vulnerabilities Identified

| Test ID | Vulnerability | Severity | Endpoint |
|-------|---------------|----------|----------|
| 008 | Broken Object Level Authorization (BOLA) | Critical | /api/users |
| 009 | GraphQL Misconfiguration | High | /graphql |

---

## Manual Testing
Authorization tokens were manipulated using Burp Suite, resulting in unauthorized access to protected resources.

---

## Impact
Exploitation demonstrated the ability to access or modify sensitive user data without proper authorization.

---

## Recommendations
- Enforce object-level authorization
- Disable unnecessary GraphQL introspection
- Validate access tokens on every request
