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
