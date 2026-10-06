AI CV Screening Automation

An AI-powered CV screening and interview automation built with n8n, AI / GPT, Google Forms, Google Sheets, Gmail, Google Calendar, HTTP Request, and JavaScript.

Overview

This automation is designed to simplify the initial candidate screening and interview scheduling process.

The workflow starts when a candidate submits an application form with their basic information and CV.

The candidate provides:

- Candidate Name
- Email Address
- CV / Resume

Once the form is submitted, the workflow automatically processes the uploaded CV and sends the required information for AI-powered screening.

The AI analyzes the candidate's CV and generates a screening score along with feedback based on the defined screening criteria.

The workflow then processes the AI response using JavaScript and stores the candidate's screening information in Google Sheets.

The screening result is then passed to an IF node that checks whether the candidate has achieved the required score.

The minimum shortlisted score is set to 70%.

If the candidate scores 70% or above, the candidate is considered shortlisted.

The workflow automatically sends a congratulations email through Gmail and creates an interview event in Google Calendar.

The interview is scheduled three days after the candidate's screening.

The Google Calendar event contains important candidate information such as:

- Candidate Name
- Candidate Email
- Screening Score
- Candidate Feedback
- Interview Date
- Interview Time

If the candidate scores below 70%, the workflow automatically sends a polite email informing the candidate that they were not selected for the next stage.

This allows the complete initial screening, candidate communication, and interview scheduling process to be handled automatically.

Workflow

Form Submission → Candidate Name + Email + CV Upload → JavaScript → HTTP Request → AI CV Screening → JavaScript → Google Sheets → IF (70% Score) → Shortlisted / Not Shortlisted

Shortlisted Candidate Flow

Candidate Score ≥ 70% → Gmail Congratulations Email → Google Calendar → Interview Scheduled After 3 Days

Not Shortlisted Candidate Flow

Candidate Score < 70% → Gmail → Polite Rejection Email

The workflow uses the candidate's screening score to automatically decide which path the candidate should follow.

Features

- 📋 Receive candidate applications through a form
- 👤 Collect candidate name and email
- 📄 Receive uploaded CV / Resume
- 🤖 AI-powered CV screening
- 📊 Automatically generate a candidate screening score
- 📝 Generate screening feedback
- 💻 Process CV screening data using JavaScript
- 🌐 Send CV data for AI processing using HTTP Request
- 📊 Store candidate information in Google Sheets
- 🔀 Automatically evaluate candidates using an IF condition
- ✅ Shortlist candidates scoring 70% or above
- ❌ Identify candidates scoring below 70%
- 📧 Automatically send rejection emails to unsuccessful candidates
- 🎉 Automatically send congratulations emails to shortlisted candidates
- 📅 Automatically create interview events in Google Calendar
- 🗓️ Schedule shortlisted candidates for an interview three days after screening
- 📌 Add candidate information to the Google Calendar event
- 📈 Include candidate score and feedback in the interview information
- ⚡ Automate the complete initial screening process

Technologies Used

- n8n
- AI / GPT
- Google Forms
- Google Sheets
- Gmail
- Google Calendar
- HTTP Request
- JavaScript

n8n

n8n is used to connect all the services and control the complete automation workflow.

It handles the form submission, data processing, AI screening, candidate score evaluation, Google Sheets storage, Gmail communication, and Google Calendar scheduling.

AI / GPT

AI is used to analyze the candidate's CV and generate a screening score and feedback.

The AI screening result is then processed by the workflow to determine whether the candidate meets the required 70% threshold.

Google Forms

Google Forms is used as the candidate application form.

Candidates can submit their basic information and upload their CV through the form.

Google Sheets

Google Sheets is used to store the candidate information and screening results.

This provides a structured record of the candidates processed by the automation.

Gmail

Gmail is used for automated candidate communication.

Candidates below the required score receive a polite rejection email.

Candidates who meet the 70% or higher requirement receive a congratulations email informing them that they have been shortlisted.

Google Calendar

Google Calendar is used to automatically schedule interviews for shortlisted candidates.

The interview event contains the candidate's name, email, screening score, feedback, date, and selected interview time.

HTTP Request

The HTTP Request node is used as part of the CV processing and AI screening process.

It allows the workflow to send the required information for further processing.

JavaScript

JavaScript is used to process and prepare information between different steps of the workflow.

It helps handle the CV and AI screening data before it is stored or passed to the next step.

Use Case

This automation can help businesses, HR teams, recruiters, recruitment agencies, and companies that regularly receive candidate applications.

Instead of manually reviewing every CV, checking candidate scores, sending individual emails, and creating interview appointments, the workflow can automatically handle these repetitive tasks.

A typical process starts when a candidate submits their application and CV.

The automation processes the application, performs AI-powered screening, generates a score and feedback, and stores the result.

Candidates who meet the required score are automatically shortlisted.

The shortlisted candidate receives a confirmation email and an interview is automatically created in Google Calendar.

Candidates who do not meet the required score receive a polite rejection email.

This can help reduce manual recruitment work and make the initial candidate screening process faster and more organized.

Project Status

Completed portfolio project.

Demo Video

"Watch the Demo" (./CV_Screening_Automation_Demo.mp4)
