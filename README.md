# GoPhish - a Phishing detection tool

I created a local phishing tool to help users and professionals to determine whether their email is a phishing attempt or not. I was inspired by my daily routine of manually reviewing reported emails at my job, which requires me to download the reported email, manually copy the raw data from the email, and paste it into a tool that helps me confirm whether it's a spoof or scam email. I also use VirusTotal to scan unknown files and documents. After analyzing the email, I block it for the company I work for. 

## ⚙️ How to Run Locally ⚙️ ## 
1. Download the file and "open with" your desired web application 

## 📂 Project Structure 📂 ##
- `taskpane.html` - The core single-file HTML and JS user interface and analysis engine.

## Key Features ##
- **Local Heuristic Scanners:** Flags high-risk file extensions and anomalous sender domains.
- **Client-Side SHA-256 Hashing:** Computes file hashes locally in browser memory instantly.
- **Display whether email is safe or not:** After analyzing it will tell if it's safe or not.
- **Google DoH:** Performs real-time DNS checks to detect invalid or suspicious domains.
- **Email Header Parsing:** Detects forwarded emails and extracts the original sender.
- **Phishing Keyword Detection:** Scans email content for common phishing keywords.
- **VirusTotal Lookup:** Uses SHA-256 hashes to check files against VirusTotal.
- **Privacy-First:** Runs locally in the browser, keeping email data and attachments off external servers.

# Project Story

## Inspiration
As a student and full-time IT specialist with six years of hands-on experience, I’ve seen firsthand how often IT professionals have to respond to suspicious and phishing emails submitted by users. The typical process requires us to download the email, inspect the raw headers and data, copy that information into a verification tool, and manually determine whether the email is legitimate or malicious. I wanted to build a security tool that streamlines this process by automating the initial verification steps, helping IT professionals investigate suspicious emails faster and reducing the manual work involved.

## What it does
GoPhish analyzes suspicious email headers and sender domains using live Google DNS-over-HTTPS (DoH) lookups and local heuristic checks to determine email legitimacy. Additionally, it features an integrated VirusTotal file-hashing workflow allowing IT staff to instantly cross-reference suspicious file attachments against global threat intelligence.

## How we built it
The application is built entirely using vanilla HTML and client-side JavaScript as a standalone local web utility, leveraging internet connectivity to execute live DNS resolution lookups and API queries.

## Challenges we ran into
My initial goal was to develop a native Microsoft Outlook add-in, but I ran into authentication and environment configuration roadblocks with Outlook accounts. While I initially wanted to build a Node.js backend, time constraints during the event forced me to pivot. I adapted the core concept into a lightweight, standalone local tool instead of a global deployment.

## Accomplishments that we're proud of
I am proud to have successfully integrated the free Google DNS-over-HTTPS API to perform real-time domain resolution checks and incorporated VirusTotal file hash lookups to significantly enhance the overall security analysis of emails and attachments. This allows IT professionals to analyze suspicious emails with minimal manual effort.

## What we learned
I learned how straightforward it is to prototype and deploy a standalone local application compared to navigating the tedious setup process of a live Outlook add-in. I also appreciated how seamlessly HTML and JavaScript work together to deliver a clean, intuitive user interface for IT personnel.

## What's next for GoPhish
Moving forward, I plan to dive deeper into the Outlook add-in development ecosystem to resolve the initial authentication blockers. I also want to integrate additional threat intelligence APIs and refined heuristics to improve detection accuracy and minimize potential false positives. Also, make the UI more engaging than boring colors. 
