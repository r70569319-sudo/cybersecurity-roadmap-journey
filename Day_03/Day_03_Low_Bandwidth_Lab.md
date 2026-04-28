# Day 3: Low Bandwidth OS Hardening

## Challenge
Internet speed restricted large ISO downloads. Pivoted to lightweight tools to achieve the same learning outcomes.

## Lab 1: Virtual Disk Partitioning (Windows Host)
- Created a 1GB VHD using Disk Management.
- Formatted as FAT32 vs NTFS. Observed the "Security Tab" missing in FAT32.
- **Insight:** NTFS supports Access Control Lists (ACLs). This is how Windows enforces file permissions.

## Lab 2: Alpine Linux Hardened Install
- Installed Alpine Linux (130MB ISO) with **LUKS Full Disk Encryption**.
- Configured UFW (Uncomplicated Firewall) post-install.
- Created a non-root user (`secadmin`) to follow Principle of Least Privilege.

## Lab 3: CIS Benchmark Analysis
- Reviewed Section 1.1 (Filesystem Hardening).
- Verified `cramfs` kernel module is blacklisted on Alpine.
- Learned that "Disabled by Default" is a sign of a secure OS baseline.

## Reflection
"Not having fast internet forced me to understand the **core components** rather than just clicking 'Next' on a fancy GUI. Alpine Linux is a beast for learning because it doesn't hide the config files."
