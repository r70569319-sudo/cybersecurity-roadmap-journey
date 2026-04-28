# Day 2: OS-Independent Troubleshooting (BIOS/UEFI & POST)

## Key Learnings
- BIOS is legacy firmware; UEFI is modern with Secure Boot support.
- POST beep codes diagnose hardware failures *before* the OS loads.
- Boot Order determines if a machine starts from HDD, USB, or Network.
- Physical access allows booting from a "Live USB" to bypass all OS passwords.

## Lab Evidence
- Screenshot: Accessing VirtualBox UEFI Firmware settings.
- <img width="1366" height="768" alt="Screenshot (6)" src="https://github.com/user-attachments/assets/9a6ed306-6ecf-480a-9bf1-879af9d17641" />

- Documented fix for 1 Long / 3 Short Beep (RAM Failure).

    User calls: "My computer turns on, fans spin, but screen is black and keyboard lights don't flash."

Your Step 1: Check monitor power and cable (Connection Types from Day 1!).

Your Step 2: Listen for Beep Codes (Today's lesson).

Your Step 3: Try booting without the hard drive connected (if you hear beeps then, the drive is the issue)

## Security Insight
"If I can change the boot order, I own the data. That's why servers are locked in cages and corporate laptops should have **BIOS passwords** enabled to prevent attackers from booting malicious USBs. Furthermore, **Secure Boot** ensures only trusted software loads during startup."

## Next Up
Day 3: Installing and Configuring Windows & Linux.
