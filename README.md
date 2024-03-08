# HackTheBox Analysis Writeup

## Overview

This document outlines the steps taken and findings from a CTF challenge focusing on various cybersecurity techniques including enumeration, exploitation, and privilege escalation on a target machine.

## Enumeration

The initial step involved using `nmap` for port scanning and identifying open services, followed by `gobuster` and `dirsearch` for directory enumeration. The goal was to map out the target's network and discover potential entry points.

## Exploitation

Key findings during the exploitation phase included identifying vulnerable web pages and leveraging a Blind LDAP injection vulnerability to extract sensitive information. This allowed for unauthorized access to certain areas of the application.

## Privilege Escalation

The privilege escalation could be done two different ways:

1. **Snort DLL Hijacking:** Leveraged writable directories and misconfigurations in the Snort application to execute a custom DLL.
2. **API Hooking - DLL Injection:** Demonstrated how to capture plaintext passwords by hooking into API calls using a custom DLL and injector.

### Here is my github repo for BCTextEncoder_DLL_injection:
    - https://github.com/player23-0/BCTextEncoder_DLL_injection

## Conclusion

This writeup provides a step-by-step guide on exploiting a series of vulnerabilities to achieve unauthorized access and escalate privileges on a target machine. The methods demonstrated include network scanning, directory enumeration, blind LDAP injection, DLL hijacking, and API hooking for password capture.

## Disclaimer

This writeup is intended for educational purposes only. Ethical guidelines and legal compliance must be followed when conducting security assessments.

