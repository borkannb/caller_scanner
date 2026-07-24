# Caller Scanner

A high-performance, asynchronous Python tool designed for automated contact scanning and session management. It features parallel processing, automated browser handling via Playwright, and seamless database synchronization with MongoDB.
---
## Features
* **Asynchronous Scanning:** Powered by `asyncio` and `httpx` for high-speed concurrent network requests.
* **Smart Session Management:** Automated login and session generation, renewal, and management via `Playwright`.
* **Interactive CLI:** Easy-to-use command-line interface for managing sessions and running scans.
---
## Prerequisites
Ensure you have the following installed on your system:
* **Python 3.8+**
* **pip** (Python package manager)
---
## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/borkannb/caller-scanner.git
   cd caller-scanner
   cd dist
   pip install -r requirements.txt
   playwright install
Configuration
Make sure your configuration files are set up properly before running the tool:

config.json (Optional): You can customize connection limits, memory divisors, and output file names. If missing, default settings will be applied automatically.

phones.txt: Create this file and add the phone numbers you want to scan, making sure they follow the correct international format (one number per line with country code).

Format Note: Ensure phone numbers are provided in the correct international format without extra symbols or spaces (e.g., entering numbers mapped to your target country code according to your search profile).   
Usage
Run the main script from your terminal:
python main.py
Interactive Menu Options:
[1] Create / Renew Session: Enter your account credentials (email and password) to authenticate, solve verification if required, and securely generate/update your session file.

[2] Start Contacts Scanner: Begins the parallel scanning process using your active sessions, checking numbers against phones.txt, saving valid findings to results.txt, and logging unknown numbers to unknown.txt.

[3] View Active Sessions Count: Displays the total number and names of currently active saved sessions.

[4] Exit: Safely closes the application
