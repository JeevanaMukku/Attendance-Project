# Attendance-Project
# AI-Powered Video Generation Workflow (n8n + Google Gemini)

## Overview
This project automates short video creation using **n8n**, **Google Gemini**, and **Google Sheets**.  
It generates video ideas, formats them into structured prompts, creates videos using the **Gemini VEO-3 API**, and logs all results automatically.

---

## Features
- End-to-end automation: idea → prompt → video → log  
- Gemini used for creative ideation  
- Google Sheets used for metadata and logging  
- Daily trigger via n8n Scheduler  
- LangChain for structured prompt formatting  
- Video generation through VEO-3 API  

---

## Architecture

---

## Workflow Nodes

| Node | Purpose |
|------|----------|
| Schedule Trigger | Runs daily |
| Google Gemini Chat | Generates video ideas |
| LangChain Parser | Converts ideas into structured format |
| Google Sheets | Stores metadata and URLs |
| Code Node (JS) | Handles logic and formatting |
| HTTP Request | Sends data to VEO-3 API |
| Wait Node | Waits for video rendering |
| Google Sheets Update | Logs video URL and status |


{
  "caption": "Ocean Rebirth",
  "idea": "Polluted bay becomes clear ocean",
  "environment": "Aerial cinematic shots",
  "sound": "Ambient waves, rising crescendo"
}
