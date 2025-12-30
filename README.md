# FTP vs SFTP Security Analysis
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/ohiozoje-ohikhuare-453791221/)  [![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:huare1960@gmail.com)


## Project Overview
This project demonstrates the security differences between FTP and SFTP by capturing and analyzing network traffic using Wireshark.
The goal is to highlight how FTP transmits sensitive information in plaintext, while SFTP protects data through encryption over SSH.



## Project Objectives
- Capture FTP and SFTP traffic using Wireshark
- Analyze how authentication and file transfer occur over the network
- Identify security risks associated with FTP
- Demonstrate how SFTP provides confidentiality and integrity
- Reinforce best practices for secure file transfer



## Tools & Technologies
- **Wireshark** – Network packet capture and analysis  
- **Linux** – For setting up test environments  
- **SFTP / FTP protocols** – Understanding secure vs insecure file transfers  
- **SSH** – Encryption mechanism used by SFTP



## Key Learnings
- FTP transmits usernames and passwords in plaintext, making them vulnerable to interception
- FTP file transfers can be exposed if the data channel is captured
- SFTP encrypts both authentication and data using an SSH tunnel  
- Encrypted protocols significantly reduce the risk of credential theft and data leakage
- Secure protocols like SFTP are preferred in real-world environments



## Methodology
1. Configure FTP and SFTP services on a Linux system  
2. Start packet capture in Wireshark
3. Perform file transfers using FTP and SFTP clients 
4. Analyze captured packets:  
   - FTP control traffic reveals plaintext credentials
   - SFTP traffic appears encrypted and unreadable  
5. Capture screenshots and document observations


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

**Figure 1:** FTP traffic reveals readable commands and credentials, while SFTP traffic is fully encrypted.

## Conclusion
This project demonstrates why FTP is insecure by design and why SFTP is the preferred alternative for secure file transfer.
Using encrypted protocols is critical for protecting sensitive data in modern networks.

