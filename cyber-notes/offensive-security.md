# Offensive Security — Lesson 1 Notes

Understanding how attackers think is essential for defending systems. Ethical hackers study the same techniques used by malicious actors, but apply them legally and responsibly to strengthen security.

---

## Overview of the Exercise
The lesson introduced a simulated hacking scenario using a virtual machine running a fake banking application called **FakeBank**. This environment allows safe, legal practice of offensive security techniques.

The objective was to discover hidden directories on the website and understand how an ethical hacker approaches reconnaissance.

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

This demonstrates how attackers find hidden or unlinked pages that developers may overlook.

---

## Key Concepts Learned
- Offensive security involves identifying vulnerabilities before attackers do.
- Ethical hackers use controlled environments to practice safely.
- Reconnaissance is often the first step in a penetration test.
- Tools like Gobuster automate the discovery of hidden resources.
- Thinking like an attacker helps defenders anticipate threats.

---

## Roles in Cybersecurity
- **Offensive roles:** penetration tester, red teamer, security engineer  
- **Defensive roles:** security analyst, incident responder, SOC analyst  

Understanding both sides improves overall security awareness.

---

## Learning Approach
Breaking complex topics into smaller areas and practicing regularly through hands‑on labs is the most effective way to build cybersecurity skills.
