# PDF to Web Form Automation

Automates the process of populating a web-based daily activity form by extracting activity logs from a structured PDF report and mapping them to the corresponding dates.

The project was built to eliminate repetitive manual data entry for internship activity submissions by combining PDF parsing with browser automation.

## Features

- Extracts activity descriptions from structured PDF tables
- Maps activities to their corresponding dates
- Automatically detects weekends and fills:
  - `Saturday - Not working.`
  - `Sunday - Not working.`
- Preserves bullet-point formatting with spacing for readability
- Locates form fields dynamically using date-based element IDs
- Automatically submits each day's activity
- Supports manual login before automation begins

## Tech Stack

- Python
- Selenium
- pdfplumber
- webdriver-manager
- Regular Expressions

## Installation

```bash
pip install selenium pdfplumber webdriver-manager
```

## Usage

1. Run the automation script.

2. Log in to the target portal manually.

3. Navigate to the activity submission page.

4. Return to the terminal and continue the script.

The automation will:

- Read the PDF
- Extract activities
- Match each activity with its date
- Populate the corresponding form fields
- Automatically mark weekends as non-working
- Submit each entry

## Applications

This workflow can be adapted for:

- Internship activity logs
- Daily work reports
- Academic journals
- Attendance records
- ERP/HRMS data entry
- Any structured PDF-to-web form workflow

## Libraries

- Selenium
- pdfplumber
- webdriver-manager
- datetime
- re (Regular Expressions)
