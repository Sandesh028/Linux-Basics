# 🐧 Linux CTF Training Environment

Welcome! This container provides a **safe playground** for learning Linux basics and practicing Capture the Flag (CTF) style challenges.  
You’ll explore, discover, and escalate privileges just like an attacker might do but all **inside an isolated Docker container**.

---


## 🎯 Learning Objectives

By the end of this lab, you will:

1. Navigate the Linux filesystem as a non-root user.  
2. Explore file permissions and hidden files.  
3. Discover and understand **SUID binaries**.  
4. Perform a simple **privilege escalation**.  
5. Locate and read multiple challenge flags.  

---

## 🚀 Starting the Lab

Build and run the container:

```bash
# Build (only once)
docker build -t basic .

# Run (fresh container each time)
docker run -it basic
```

## Commands 
* whoami        # check your current user
* id            # see your UID and groups
* pwd           # show current directory
* ls            # list files, (-l) permissions of files, (-a) including hidden ones
