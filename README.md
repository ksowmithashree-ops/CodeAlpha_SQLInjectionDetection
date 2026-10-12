#Task-2:
SQL Injection Detection System

A Flask-based security dashboard that detects suspicious SQL-like input, identifies potential risks, and records security events for review.

## Features

- Rule-based detection of suspicious SQL patterns
- Risk classification: Low, Medium, and High
- Safe database search using parameterized SQL queries
- Security event logging with timestamps and matched rules
- Event review functionality
- Responsive dashboard
- Health check endpoint (`/health`)
- Automated tests using Pytest

## Technologies Used

- Python
- Flask
- SQLite
- HTML and CSS
- Pytest

## Installation and Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
   ```

2. Navigate to the project folder:

   ```bash
   cd YOUR-REPOSITORY
   ```

3. Install dependencies:

   ```bash
   python -m pip install -r requirements.txt
   ```

4. Configure the environment variables using `.env.example`, if required by the application.

5. Start the application:

   ```bash
   python app.py
   ```

6. Open `http://127.0.0.1:5000` in your browser.

## How to Test

1. Search for a sample record, such as `Asha`.
2. Scan normal text to observe a low-risk result.
3. Try a harmless SQL injection training string to observe detection.
4. Review the recorded security event.
5. Check the `/health` endpoint.

## Run Automated Tests

```bash
python -m pytest -q
```

## Project Purpose

This project demonstrates basic web application security concepts, suspicious-input detection, database query safety, and security-event monitoring.

## Limitations

This is an educational demonstration, not a production intrusion detection or prevention system. Rule-based detection may produce false positives or miss certain attacks. Always use parameterized queries and appropriate security controls in real applications.
