# 🛡️ TryHackMe: Offensive Security Intro (Write-Up)

## 📌 Project Overview
This repository documents my completion of the **Offensive Security Intro** lab on TryHackMe. The purpose of this exercise was to understand the attacker's methodology regarding web application vulnerabilities in order to better defend enterprise networks.

## 🔎 Vulnerability Explored: Broken Access Control
During this lab, I simulated an attack on a web application's administrative capabilities. 

*   **The Flaw:** The web application utilized insecure routing, allowing unauthenticated users to access a sensitive portal (`/bank-transfer`) simply by inputting the direct URL path into the browser.
*   **The Impact:** Due to a lack of proper authentication checks on the administrative endpoint, an unauthorized user could manipulate database values (e.g., artificially altering account balances).

## 🛠️ Skills & Concepts Practiced
*   **Web Architecture:** Navigating hidden administrative directories and understanding URL paths.
*   **Offensive Perspective:** Simulating administrative bypass techniques to understand what malicious traffic looks like in web server logs.
*   **Defensive Takeaway:** To mitigate this vulnerability, developers must implement strict **server-side authentication and authorization checks** on every sensitive endpoint, ensuring that requests without valid session tokens are automatically rejected.

---
*Note: This lab was performed entirely within a legally compliant, isolated sandbox environment provided by TryHackMe for educational purposes.*

