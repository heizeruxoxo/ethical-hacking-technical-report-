# Ethical Hacking Technical Report

**Client:**Atomic Roastery &nbsp;
**Date:** May 7, 2024 &nbsp;
**Prepared by:** Hazel Anne Sanorjo

## Executive Summary:
This report presents the technical findings of the ethical hacking assessment conducted for Atomic Roastery. The assessment aimed to identify vulnerabilities within the organization's network infrastructure, applications, and systems. Through various testing methodologies, including penetration testing and vulnerability scanning, critical and high-risk issues were discovered. This report provides detailed descriptions of these findings, along with actionable recommendations for remediation.

## Vulnerability Summary:
1. **Network Infrastructure:**
   - Critical: Open SSH port (22) accessible from any external IP, potentially allowing unauthorized access to sensitive systems.
   - High: Outdated router firmware (Netgear Nighthawk R7000) with known security vulnerabilities, leaving the network exposed to exploitation.

2. **Web Applications:**
   - Critical: Lack of input validation in the login form of the web application, making it vulnerable to SQL Injection attacks.
   - High: Missing secure flag in session cookies, exposing users to session hijacking attacks.

3. **Operating Systems:**
   - Critical: Unpatched Windows Server 2016 systems, leaving them vulnerable to exploits such as EternalBlue (CVE-2017-0144).
   - High: Default configurations on Linux servers allowing root SSH access, increasing the risk of unauthorized access.

4. **Database:**
   - Critical: Weak database credentials (username: 'root', password: 'password123') with full administrative privileges, posing a significant security risk.
   - High: Lack of encryption for sensitive data stored in the database, making it susceptible to data breaches.

5. **Social Engineering:**
   - High: Employees easily tricked into revealing sensitive information over the phone during simulated phishing calls.

6. **Database Security:**
   - *Critical:* Lack of encryption at rest and in transit for sensitive database data, exposing it to unauthorized access.
   - *High:* Default credentials left unchanged on the database management system, allowing easy access to attackers.

7. **Email Security:**
   - *Critical:* Absence of DMARC (Domain-based Message Authentication, Reporting, and Conformance) policy, leaving the organization vulnerable to email spoofing and phishing attacks.
   - *High:* No email filtering in place, increasing the likelihood of malicious emails reaching employees' inboxes.

8. **Cloud Infrastructure:**
   - *Critical:* Misconfigured access control policies in the cloud environment, leading to unauthorized access to sensitive data stored on cloud servers.
   - *High:* Lack of activity monitoring and logging in the cloud environment, hindering the detection of suspicious behavior.

9. **Mobile Applications:**
   - *Critical:* Insecure data storage on mobile devices, allowing sensitive data to be accessed if the device is compromised.
   - *High:* Lack of secure communication channels between the mobile application and backend servers, making it susceptible to man-in-the-middle attacks.

10. **Physical Security:**
    - *Critical:* Weak physical access controls, such as easily duplicable keys or lack of badge access, compromising the security of physical assets.
    - *High:* Absence of surveillance cameras in critical areas, hindering the investigation of security incidents and breaches.


## Recommendations:
1. **Network Infrastructure:**
   - Close unnecessary open ports and restrict SSH access to specific IP ranges.
   - Update router firmware to the latest version to address known security vulnerabilities.

2. **Web Applications:**
   - Implement input validation mechanisms to prevent SQL Injection attacks.
   - Enable the secure flag for session cookies to mitigate session hijacking risks.

3. **Operating Systems:**
   - Apply security patches regularly to keep systems up to date and protected against known vulnerabilities.
   - Disable root SSH access and use individual user accounts with limited privileges.

4. **Database:**
   - Change database credentials to strong, complex passwords and restrict privileges based on the principle of least privilege.
   - Implement encryption mechanisms such as Transparent Data Encryption (TDE) to protect sensitive data at rest.

5. **Social Engineering:**
   - Conduct regular security awareness training sessions to educate employees about the risks of social engineering attacks and how to identify and respond to them effectively.

6. **Database Security:**
   - Implement encryption mechanisms for sensitive data both at rest and in transit.
   - Change default credentials on the database management system and enforce strong password policies.

7. **Email Security:**
   - Implement DMARC policy to prevent email spoofing and phishing attacks.
   - Deploy email filtering solutions to block malicious emails before they reach employees' inboxes.

8. **Cloud Infrastructure:**
   - Review and update access control policies in the cloud environment to restrict access to authorized personnel only.
   - Enable activity monitoring and logging in the cloud environment to detect and respond to suspicious activities.

9. **Mobile Applications:**
   - Encrypt sensitive data stored on mobile devices and implement secure storage practices.
   - Implement secure communication protocols, such as HTTPS, for communication between the mobile application and backend servers.

10. **Physical Security:**
    - Strengthen physical access controls by implementing biometric authentication or keycard access.
    - Install surveillance cameras in critical areas to monitor and record physical access activities.

## Conclusion:
The findings of the ethical hacking assessment highlight several critical vulnerabilities and security weaknesses within Atomic Roastery's infrastructure and applications. By implementing the recommended remediation measures, Atomic Roastery can significantly enhance its security posture and mitigate the risk of cyber threats and data breaches.

**Signature:** [Hazel Anne C.Sanorjo] 
