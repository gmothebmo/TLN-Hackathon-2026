# GoPhish - a Phishing detection tool

I created a local phishing tool to help users and professionals to determine whether their email is a phishing attempt or not. I was inspired by my daily routine of manually reviewing reported emails at my job, which requires me to download the reported email, manually copy the raw data from the email, and paste it into a tool that helps me confirm whether it's a spoof or scam email. I also use VirusTotal to scan unknown files and documents. After analyzing the email, I block it for the company I work for. 

## ⚙️ How to Run Locally ⚙️ ## 
1. Clone or download this repository.
2. Start a local development server or run via Office Add-in CLI (`npm run start`).
3. Access the taskpane locally at `https://localhost:3000/taskpane.html`.

## 📂 Project Structure 📂 ##
- `taskpane.html` - The core single-file HTML/JS user interface and analysis engine.

## Key Features ##
- **Local Heuristic Scanners:** Flags high-risk file extensions and anomalous sender domains.
- **Client-Side SHA-256 Hashing:** Computes file hashes locally in browser memory instantly.

