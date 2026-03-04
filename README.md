# Zoom Classmate Buddy - AI Lecture Assistant

An AI-powered system that converts unstructured lecture transcripts into structured insights and reminders using LLM agents and automation workflows.

The system processes transcripts from Zoom recordings, extracts key technical insights, generates summaries, and automatically sends reminders to students through integrated productivity tools.

---

## Features

- Fetches lecture transcripts from the Attendee Zoom bot API
- Uses LLM-powered agents (CrewAI + Gemini 1.5 Pro) for transcript analysis
- Generates structured outputs including summaries, key concepts, and assignments
- Automatically updates a Notion knowledge base
- Sends assignment reminders via Gmail API 

---

## Architecture

The system follows a simple LLM agent pipeline:
1. Transcript ingestion

Lecture transcripts are retrieved from the Attendee Zoom bot API or provided manually.

3. Agent-based analysis

A CrewAI agent powered by Gemini 1.5 Pro processes the transcript and performs:
- summarization
- key concept extraction
- task identification

3. Structured output generation

The LLM converts unstructured transcript data into structured information including summaries, technical concepts, and assignment reminders.

5. Workflow automation

The processed results are:
- stored in Notion via Notion API
- sent to students via Gmail notifications

---

## Technologies Used

- **Python**
- **CrewAI** – multi-agent workflow orchestration
- **Gemini Pro (Google GenAI)** – LLM processing
- **Notion API** – knowledge base integration
- **Gmail API** – automated reminders
- **Google OAuth 2.0** – authentication
