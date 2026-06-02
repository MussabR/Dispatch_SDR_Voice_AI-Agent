# Dispatch SDR Voice AI Agent

This project automates outbound sales calls for JMF Freight using AI. It qualifies truck drivers, identifies their equipment type, and books meetings with specialists.

## Features
- **Automated Outbound Calling**: Integrated with VAPI for human-like AI conversations.
- **Data Enrichment**: Automatically captures Name, Email, MC/DOT, and Equipment Type.
- **Workflow Automation**: Built on n8n to manage leads from Google Sheets, trigger calls, and update statuses in real-time.
- **Intelligent Routing**: Handles data verification and meeting scheduling seamlessly.

## How it Works
1. **Lead Source**: A Google Sheet containing lead phone numbers and existing data.
2. **n8n Automation**: 
   - Filters pending leads.
   - Triggers calls via VAPI API.
   - Extracts structured data (Name, Email, MC/DOT, Truck Type) from call reports.
   - Updates Google Sheets with call outcomes.
3. **Voice AI**: Tara (AI Agent) qualifies leads and schedules callbacks.

## Setup Instructions
1. **VAPI Configuration**: 
   - Setup an Assistant with the provided system prompt.
   - Configure Structured Outputs for data extraction.
2. **n8n Workflow**: Import the provided JSON workflow.
3. **Credentials**: Add your VAPI API Key and Google Sheets OAuth credentials to n8n.