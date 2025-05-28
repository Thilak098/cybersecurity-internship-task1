# Local Network Port Scanning Project
This project demonstrates how to scan a local network for open ports and analyze potential security risks.

## Objective
Learn to discover open ports on devices in a local network to understand network exposure and potential vulnerabilities.

## Tools Used
- Kali Linux (VirtualBox)
- Nmap
- Wireshark

## Methodology

### Step 1: Environment Setup
- Opened Kali Linux in VirtualBox

### Step 2: IP Address Identification
- Used `ipconfig` (Windows) and `ifconfig`/`ip addr` (Kali Linux) to identify local IP addresses

### Step 3: TCP SYN Scan with Nmap
- Performed scan using: `nmap -sS 10.0.2.0/24`
- Identified active hosts and open ports in the network

### Step 4: Service Identification
- Used version detection scan: `nmap -sV 10.0.2.15/24`
- Performed aggressive scan: `nmap -A 10.0.2.15/24`
- Identified services running on open ports

### Step 5: Risk Analysis
Identified potential risks associated with open ports:
- Unauthorized Access
- Malware Infections
- Data Exfiltration
- Denial-of-Service (DoS) Attacks
- Misconfigured Services

### Step 6: Network Traffic Analysis with Wireshark
- Captured and analyzed network traffic
- Detected suspicious activity
- Identified potential security risks

## Screenshots
Include your screenshots from the document (you'll need to upload them to your repository):
1. `ifconfig` command output
2. `ip addr` command output
3. Nmap TCP SYN scan results
4. Nmap service version detection results
5. Nmap aggressive scan results
6. Wireshark capture analysis

## How to Run
1. Set up Kali Linux in VirtualBox
2. Open the terminal and identify your network IP range
3. Run Nmap scans as shown above
4. Analyze results with Wireshark

## Security Considerations
- Only scan networks you have permission to test
- Understand the legal implications of network scanning
- Document all findings responsibly
