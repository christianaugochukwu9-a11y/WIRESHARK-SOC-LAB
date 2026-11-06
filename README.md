<img width="1080" height="1700" alt="Lab 8 Result - Christiana Joseph Ugochukwu (1)" src="https://github.com/user-attachments/assets/9eb8cb31-847f-4b3e-8739-88d5a6ff01ac" />
<img width="1080" height="1700" alt="Lab 7 Result - Christiana Joseph Ugochukwu" src="https://github.com/user-attachments/assets/9171aad1-86cf-4752-ab27-d93a24821430" />
<img width="1080" height="1700" alt="Lab 6 Result - Christiana Joseph Ugochukwu" src="https://github.com/user-attachments/assets/907c429c-abe6-45c4-9c22-129397346945" />
<img width="1080" height="1700" alt="Lab 5 Result - Christiana Joseph Ugochukwu" src="https://github.com/user-attachments/assets/43320807-a253-4288-a82b-085074406c6c" />
<img width="1080" height="1700" alt="Lab 4 Result - Christiana Joseph Ugochukwu" src="https://github.com/user-attachments/assets/76b0255b-442f-4b06-b68a-7935423d9d4e" />
<img width="1080" height="1700" alt="Lab 3 Result - Christiana Joseph Ugochukwu" src="https://github.com/user-attachments/assets/28f0fa02-9239-485b-8c67-c2ca713b24af" />
# Wireshark SOC Analysis - Internship Week 2 Labs

**Intern:** Christiana Joseph Ugochukwu  
**Program:** Networkwalks Academy Internship  
**Completion Date:** November 6, 2026  
**Overall Score:** 100% (600/600 total points)

## Overview
This repository contains key findings, display filters, and investigative notes from Week 2 of the Networkwalks Academy Cybersecurity Internship. The focus of this week was network traffic analysis, protocol inspection, and threat identification using Wireshark.

---

## Lab Breakdown & Technical Objectives

### 1. Lab 3: Identify the Attacker's IP (Port Scanning Analysis)
* **Focus:** Identifying network reconnaissance and active port scanning.
* **Key Techniques:**
  * Filtered `tcp.flags.syn == 1` to locate initial connection requests.
  * Identified source/destination IP pairs involved in port sweeping.
  * Analyzed RST/ACK responses to determine open vs. closed target ports.

### 2. Labs 4 & 5: Follow TCP Stream (Session Reconstruction)
* **Focus:** Session reassembly and data extraction across chat and web protocols.
* **Key Techniques:**
  * Reassembled multi-packet TCP streams to reconstruct full plaintext conversations.
  * Identified specific port assignments, hidden directory paths, and server backup endpoints.
  * Verified HTTP status codes (200 OK) and extracted file download metadata.

### 3. Lab 6: HTTP Plaintext Credentials
* **Focus:** Analyzing cleartext credential exposure.
* **Key Techniques:**
  * Filtered HTTP `POST` requests targeting login forms.
  * Extracted plain-text usernames and passwords directly from request body lines.
  * Identified target login URI paths and client source IPs.

### 4. Lab 7: Brute Force Detection
* **Focus:** Identifying automated authentication attacks.
* **Key Techniques:**
  * Tracked failed authentication HTTP status codes (e.g., 401/403).
  * Calculated attack volume and identified the exact credential combination that successfully logged in.
  * Differentiated between dictionary attack patterns and normal user traffic.

### 5. Lab 8: VoIP Call Replay & Inspection
* **Focus:** Analyzing signaling and voice media protocols.
* **Key Techniques:**
  * Analyzed **SIP** setup parameters (INVITE, 200 OK, BYE) to identify caller and receiver extensions.
  * Identified voice payload codecs (`ITU-T G.711 PCMU`).
  * Evaluated security risks of unencrypted RTP and recommended **SRTP** for encrypted voice communications.

---

## Skills Demonstrated
* Packet Capture Analysis (PCAP)
* Wireshark Display Filtering & Syntax
* Protocol Analysis: TCP, HTTP, SIP, RTP
* Credential Harvesting Detection & Brute Force Analysis
* Mitigation Strategies (TLS/HTTPS, SRTP, Key Exchange)
