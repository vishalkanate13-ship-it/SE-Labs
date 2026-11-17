@'
# Lab 5: Static Code Analysis Reflection

## 1. What is the purpose of static analysis?
Static analysis examines source code without executing it. Pylint checks code quality, Bandit checks for potential security issues, and Flake8 checks style and formatting.

## 2. What important issues did you find?
The analysis identified an unsafe shell command, unsafe XML parsing, a hard-coded password, a mutable default argument, naming problems, and formatting violations.

## 3. How did you fix and verify the issues?
I removed the unnecessary shell-command helper and hard-coded password, switched to defusedxml, corrected the mutable default argument, improved naming and documentation, and fixed formatting. I reran all three tools to verify the results.

## 4. How will you use static analysis in the future?
I will run static-analysis tools regularly before committing code to help catch security risks, maintainability problems, and formatting issues early.
'@ | Set-Content -Encoding utf8 reflection.md