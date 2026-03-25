# sql-injection-dvwa-lab
Overview

This lab demonstrates the exploitation of SQL Injection vulnerabilities using a deliberately vulnerable web application. The objective is to understand how improper input validation can lead to unauthorized data access and authentication bypass.

⸻

 Objectives
	•	Identify SQL Injection vulnerability
	•	Extract data from the database
	•	Perform authentication bypass
	•	Understand the impact and mitigation techniques

⸻

Lab Environment
	•	Attacker Machine: Kali Linux
	•	Target Application: Damn Vulnerable Web Application
	•	Web Server: Apache2
	•	Database: MariaDB
	•	Browser: Firefox

⸻

 Setup
	1.	Installed DVWA on Kali Linux
	2.	Configured Apache and MariaDB services
	3.	Created and initialized the DVWA database
	4.	Set DVWA security level to Low

⸻

 Methodology

1. Basic Input Test
	•	Input: 1
	•	Result: Returned a single user record

⸻

2. SQL Injection (Data Extraction)
	•	Payload:1' OR '1'='1
Result:
	•	Retrieved multiple user records from the database
	•	Demonstrated improper input sanitization

⸻

3. SQL Injection (Authentication Bypass)
	•	Username:admin' OR '1'='1
	•	Password: anything	•	Result:
	•	Successfully logged in without valid credentials
	•	Demonstrated complete authentication bypass



Vulnerability Details
	•	Type: SQL Injection
	•	Severity: Critical
	•	Impact:
	•	Unauthorized data access
	•	Authentication bypass
	•	Potential full system compromise

⸻

 Mitigation Strategies
	•	Use prepared statements (parameterized queries)
	•	Implement input validation and sanitization
	•	Apply least privilege principle to database users
	•	Use Web Application Firewalls (WAFs)

⸻

 Key Learnings
	•	SQL Injection is caused by unsanitized user input
	•	Even simple inputs can compromise a system
	•	Secure coding practices are essential in web applications

⸻

Author
Ibrahim M.
Cybersecurity Enthusiast
