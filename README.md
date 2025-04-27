# 📄 MailPhoneExtractor

**MailPhoneExtractor** is a lightweight Python tool that automatically extracts email addresses and US-format phone numbers from raw text data like email discussions and message threads.

---

## 🚀 Features
- Extract all **email addresses** and **US phone numbers** from unstructured text.
- Automatically clean noisy text (e.g., remove "Original Message" parts).
- Flexible phone number format support: (xxx) xxx-xxxx, xxx-xxx-xxxx, etc.
- Save clean results into a structured Excel file.

---

## 🛠 How It Works
1. Read input Excel file (must have a `message` column).
2. Clean text (remove unnecessary content).
3. Extract emails and phone numbers using regex.
4. Save results into a new Excel file.

---

## 📥 Installation
```bash
git clone https://github.com/yourusername/MailPhoneExtractor.git
cd MailPhoneExtractor
pip install -r requirements.txt
```

---

## 🧩 Usage
Prepare an input Excel file sample_input.xlsx inside the sample_data/ folder with a column named message.
Then run:
```bash
python main.py
```

The cleaned and extracted emails/phones will be saved to a new Excel file:
output_result.xlsx

---

## 📊 Example
**Input text:**
```bash
Hello, you can reach me at john.doe@example.com or call me at (123) 456-7890. Thanks!
```
**Extracted Output:**

| email_1               | phone_1       |
|:----------------------|:--------------|
| john.doe@example.com   | (123) 456-7890 |

---

## 📌 Requirements
Python 3.7+
pandas
openpyxl

