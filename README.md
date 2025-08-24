# Artemis Financial – Secure Software Project (CS 305)

This repository includes my final project for CS 305, where I worked with a fictional client, Artemis Financial, to improve the security of their Java-based web application. The artifact I’ve chosen to include is the completed **Practices for Secure Software Report** from Project Two.

## Reflection

**Who was the client, and what did they need?**  
Artemis Financial is a consulting company that provides financial planning services. They wanted to modernize their public-facing application and ensure secure data transmission. My role was to identify vulnerabilities and improve the security of their software.

**What did I do well?**  
I was able to properly configure HTTPS communication, generate and apply a cryptographic hash for data verification, and use OWASP's Dependency-Check tool to identify and suppress known vulnerabilities. Coding securely is essential because it helps protect sensitive client data and builds trust.

**What was challenging or helpful during the assessment?**  
Configuring the `suppression.xml` file was the most challenging part. Making sure the schema and syntax were correct took time and careful troubleshooting. However, learning how to properly suppress only false positives was valuable.

**How did I increase layers of security?**  
I implemented SSL using a self-signed certificate, switched the server to HTTPS, and added a checksum verification mechanism. In the future, I’d use automated static testing tools and manual reviews to assess vulnerabilities and choose appropriate mitigations.

**How did I confirm the code was functional and secure?**  
I ran the application locally and tested it through `https://localhost:8443/hash` to verify it was running securely. I also re-ran the dependency-check scan to ensure no new vulnerabilities were introduced after refactoring.

**What tools and practices were helpful?**  
- OWASP Dependency-Check (Maven plugin)  
- Java Keytool for certificate generation  
- Spring Boot for secure application development  
- Manual code review and checksum implementation

**What could I show an employer from this assignment?**  
This project demonstrates that I can take an insecure application and apply multiple layers of security, validate functionality, and document my process clearly. It shows my ability to implement best practices and use industry tools in real-world scenarios.
