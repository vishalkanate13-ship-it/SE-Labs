
# Lab 5: Static Code Analysis — Issue Log

| Issue | Type | Line(s) | Description | Fix Approach |
|---|---|---|---|---|
| Missing docstrings | Code quality | Multiple | Module and functions lacked documentation. | Added module and function docstrings. |
| Invalid naming conventions | Style | Multiple | Functions and variables used camelCase. | Renamed them using snake_case. |
| Mutable default argument | Bug | 42 | extras={} could share mutable state between calls. | Changed the default to None and initialized a new dictionary. |
| Unused parameter | Code quality | 50 | currency was accepted but never used. | Removed the parameter and updated the function call. |
| Unsafe shell command | Security | 63 | os.system constructed a shell command using meterIp. | Removed the unused helper and os import. |
| Unsafe XML parsing | Security | 3, 18 | Standard-library XML parsing was flagged by Bandit. | Switched to defusedxml.ElementTree. |
| Hard-coded password | Security | 13 | A password string was embedded in the source. | Removed the unused constant. |
| Unspecified file encoding | Code quality | 57 | open() did not specify an encoding. | Added encoding="utf-8". |
| Formatting violations | Style | 22, 44, 72, 76 | Flake8 reported blank-line, whitespace, and line-length issues. | Corrected spacing and line formatting. |
