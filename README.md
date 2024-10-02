# Red-Teaming and Penetration Testing for Vulnerable Web Applications and Networks

This project details a red-teaming exercise involving password cracking, brute-force attacks, and vulnerability assessment. The focus is on exploiting weaknesses in web applications and network services to gain unauthorized access, followed by recommendations to mitigate these vulnerabilities.

## Project Overview:
The project includes several key areas:
- **Password Cracking**: Cracking SHA-256 and SHA-1 hashed passwords using dictionary and brute-force attacks.
- **Web Application Attacks**: Using tools like **Hydra** to brute-force login credentials on vulnerable web apps.
- **File Manipulation Malware**: Demonstrating how a script replicates its code to other files, mimicking a virus.
- **Vulnerability Assessment**: Performing network scans and assessing vulnerabilities in services like FTP, Telnet, SMTP, SMB, and VNC on a target system (Metasploitable2).

## Key Sections:
### 1. Password Cracking:
- Implemented a script that reads passwords from a dictionary, calculates their hashes, and attempts to crack them. The project includes cracking SHA-256 hashed passwords with varying complexities.
- **Tools Used**: Python script, Hashcat, rockyou.txt dictionary.

### 2. Brute-Force Attacks on Web Applications:
- Using **Hydra**, a brute-force tool, to crack login credentials on a vulnerable web application (DVWA). The attack emulates how red-teamers can exploit weak credentials to gain unauthorized access.
  
### 3. Malware Analysis and File Manipulation:
- Demonstrating file manipulation malware that infects Python scripts by injecting its own code into them, simulating a virus attack.
  
### 4. Vulnerability Assessment and Exploitation:
- Performed a **vulnerability scan** on Metasploitable2 using **Nmap** and identified services running on ports such as FTP, Telnet, SMTP, SMB, and VNC.
- Exploited identified vulnerabilities (e.g., anonymous FTP access, Telnet clear text transmission, weak VNC passwords) using **Metasploit**.
- Provided detailed recommendations to mitigate the risks associated with these vulnerabilities.

## Tools and Technologies:
- **Hashcat**: For cracking SHA-1 and SHA-256 password hashes.
- **Hydra**: Used for brute-force login attempts on web applications.
- **Metasploit**: For exploiting vulnerabilities in network services.
- **Nmap**: For scanning and identifying open ports on target systems.
- **Python**: Custom scripts for password cracking and file manipulation malware demonstration.

## Key Findings:
1. **Weak Passwords**: The cracking process showed that weak passwords were highly susceptible to dictionary attacks, highlighting the need for stronger password policies.
2. **Insecure Services**: Vulnerabilities in services like Telnet (clear text credentials) and FTP (anonymous access) pose significant risks.
3. **File Manipulation Malware**: Malware that infects other files could lead to severe security breaches if not contained.

## Recommendations:
- Enforce **strong password policies** and use salted hashes to prevent password cracking.
- Replace vulnerable services like **Telnet** with more secure alternatives such as SSH.
- Regularly update and patch services like FTP and SMB to mitigate known vulnerabilities.
- Implement **network segmentation** and **monitoring** to limit lateral movement and detect suspicious activity.

## Conclusion:
This red-teaming exercise demonstrated various techniques used by attackers to exploit web applications and network vulnerabilities. By understanding these attack vectors, organizations can take steps to improve their security posture and protect against unauthorized access and malware infections.

---

### Author:
- **Ali Abdelhamid**  
  Email: Aa2100274@tkh.edu.eg
