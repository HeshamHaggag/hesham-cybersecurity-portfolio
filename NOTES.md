# SQL Injection Lab – Example Notes

Target: Demo web application (e.g. DVWA / test environment)

Performed tests:
- Identification of injectable parameters using special characters and boolean tests
- Error-based and boolean-based SQL injection checks
- Determining number of columns with `ORDER BY` and `UNION SELECT`
- Extracting example data in a controlled lab environment

Example payload (lab context only):
- `' OR '1'='1' -- `
- `' UNION SELECT NULL, @@version -- `

Reporting:
- Describe vulnerable parameter
- Show proof-of-concept payload
- Rate risk (e.g. High)
- Provide remediation: use prepared statements, parameterized queries, input validation
