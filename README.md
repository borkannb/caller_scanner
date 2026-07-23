Caller Scanner Tool
An advanced, parallel tool for efficiently scanning and extracting contact data, with secure session management support.

🚀 Key Features
Parallel Scanning (Async/Concurrent): Fully utilizes processor and network capabilities to scan numbers at maximum speed.

Smart Session Management: Supports automatic session creation and renewal via a secure browser.

⚙️ System Requirements
Before starting, ensure the following are installed on your machine:

Python 3.10 or later

Supported Operating System: Linux (Kali Linux recommended)

📥 Installation and Operation
Follow these steps to set up and run the tool on your local machine:

1. Clone the Repository
Open your terminal and clone the project repository, then navigate into the project directory:

Bash
git clone https://github.com/borkannb/caller_scanner.git
cd caller_scanner
2. Install Prerequisites
Install all required Python libraries by running the following command:

Bash
pip install -r requirements.txt
3. Prepare the Input Data
Create a text file named phones.txt inside the dist directory (or the main project folder depending on your structure), and add the phone numbers you want to scan.

Example format (phones.txt):

Plaintext
+201012345678
+201123456789
+201234567890
4. Run the Tool
Execute the main script to start the scanning and session management process:

Bash
python3 main.py
