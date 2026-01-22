# Project Gospel Network: Cryptographic Integrity for Digital Outreach
**Field:** Information Security / Cryptography / Data Integrity

## Project Overview
The goal of **MissionGuard** is to ensure the **authenticity** and **integrity** of bible scripture in environments where digital communication may be monitored or tamperered. By using Public Key Infrastructure (PKI), I ensure that the recipient can verify that the message came from a trusted source and has not been altered by a third party.

## ️ Technical Stack
- **OS:** macOS (Apple M3)
- **Environment:** Unix Terminal (Zsh)
- **Tools:** GnuPG (GPG), Homebrew
- **Protocol:** RSA-3072

## Implementation
1. **Key Generation:** I generated a 3072-bit RSA key pair to ensure long-term strength.
2. **Digital Signing:** Applied 'clearsign' protocols to Gospel texts to maintain human-readability while embedding a cryptographic hash.
3. **Identity Verification:** Linked digital signatures to my verified email identity.

## Repository Contents
- 'verse.txt': An original copy of the bible verse with no encryption(John 15:17).
- 'verse.txt.asc': A clear-signed bible verse (John 15:17).
- 'ProjectGospelNetwork_PublicKey.asc': My first public key for verification(expired).
- 'ProjectGospelNetworkv2_PublicKey.asc': The current public key for verification.

## How to Verify My Work
To verify the integrity of the signed file in this repository, follow these steps in your terminal:

1. **Import my key:**
   'gpg --import ProjectGospelNetworkv2_PublicKey.asc'
2. **Verify the message:**
   'gpg --verify verse.txt.asc'

*If successful, you will see: "gpg: Good signature from Perry Long "*

---
**Disclaimer:** This project is for educational purposes as part of a cybersecurity analyst career path and it is focused on ethical stewardship and data protection. 
