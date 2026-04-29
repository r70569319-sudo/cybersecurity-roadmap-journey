# Day 4: CLI Navigation & Command Fundamentals

## Key Learnings
- **Linux Filesystem Hierarchy:** `/etc` = configs, `/var/log` = evidence, `/home` = user data.
- **CRUD Operations:** `touch` (create), `mv` (rename/move), `cp` (copy), `rm` (delete). Extremely dangerous as `root`.
- **Permission Errors:** Seeing `Permission Denied` is a sign of a properly configured system.
- **Windows Net Commands:** `net user`, `netstat`, `tasklist` are the holy trinity of IR triage.

## Lab Evidence
- Screenshot: Output of `ls -la /` on Alpine showing the directory structure.
- Screenshot: Output of `net user` on Windows showing no suspicious accounts.

## CLI vs GUI Reflection
"I realized that to truly understand what my computer is doing, I have to ask it questions in text. The GUI is a polite receptionist; the CLI is the engineer in the server room. Today I learned how to walk past the receptionist."

## Next Up
Day 5: Permissions Deep Dive (Linux chmod, Windows ACLs).
