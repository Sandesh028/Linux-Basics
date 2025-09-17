# Linux-Basics
## Linux CTF Training 

### Welcome!
This container is a safe, isolated training environment to learn Linux privilege-escalation fundamentals and common misconfigurations. You will be presented with several short, focused challenges. The goal is learning by exploring — we will tell you where to look and which commands/tools to use, but we won't provide direct solutions. Think like an investigator: examine, hypothesize, and test.

Important: this lab runs inside a container and is intentionally vulnerable for training only. Do not mount host folders or run with --privileged. Keep everything isolated.

#### What you should learn: 
```

How to discover privileged files and misconfigurations (SUID, file permissions, sudo rules).

How to inspect binaries and config files safely (use strings, file, ldd, ls -l).

Basic privilege escalation concepts (SUID misuse, sudo misconfiguration, PATH / helper issues).

How to reason about remediation and secure configuration.
```


## Where to start (places to inspect)

- Explore these areas and concepts. We list places rather than explicit answers:

- System-wide locations that often contain privileged binaries, config, and flags (look at file ownership and permissions).

- User home directories — check for readable files that may contain hints or public artifacts.

- Root-owned top-level directories (/root, /etc) for protected artifacts (you won’t have access initially; learn how escalation works).

- Sudo configuration and sudo-related files (who can run what).


## Useful commands & tools (learn these)

These commands are allowed and expected in the lab. Use them to examine the system — learn their output and what it implies.

#### Basic identity & file commands
- whoami
- id
- pwd
- ls -la /path
- stat /path



sudo -l (to see what your user may run)

## There are 3 users:
* root
* ctfplayer : ctfplayer
* challenger : challenger
```
# To switch user:
su - username
```
```
# To exit:
exit
```
