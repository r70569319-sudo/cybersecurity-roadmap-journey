# Day 5: Permissions & Access Control

## Key Learnings
- Linux `rwx` applies to Owner, Group, and Others.
- Octal notation: 4=Read, 2=Write, 1=Execute. `chmod 640` is the security sweet spot.
- To delete a file, you need write permission on the **directory**, not the file.
- Windows `icacls` lets you view and set granular NTFS permissions.
- "Everyone: Full Control" is the Windows equivalent of `chmod 777` and must never exist on a server share.

## Lab Evidence
- Alpine: Created a world-writable file, then secured it to `640`. Demonstrated directory-based deletion.
- Windows: Used `icacls` to grant and revoke permissions on a test folder.

## Security Insight
"The SUID bit on a root-owned binary is a loaded gun. Finding all SUID files on a system is one of the first things an auditor or an attacker does. I ran `find / -perm -4000` and saw how many legitimate programs need this (like `sudo`). Hiding a malicious SUID binary is a classic backdoor."

## Next Up
Day 6: Software Installation & Package Management.
