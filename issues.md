
# Lab 5: Static Code Analysis — Issue Log

| Tool | Issue | Type | Original line(s) | Fix applied |
|---|---|---|---|---|
| Pylint | Missing module and function docstrings | Code quality | 1, 9, 15, 27, 32, 39, 44, 49, 54 | Added module and function docstrings. |
| Pylint | Function and argument names not in snake_case | Naming convention | 9, 15, 27, 32, 39, 44, 49, 54 | Renamed functions and parameters using snake_case. |
| Pylint | Mutable default argument | Potential bug | 9 | Replaced the empty-list default with None and initialized a new list. |
| Pylint | Unused parameter | Code quality | 39 | Removed the unused sortOrder parameter. |
| Bandit | Unsafe pickle deserialization | Security | 2, 51 | Replaced pickle persistence with JSON. |
| Bandit | Shell command constructed from user-controlled text | Security | 56 | Removed the os.system() helper. |
| Bandit | Standard random generator used for the lucky draw | Security practice | 72 | Replaced random.choice() with secrets.choice(). |
| Flake8 | Missing whitespace and incorrect spacing | Style | 61, 66, 75 | Corrected whitespace and inline comment formatting. |
| Flake8 | Incorrect blank-line spacing | Style | 79 | Corrected function spacing. |

## Verification

After applying the fixes, Pylint reported 10.00/10.
Bandit reported no issues.
Flake8 reported no style violations.
