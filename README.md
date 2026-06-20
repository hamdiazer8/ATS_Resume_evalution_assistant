\# ATS Resume Evaluation Assistant



An AI-powered workflow that evaluates resumes against Applicant Tracking System (ATS) criteria and automatically stores results in Google Sheets.



\## Overview



Recruiters often receive hundreds of resumes for a single position. This project automates the initial screening process by extracting resume content, analyzing it with a Large Language Model (LLM), generating an ATS compatibility score, and storing structured evaluation results for further review.



\## Features



\- Resume upload via webhook

\- Automatic text extraction from uploaded files

\- AI-powered ATS analysis using Groq

\- ATS score generation

\- Strengths and weaknesses detection

\- Resume improvement recommendations

\- Automatic storage of results in Google Sheets



\## Workflow



```text

Webhook

   ↓

Resume Extraction

   ↓

Data Processing

   ↓

Groq LLM Analysis

   ↓

JSON Parsing

   ↓

Google Sheets

```



\## Tech Stack



\- n8n

\- Groq LLM

\- JavaScript

\- Google Sheets



\## Current Status



✅ End-to-end workflow implemented and tested.



\## Future Improvements

&#x20;-Improved ATS scoring methodology

\- Add error handling and input validation

\- Support for additional document formats

\- Web application interface

\- Multi-resume batch processing



\## Setup:



1\. Import the workflow into n8n.

2\. Configure your Groq and Google Sheets OAuth credentials.

3.Set your real Spreadsheet ID and sheet tab name

4\. Activate the workflow.

5\. Trigger:

&#x20;    Send a POST request with a resume file to the webhook URL to start the workflow.

&#x20;     Example



```text

POST http://your-n8n-instance/webhook/ATS\\Resume\\evalution\\assistant

```



6\. The workflow will:

&#x20;  - Extract the resume text

&#x20;  - Analyze it using Groq

&#x20;  - Generate an ATS score and recommendations

&#x20;  - Store the results in Google Sheets



\## Author



Azer Hamdi

