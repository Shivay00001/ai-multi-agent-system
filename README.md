# AI Multi-Agent System

This repository is an **All-In-One Enterprise AI Automation Suite**. It contains 10 highly specialized, autonomous AI agents and 1 central orchestrator (Connector System) that ties them all together into dynamic, multi-agent workflows.

## The Architecture
Every agent is built using the same robust, standardized architecture:
- **Backend**: FastAPI (Python), LiteLLM (OpenAI, Anthropic, Gemini, GLM)
- **Frontend**: Next.js 15, React, Tailwind CSS
- **Database**: SQLite / PostgreSQL
- **Port Locking**: Each agent runs on a dedicated port (8001-8010) to avoid conflicts during orchestration.

## Included Agents

1. **Connector System (/connector-system) - Port 8012**
   - The Central Coordinator! It features a dynamic Pipeline Builder UI where you can string together multiple agents (e.g. SEO Node -> Email Node), map their outputs visually using intermediate LLM translation, and trigger synchronous or background pipelines natively!
   
2. **Ads Runner Agent (/ads-runner-agent) - Port 8007**
   - Generates and manages digital ad campaigns natively (Google Ads structure, keywords).

3. **Calling AI Agent (/calling-ai-agent) - Port 8006**
   - Voice-AI Sales agent powered by Twilio and OpenAI Realtime API for automated outbound calling.

4. **Data Analyst Agent (/data-analyst-agent) - Port 8002**
   - Analyzes datasets natively and produces SQL queries and visualizations.

5. **Data Scientist Agent (/data-scientist-agent) - Port 8001**
   - Python-capable autonomous agent for training machine learning models and data preprocessing.

6. **Email Outreach Agent (/email-ai-agent) - Port 8004**
   - Autonomous cold email sequencer powered by SendGrid.

7. **SEO Master Agent (/seo-master-agent) - Port 8009**
   - Automates On-Page SEO (HTML optimization), Off-Page (Link building), and Google My Business updates.

8. **Social Media Agent (/social-media-agent) - Port 8008**
   - Uses Buffer API to auto-generate and schedule native multi-platform social content.

9. **Software Engineer Agent (/software-engineer-agent) - Port 8003**
   - Autonomous coding agent that manages your workspace and builds production software.

10. **Website Optimizer Agent (/website-optimizer-agent) - Port 8010**
    - CRO and A/B Testing landing pages based on live metrics.

11. **WhatsApp Marketing Agent (/whatsapp-ai-agent) - Port 8005**
    - Twilio-powered conversational AI for lead qualification natively via WhatsApp.

## How to Run the Ecosystem
You can boot each agent individually using their respective \ackend\ and \rontend\ folders. 

To run the full system concurrently, we recommend booting the **Connector System** on port 8012, and then bringing up the specific agents you want to use in your pipeline!


## Prerequisites
- Required environment and dependencies

## Installation
Follow standard installation steps for this language.

