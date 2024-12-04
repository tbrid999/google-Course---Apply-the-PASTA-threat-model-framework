# google-Course---Apply-the-PASTA-threat-model-framework

Stage I: Business Objectives
The app should meet specific business needs while ensuring security and privacy. Based on the scenario:

Objective 1: Allow seamless communication between buyers and sellers with a focus on user experience (e.g., direct messaging, smooth checkouts).
Objective 2: Prioritize user data privacy and ensure proper payment handling to avoid legal issues.
Objective 3: Encourage trust by maintaining a secure and efficient platform for transactions.
Stage II: Technology Requirements
Evaluate the app's technologies for potential risks:

Priority Technology: Public Key Infrastructure (PKI)
Reason: PKI handles encryption for sensitive data (credit cards, communication). Any misconfiguration could lead to data breaches.
Secondary Technology: Structured Query Language (SQL)
Reason: SQL is crucial for data storage and retrieval. SQL injection attacks could compromise user data and disrupt operations.
Stage III: Data Handling Analysis
Analyze data flow processes and identify security needs:

Data is inputted by users for account creation, transactions, and communication.
Sensitive data like payment information and passwords are encrypted using AES, RSA, and hashed via SHA-256.
SQL queries fetch and store data related to products and user accounts.
Stage IV: Potential Threats
Threat 1: Man-in-the-Middle (MitM) Attack
A threat actor intercepts data between the app and server, compromising user credentials or financial information.
Threat 2: SQL Injection
Malicious actors exploit vulnerable SQL queries to access or manipulate the database.
Stage V: System Vulnerabilities
Vulnerability 1: Weak API Authentication
If APIs lack robust authentication mechanisms, they may expose endpoints to unauthorized access.
Vulnerability 2: Improper Input Validation
Failing to sanitize user input could leave the app vulnerable to injection attacks.
Stage VI: Attack Tree
Root Node: Access user payment data.
Branch 1: Exploit weak encryption.
Branch 2: Inject malicious SQL code into vulnerable forms.
Branch 3: Bypass API authentication to retrieve sensitive information.
Stage VII: Security Controls
Implement Multi-Factor Authentication (MFA)
To ensure only authorized users access accounts and data.
Encrypt All Data at Rest and In-Transit
Use AES for sensitive data and enforce secure TLS connections.
Use Input Validation and Parameterized Queries
Prevent SQL injection and ensure input data is sanitized.
Conduct Regular Penetration Testing and Audits
Identify and mitigate vulnerabilities in real time.
This analysis addresses business objectives, technical requirements, potential threats, vulnerabilities, and mitigation strategies to secure the app. It provides a comprehensive roadmap for securing the sneaker app using the PASTA framework.
