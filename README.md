# CS-305-Software-Security

## Briefly summarize your client, Artemis Financial, and its software requirements. Who was the client? What issue did the company want you to address?
Artemis Financial is a financial planning consultancy that needed to enhance security for their client web portal. As their development partner, we were tasked with addressing two critical issues which are implementing checksum verification to ensure file integrity during data transfers and upgrading all communications from HTTP to HTTPS to protect sensitive financial information from interception. Their primary concern was safeguarding client data while maintaining system performance.

## What did you do well when you found your client’s software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall well-being?
During the vulnerability assessment, I excelled at identifying cryptographic weaknesses and recommending appropriate solutions. I successfully matched security controls to specific risks, implementing SHA-256 for data verification and TLS for secure transport. Secure coding is essential because vulnerabilities can lead to data breaches, regulatory penalties and loss of customer trust. For Artemis Financial, robust security directly protects their reputation in the financial sector and ensures compliance with strict data protection laws.

## Which part of the vulnerability assessment was challenging or helpful to you?
The most valuable yet challenging aspect was analyzing dependency vulnerabilities. While time-consuming, tracing library dependencies helped uncover hidden risks in third-party components. This process revealed how outdated libraries could undermine even well-secured custom code, emphasizing the importance of comprehensive dependency management in security planning.

## How did you increase layers of security? In the future, what would you use to assess vulnerabilities and decide which mitigation techniques to use?
Security was enhanced through defense-in-depth measures: checksum validation for data integrity, HTTPS encryption for secure transport and input sanitization to prevent injection attacks. For future assessments, I would use OWASP ZAP for dynamic scanning alongside static analysis tools, creating a more complete vulnerability profile to guide mitigation strategies based on risk severity and business impact.
    
## How did you make certain the code and software application were functional and secure? After refactoring the code, how did you check to see whether you introduced new vulnerabilities?
Post-refactoring verification involved multiple test layers such as unit tests for checksum functionality, integration tests for HTTPS enforcement and dependency scans to detect new issues. The OWASP Dependency-Check tool was particularly valuable for identifying whether our changes inadvertently introduced vulnerable components, while manual code reviews ensured no logical flaws were created during modifications.
 
## What resources, tools, or coding practices did you use that might be helpful in future assignments or tasks?
Key tools included OWASP Dependency-Check for vulnerability scanning, Postman for API security testing and Spring Security for implementation. The practice of conducting threat modeling during design and maintaining a security checklist throughout development proved extremely valuable, approaches I'll definitely reuse. NIST's cryptographic guidelines provided reliable standards for our encryption implementations.

## Employers sometimes ask for examples of work that you have successfully completed to show your skills, knowledge, and experience. What might you show future employers from this assignment?
For future employers, I would showcase the before-and-after security analysis reports demonstrating identified risks and implemented solutions. The refactored code samples with SHA-256 implementation and HTTPS configuration would highlight technical skills, while the testing documentation would illustrate rigorous verification processes. Most importantly, I'd present the measurable security improvements achieved through these changes.
