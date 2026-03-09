
 **TASK 3** — Secure Coding Review

**Programming Language and Application Selected**

The programming language used for this task is Python.
The application reviewed is a simple login system (login.py) that accepts a username and password from the user and checks them against stored credentials.

**Code Review Findings**

**Identified Vulnerabilities*

**1. Hardcoded Credentials**
The username and password are written directly in the source code, making them easy to discover and insecure.

**2. Weak Authentication Mechanism**
The program compares plain-text credentials without hashing or encryption.

**3. Insecure Input Handling**
User inputs are not validated or sanitized, which may lead to security risks.

**Tools Used**

*Manual code inspection
*Bandit (static analyzer) — used to detect security issues in the Python code.

**Recommendations and Best Practices**

*Avoid hardcoding sensitive information.
*Use password hashing (e.g., bcrypt).
*Store credentials securely in a database.
*Validate and sanitize all user inputs.
*Follow secure coding standards.

**Evidence (Screenshots Included)**

screenshot1_code.png — Code review
screenshot2_run.png — Program execution
screenshot3_bandit.png — Static analysis result

screenshot2_run.png — Program execution

screenshot3_bandit.png — Static analysis result
