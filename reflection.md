# Lab 5: Static Code Analysis — Reflection

## 1. What is static code analysis?
Static code analysis examines source code without executing it. It helps identify programming errors, security vulnerabilities, maintainability problems, and style violations.

## 2. What did Pylint identify?
Pylint identified missing docstrings, naming convention violations, a mutable default argument, an unused parameter, and unnecessary else statements. These issues were corrected to improve code readability and maintainability.

## 3. What did Bandit identify?
Bandit identified unsafe pickle deserialization, a shell command execution risk, and the use of a standard pseudo-random generator. The fixes replaced pickle persistence with JSON, removed the shell execution helper, and used the secrets module for the lucky draw.

## 4. What did Flake8 identify?
Flake8 identified spacing and blank-line formatting violations. The formatting was corrected to follow Python style conventions.

## 5. What did I learn?
Static analysis helps identify issues before software is deployed. Pylint improves code quality, Bandit highlights security risks, and Flake8 checks style consistency. Using all three tools makes code easier to maintain and review. However, static analysis should be combined with functional testing because clean reports do not guarantee that every program behavior is correct.

## 6. Final results
Pylint: 10.00/10.
Bandit: No issues identified.
Flake8: No style violations reported.
