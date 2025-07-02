📥 Automated-Inovoice-Processor


A powerful GUI-based Python application that automates the process of extracting invoice data from email attachments. 
It connects to your Gmail account, searches for emails containing a specific keyword in the subject (e.g., "Invoice"), 
downloads attached PDF files, extracts structured key-value pairs, displays them in a table, and allows exporting to CSV.


🚀 Features

- 📧 Secure Gmail login using app password
- 🔍 Automatically searches inbox for emails with subject containing "Invoice"
- 📎 Downloads PDF attachments only
- 📑 Extracts text from PDFs using `pdfplumber`
- 🔍 Detects key-value pairs using regex for structured data extraction
- 📊 Displays extracted data in a clean, sortable table
- 💾 One-click CSV export
- ⚙️ Multithreading for smooth UI performance
- 🪵 Detailed logging for debugging and traceability

🛠️ Technologies Used

- [Tkinter](w) – GUI framework
- [imaplib](w) – Email access
- [pdfplumber](w) – PDF text extraction
- [Pandas](w) – Data handling and CSV export
- [Logging](w), [threading](w), [regex](w) – Python standard libraries



🔐 Prerequisites

- A Gmail account
- A Gmail [App Password](w) (required due to Gmail's security policies)
- Python 3.7+
- Required libraries:
  `pip install pdfplumber pandas`


💻 How to Run
1. Clone the repository
   git clone https://github.com/your-username/invoice-pdf-extractor.git
   cd invoice-pdf-extractor

2. Install dependencies
   `pip install -r requirements.txt`

3.Run the app
  python invoice_extractor.py

4.Use the GUI
  Enter your Gmail address
  Enter your App Password (not your Gmail password)
  Click Download PDFs
  Once processed, click Export to CSV

📂 Folder Structure
   invoice-pdf-extractor/
   ├── attachments/         # Downloaded PDFs
   ├── extracted_data.csv   # Output file (after export)
   ├── invoice_app.log      # Logging file
   ├── invoice_extractor.py # Main script
   ├── README.md            # This file

🔐 Security Notes
   This application uses Gmail App Passwords to prevent security risks.
   Your credentials are not stored anywhere.
   It only searches for emails with subject line containing Invoice.

📊 Sample Output
   | Invoice Number | Date       | Amount  |
   | INV-001        | 2024-06-01 | ₹ 5,000 |
   | INV-002        | 2024-06-15 | ₹ 7,800 |
NOTE: Output is customizable depending on the key-value structure in your PDF invoices.

📝 License
   This project is open source under the `MIT License`.

🙌 Contributing
Contributions are welcome! Feel free to fork this repo and submit a pull request.

📧 Contact
    For support or feature requests, 
    reach out at: tailorkarthik15@gmail.com








