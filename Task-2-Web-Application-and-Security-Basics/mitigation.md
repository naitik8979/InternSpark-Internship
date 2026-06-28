# Mitigation Recommendations

## SQL Injection

**Vulnerability:**
The application was vulnerable to SQL Injection because user input was directly included in SQL queries without proper validation.

**Recommendations:**

* Use prepared statements (parameterized queries).
* Validate and sanitize all user inputs.
* Apply server-side input validation.
* Use least-privilege database accounts.
* Avoid exposing database error messages to users.

---

## Cross-Site Scripting (Reflected XSS)

**Vulnerability:**
The application executed user-supplied JavaScript without proper input sanitization or output encoding.

**Recommendations:**

* Validate and sanitize all user inputs.
* Encode output before displaying it in web pages.
* Implement a Content Security Policy (CSP).
* Use secure frameworks that automatically escape user-generated content.
* Set HTTP security headers where appropriate.

---

## Burp Suite Usage

Burp Suite was used as an intercepting proxy to capture and inspect HTTP requests and responses between the browser and the DVWA application. It helped analyze request parameters, observe application behavior, and verify the presence of SQL Injection and Reflected XSS vulnerabilities.

---

## Conclusion

This task provided practical experience in identifying common web application vulnerabilities and understanding how attackers exploit insecure input handling. It also reinforced the importance of secure coding practices, input validation, output encoding, and regular security testing to protect web applications from common attacks.

