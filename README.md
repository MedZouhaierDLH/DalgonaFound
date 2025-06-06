# IHEC Chatbot

## Introduction
The IHEC Chatbot is designed to provide automated, efficient, and intuitive responses to frequently asked questions from students of the **Institut des Hautes Études Commerciales (IHEC)**. The chatbot aims to improve access to information on topics like administration, courses, registration, schedules, and exams.

## Objectives
- Provide 24/7, fast, and automated responses to students' queries.
- Ensure integration with IHEC's existing web infrastructure.
- Adhere to IHEC's branding and security standards.

## Features
### Core Functionalities
- **Automated FAQs**: Responds to common questions like "What documents are needed for registration?".
- **Guided Navigation**: Redirects students to relevant resources like forms or schedules.
- **Keyword Search**: Searches for terms like "schedule" or "registration".
- **Multilingual Support**: Supports both French and English.

### Optional Features
- **Feedback System**: Improve response accuracy based on user feedback.
- **Usage Statistics**: Provide insights for the administrative team.

## Technical Overview
### Architecture
- **Front-End**: Built with Next.js and styled using Tailwind CSS.
- **Back-End**: A microservice using Node.js and TensorFlow, powered by the `sentence-transformers/distiluse-base-multilingual-cased-v2` model.
- **Database**: JSON/CSV for local data storage, populated via web scraping.

### Data Flow
1. User inputs a question in the chatbot interface.
2. The question is sent to the server for processing.
3. The NLP model processes the query and retrieves the most relevant answer.
4. The response is displayed in the user interface.

### Deployment
- **Front-End**: Hosted locally or on platforms compatible with Next.js.
- **Back-End**: TensorFlow service deployed via Docker or a local Node.js server.

## Security
- Fully compliant with GDPR.
- Data encryption (SSL/TLS) for all communications.
- No storage of sensitive personal data (emails, phone numbers).
- Access to collected data is restricted to authorized administrators.

## Installation and Setup
### Prerequisites
- **Node.js** and **npm** installed.
- **Docker** (optional for TensorFlow deployment).

### Steps
1. Clone this repository:
   ```bash
   git clone https://github.com/MedZouhaierDLH/DalgonaFound
