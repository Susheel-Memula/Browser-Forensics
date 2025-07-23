Browser Forensics
This Python project analyzes Chrome browser artifacts—specifically History, Cookies, and Downloads—and generates a structured PDF report (forensic_report.pdf). It's ideal for digital forensic investigations, browser behavior analysis, and educational purposes.

📁 Input Files
Ensure the following CSV files are present in the same directory as the script:

History.csv

Cookies.csv

Downloads.csv

These files are typically extracted from Chrome's SQLite databases using tools like DB Browser for SQLite or automated browser artifact extraction tools.

✨ Features
🔍 Analyzes browsing history, identifying the most recently visited site and the site visited most frequently.

🍪 Extracts and lists long-lived cookies (valid for more than 1 year).

📥 Displays complete information about the most recent download.

🧾 Generates a clean PDF report using the ReportLab library.

📦 Installation
Install the required dependencies using pip:

bash
Copy
Edit
pip install pandas reportlab
🚀 How to Run
Place History.csv, Cookies.csv, and Downloads.csv in the same folder as forensic_report.py.

Execute the script using:

bash
Copy
Edit
python forensic_report.py
The report will be saved as forensic_report.pdf in the current directory.

📄 Output Report Includes
🧭 Browsing History
Last visited website with timestamp.

Most visited website based on visit count.

🍪 Cookies
List of session cookies with a lifespan of over one year.

📥 Downloads
Information about the latest downloaded file:

File name

Download URL

Start time

Received bytes

Total size

Download state

🔐 Use Cases
This project can be used by:

👮 Digital forensic analysts and cybersecurity professionals

🏛️ Law enforcement officers investigating browser activity

🎓 Academic researchers and students in cyber forensics

👨‍👩‍👧‍👦 Parents monitoring browser usage for safety

📃 License
This project is released under the MIT License.

