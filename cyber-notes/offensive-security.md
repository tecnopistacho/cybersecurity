# Offensive Security — Lesson 1 Notes

Understanding how attackers think is essential for defending systems. Ethical hackers study the same techniques used by hackers, but apply them legally and responsibly to strengthen security.

---

## Overview of the Exercise
Simulated hacking scenario using a virtual machine, that runs a fake banking application called **FakeBank**. 

The objective was to discover hidden directories on the website.

---

## Gobuster: Directory Enumeration Tool
We used **Gobuster**, a command-line tool for brute‑forcing directories and files on a web server.

### Command used:

```
gobuster -u http://fakebank.thm -w wordlist.txt dir
```

### Flags explained:
- **`-u`** — specifies the target URL  
- **`-w`** — provides a wordlist for Gobuster to iterate through  
- **`dir`** — tells Gobuster to search for directories

Gobuster reports directories that return a **Status: 200**, meaning the page exists. One of the discovered pages was:

```
http://fakebank.thm/bank-transfer
```

---

## Key Concepts Learned
- Offensive security involves identifying vulnerabilities before attackers do, helping defenders anticipate threats.
- Reconnaissance is often the first step in a penetration test.
- Tools like Gobuster automate the discovery of hidden resources.

---

## Roles in Cybersecurity
- **Offensive roles:** penetration tester, red teamer, security engineer  
- **Defensive roles:** security analyst, incident responder, SOC analyst  

Understanding both sides improves overall security awareness.

---

## Learning Approach
Breaking complex topics into smaller areas and practicing regularly through hands‑on labs is the most effective way to build cybersecurity skills.
