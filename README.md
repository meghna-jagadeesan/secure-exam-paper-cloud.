# Secure Exam Paper Cloud

## 1. Project Description

Secure Exam Paper Cloud is a Cloud Computing micro project that provides a secure platform to upload, encrypt, store, and release examination question papers at a scheduled time.

## 2. Technologies Used

* Python
* Flask
* SQLite
* Cryptography (Fernet encryption)
* HTML and CSS
* GitHub

## 3. Features

* User login with demo OTP verification
* Role-based access for administrators, examiners, and students
* Encryption of uploaded question papers
* Scheduled release of question papers
* Secure document viewer
* Audit logs and reports

## 4. Installation and Execution

### Requirements

* Python 3.10 or newer
* pip

### Steps

1. Download or clone the project.

2. Open the project folder in a terminal.

3. Create a virtual environment:

   `python -m venv .venv`

4. Activate it on Windows:

   `.venv\Scripts\activate`

5. Install dependencies:

   `python -m pip install -r requirements.txt`

6. Start the application:

   `python app.py`

7. Open `http://127.0.0.1:5000` in a browser.

## 5. Demo Credentials

| Role     | Username | Password    | OTP    |
| -------- | -------- | ----------- | ------ |
| Admin    | admin    | Admin@123   | 123456 |
| Examiner | examiner | Exam@123    | 234567 |
| Student  | student  | Student@123 | 345678 |

These credentials are for local educational demonstrations only.

## 6. Project Structure

* `app.py` — Flask application, authentication, encryption, timed release, and database operations.
* `templates/` — HTML templates for the website.
* `static/` — CSS styling.
* `requirements.txt` — Python dependencies.
* `sample_question_paper.txt` — Sample input file.
* `README.md` — Project documentation.

## 7. Sample Input and Output

**Sample input:**
A text file containing examination questions, such as defining cloud computing and explaining IaaS, PaaS, and SaaS.

**Expected output:**

* Uploaded paper is encrypted and stored.
* Before its scheduled release, access is blocked.
* After its release time, authorized users can view the paper.
* Access events are recorded in the audit log.

## 8. Security Notes

This project is an educational prototype. The OTP values are fixed demo codes, and the local application is not automatically deployed to a cloud provider. Production use would require real multi-factor authentication, HTTPS, secure secret management, and cloud hosting.
