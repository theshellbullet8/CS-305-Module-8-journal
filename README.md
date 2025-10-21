# CS-305-Module-8-journal

1. Client Summary

The client, Artemis Financial, is a consulting company that develops personalized financial plans for its customers. These plans include retirement strategies, investment management, savings plans, and insurance solutions. Artemis Financial wanted to modernize its web application to ensure secure data communication and file integrity verification. The company’s main concern was protecting sensitive client and financial data by adding secure communication mechanisms, such as HTTPS and checksum verification, to prevent tampering or unauthorized access.

2. Security Vulnerabilities and Importance of Secure Coding

I identified and analyzed the security vulnerabilities in the existing Artemis Financial application using the OWASP Dependency Check tool. I did well at reviewing the dependency report and suppressing false positives while retaining visibility of legitimate risks.
Coding securely is essential because even small vulnerabilities in dependencies or configurations can lead to data breaches, financial loss, or reputational damage. By applying secure coding practices, companies like Artemis Financial gain customer trust, reduce risks, and ensure regulatory compliance — all of which strengthen the organization’s overall well-being.

3. Challenges in Vulnerability Assessment

The most challenging part of the vulnerability assessment was distinguishing between true vulnerabilities and false positives in the OWASP dependency-check results. Some libraries, such as Spring Boot and Tomcat, had known vulnerabilities with no immediate fixes, requiring configuration of a suppression file rather than code changes. This process was also helpful because it taught me how to properly interpret and manage security scan results in a real-world environment.

4. Increasing Layers of Security

To increase layers of security, I implemented HTTPS communication, self-signed certificate generation, and a cryptographic hash checksum verification feature. These layers ensure that transmitted data is encrypted, authenticated, and verified for integrity.
In the future, I would continue using tools like OWASP Dependency Check, SonarQube, and Static Application Security Testing (SAST) platforms to assess vulnerabilities and select appropriate mitigation techniques.

5. Verifying Functionality and Security

After refactoring the code, I ensured the application remained both functional and secure by testing the HTTPS endpoint at https://localhost:8443/hash and verifying checksum output. I reran the dependency check to confirm that no new vulnerabilities were introduced. This verification ensured that the code maintained both functionality and security after the enhancements.

6. Tools, Resources, and Practices Used

I used several tools and practices to complete this project successfully:

OWASP Dependency Check for vulnerability scanning

Java Keytool for generating self-signed certificates

Spring Boot for secure HTTPS implementation

Checksum verification (SHA-256) for file integrity

Maven for dependency management and build automation
These tools will continue to be valuable for future development and security projects.

7. Example of Work for Employers

For future employers, I would showcase this project because it demonstrates secure coding, vulnerability analysis, and DevSecOps integration. It highlights my ability to work with real-world security tools, manage certificates, implement encryption, and ensure that web applications meet modern security standards. This project is an excellent example of applying both software engineering and cybersecurity principles to create a secure and functional product.
