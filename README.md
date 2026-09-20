# GoPhish - a Phishing detection tool

I created a local phishing tool to help users and professionals to determine whether their email is a phishing attempt or not. I was inspired by my daily routine of manually reviewing reported emails at my job, which requires me to download the reported email, manually copy the raw data from the email, and paste it into a tool that helps me confirm whether it's a spoof or scam email. I also use VirusTotal to scan unknown files and documents. After analyzing the email, I block it for the company I work for. 

## ⚙️ How to Run Locally ⚙️ ## 
1. Download the file and "open with" your desired web application 

## 📂 Project Structure 📂 ##
- `taskpane.html` - The core single-file HTML and JS user interface and analysis engine.

## Key Features ##
- **Local Heuristic Scanners:** Flags high-risk file extensions and anomalous sender domains.
- **Client-Side SHA-256 Hashing:** Computes file hashes locally in browser memory instantly.
- **Display whether email is safe or not** After analyzing it will tell if it's safe or not.

