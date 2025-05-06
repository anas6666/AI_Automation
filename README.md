# AI_Automation

I’ve built AI-powered workflows using N8N and Make.com to automate key tasks like resume sorting, lead extraction, and email handling. These automations streamline processes, saving time and boosting efficiency across HR, data analysis, and digital communication.

# N8N

### Email (IMAP) Resume Classifier & Sorter with Validation : ( RESUME CLASSIFIER FROM EMAIL.json )
![image](https://github.com/user-attachments/assets/1cf5a28c-f182-4488-b43d-10819a145939)

### Description: 
Monitors an email inbox (IMAP) for messages with attachments. Checks if the attachment is a PDF and if the email subject matches a job reference in a Google Sheet. If valid, uses AI to analyze the CV (extract info, calculate experience, score). Logs data to a Sheet and moves/renames the CV in Google Drive based on the score. Sends automated email replies if the attachment isn't PDF or the job reference is missing/invalid.

### Google Drive Resume Classifier & Sorter : (RESUME CLASSIFIER FROM GOOGLE DRIVE.json )
![image](https://github.com/user-attachments/assets/41e93eff-4a01-4de5-86ce-9a1dcd39f3de)

### Description: 
Watches a Google Drive folder for new PDF resumes. Extracts text, looks up corresponding job details from a Google Sheet (based on filename prefix). Uses AI to analyze the CV, extract candidate info, calculate total experience, and score suitability. Appends details to a central Google Sheet, moves the original CV file to a folder based on suitability score (>70% or <70%), and renames the file.

## Gmail Resume Classifier (PDF & Word) : (AI_CV_CLASSIFIER__PDF___WORD_.json )
![image](https://github.com/user-attachments/assets/9e45ee36-2be6-4cd1-b7f9-aa7376e451d2)

### Description: 
Monitors a Gmail account for emails with PDF or Word attachments. Extracts text accordingly. Looks up job details from a Google Sheet

## Daily Google Analytics Summary : (AI_Google_analytics.json )
![image](https://github.com/user-attachments/assets/9bf0fc71-5243-444a-8309-5c8e46a61f86)

### Description: 
Fetches yesterday's Google Analytics data (users, location, device, source, etc.). Filters out data from the US and Canada. Aggregates key metrics. Uses AI to generate a structured HTML summary report. Sends the report to a designated Telegram chat. (Note: Currently set to manual trigger, but processes daily data).

## Outlook CV Analysis & Feedback Responder : (AI_EMAIL CV ANALYSER.json )
![image](https://github.com/user-attachments/assets/c72e6ceb-d262-46f0-8724-33d53f32b737)

### Description :
Monitors a Microsoft Outlook inbox for emails with PDF attachments. Extracts text from the CV. Uses AI to generate an analysis including suggested jobs and improvement tips. Formats the analysis using basic HTML and sends it as an email reply to the sender. Also uploads the original CV attachment to Google Drive.

## Assertiveness Assessment & Report Generation (Test Orientation)
![image](https://github.com/user-attachments/assets/6028f7a6-85fa-48ec-8413-19ca0f1db274)

### Description :
his n8n workflow automates the analysis of assertiveness questionnaire responses. It takes input from a webhook, uses a language model to evaluate the responses and generate a personality profile, creates a pie chart visualization, and produces a styled .doc report with analysis, and stores all generated content in Google Drive.



# Make.com

### Web Scraping and Lead Extraction with Apify & Make.com : (Scraping the web and getting Leads (Apify) )
![image](https://github.com/user-attachments/assets/5e4011fb-3f73-46d2-bc0c-0022f71d713d)

### Description:
This automation scrapes Google search results using Apify's Google Search Scraper actor, waits briefly to ensure data is ready, then fetches the resulting dataset (up to 100 entries) in JSON format. It's ideal for generating lead lists, extracting relevant links, or researching specific topics. You can change the search query ("python" in this case) to target different keywords and collect updated leads automatically.


