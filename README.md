# FTP vs SFTP Security Analysis
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ohiozoje-ohikhuare-453791221/)  [![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:huare1960@gmail.com)


## Project Overview
This project demonstrates the security differences between FTP and SFTP by capturing and analyzing network traffic. The goal is to show how FTP transmits data in plaintext, while SFTP encrypts data, protecting sensitive information from interception.



## Project Objectives
- Capture FTP and SFTP traffic using Wireshark
- Analyze how login credentials and file transfers are transmitted
- Compare the security risks of FTP with the encrypted communication of SFTP
- Demonstrate best practices for secure file transfer



## Tools & Technologies
- **Wireshark** – Network packet capture and analysis  
- **Linux** – For setting up test environments  
- **SFTP / FTP protocols** – Understanding secure vs insecure file transfers  
- **SSH** – Underlying encryption for SFTP



## Key Learnings
- FTP sends credentials and files in plaintext, making it vulnerable to interception  
- SFTP uses SSH encryption, ensuring confidentiality and integrity of transmitted data  
- Real-world implication: Organizations should prefer SFTP over FTP for secure file transfers  
- Hands-on experience with network traffic capture and analysis



## How to Reproduce
1. Set up a test environment with FTP and SFTP servers  
2. Use Wireshark to capture packets while transferring files  
3. Observe the difference:  
   - FTP packets show plaintext usernames and passwords
   - SFTP packets are encrypted and unreadable  
4. Document findings and generate screenshots for reports


## 📝 Summary of Findings

| Feature/Aspect          | FTP                           | SFTP                          |
|-------------------------|-------------------------------|-------------------------------|
| Encryption              | None (plaintext)              | SSH encryption                |
| Credentials Security    | Exposed                       | Encrypted                     |
| Data Transfer Security  | Vulnerable to interception    | Protected                     |
| Authentication Method   | Username/Password (plain)     | Username/Password over SSH    |
| Real-world Recommendation | Avoid for sensitive data      | Recommended for secure transfers |


## FTP vs SFTP Traffic Comparison

<div style="display: flex; justify-content: space-between;">

<img src="https://github.com/Zoje-stack/FTP-vs-SFTP-Security-Analysis/raw/bf14439498e3f45ab522b1c166289ca661d87faf/ftp_capture.png.png" alt="FTP Traffic" width="48%" height="300px" />
<img src="https://github.com/Zoje-stack/FTP-vs-SFTP-Security-Analysis/raw/bf14439498e3f45ab522b1c166289ca661d87faf/sftp_capture.png.png" alt="SFTP Traffic" width="48%" height="300px" />

</div>

**Figure 1:** FTP (left) shows plaintext credentials; SFTP (right) is encrypted.

