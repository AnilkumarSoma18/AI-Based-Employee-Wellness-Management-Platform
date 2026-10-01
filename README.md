# MoodMentor
## AI-Based Employee Wellness Management Platform

### Live Application
https://moodmentor-anil.streamlit.app/

---

## 1. Project Overview

MoodMentor is an AI-based Employee Wellness Management Platform developed to provide employees with a private digital environment for recording, understanding, and reflecting on their emotional wellbeing.

The platform combines Natural Language Processing, sentiment analysis, emotion detection, conversational AI, secure authentication, database management, analytics, and report generation into a single application.

Instead of treating employee wellness as only structured questionnaire data, MoodMentor allows employees to communicate naturally through journal entries and wellness conversations. The platform processes this unstructured text and converts it into understandable wellness insights.

The core idea is simple:

Employees express how they feel in their own words, the AI analyzes the language, and the platform presents the resulting information in a structured and understandable form.

---

## 2. Problem Statement

Employee wellness is an important part of a healthy and productive working environment.

However, employees do not always have a convenient way to record their feelings, understand changes in their mood, or reflect on their workplace experiences.

Traditional employee management systems mainly focus on operational information such as attendance, tasks, performance, and organizational records.

They generally do not provide an intelligent interface where employees can communicate naturally and receive immediate AI-assisted wellness insights.

MoodMentor addresses this gap by introducing an AI and NLP layer into employee wellness management.

---

## 3. Proposed Solution

MoodMentor provides a centralized platform where an authenticated employee can:

1. Create and manage an account.
2. Record thoughts and experiences through a mood journal.
3. Submit natural-language text for AI/NLP analysis.
4. Obtain sentiment and emotion information from the submitted text.
5. Interact with a wellness-oriented conversational interface.
6. Complete structured wellness questionnaires.
7. Receive general wellness recommendations.
8. Review personal wellness-related information.
9. Generate reports and export relevant information.

The platform therefore combines structured information from questionnaires with unstructured information from natural-language communication.

---

## 4. How Artificial Intelligence Is Used

AI is not used only as a decorative component of the application.

It is directly involved in the processing of employee-generated text.

When an employee submits a journal entry, the system processes the text through an NLP pipeline.

The general processing flow is:

User Text
→ Text Processing
→ Language Detection
→ Normalization
→ NLP Analysis
→ Sentiment Analysis
→ Emotion Analysis
→ Confidence Estimation
→ Wellness Insight

This allows the application to transform free-form human language into structured information that can be displayed to the user.

For example, an employee may write:

"I had a stressful day at work, but after completing my tasks I feel much better."

Instead of simply storing this sentence as text, the platform analyzes the content and produces structured results such as sentiment, emotion, and confidence information.

---

## 5. Mood Journal

The Mood Journal is one of the main AI features of the platform.

Employees can describe their experiences using natural language rather than selecting only predefined options.

The submitted text is sent to the backend for processing.

The system analyzes the text and returns information including:

- Sentiment
- Emotion
- Confidence
- Processed wellness information

The result is then displayed through the application interface.

This approach allows the platform to work with unstructured employee communication rather than relying exclusively on predefined forms.

---

## 6. Wellness Chat

MoodMentor also provides a conversational wellness interface.

The wellness chat allows employees to interact with the application using natural language.

The conversation is processed through the backend and is designed to provide general wellness-oriented support and interaction.

The purpose of this feature is to provide an accessible digital wellness interface rather than requiring employees to navigate only through structured forms.

---

## 7. Natural Language Processing

The NLP layer is responsible for processing employee-generated text before analysis.

The project incorporates capabilities including:

- Language detection
- Text cleaning
- Text normalization
- Unicode and text correction
- Stop-word processing
- Translation support
- Sentiment analysis
- Emotion analysis

The project uses Python NLP technologies including spaCy, VADER Sentiment, language detection, translation utilities, and transformer-based components.

This combination allows the application to process natural-language input and convert it into meaningful application-level information.

---

## 8. Multilingual Processing

Employee communication can occur in different languages.

For this reason, the platform includes multilingual NLP capabilities such as language detection, text normalization, translation, and multilingual processing.

The objective is to reduce the dependency on a single language and make natural-language interaction more accessible.

---

## 9. Wellness Questionnaire

In addition to free-form journal entries, MoodMentor provides structured wellness questionnaires.

This creates two different types of employee wellness information:

Natural-language information from journal entries and conversations.

Structured information from questionnaire responses.

Combining these sources provides a broader foundation for the application's wellness-oriented analysis.

---

## 10. Wellness Recommendations

The platform includes a recommendation component that provides general wellness-oriented suggestions based on available application information.

Recommendations can include areas such as:

- Relaxation
- Self-care
- Reflection
- Healthy routines
- General workplace wellness

The recommendation functionality is intended to support personal reflection and general wellbeing.

It is not designed to provide medical diagnosis or replace professional healthcare.

---

## 11. Authentication and Security

Because employee wellness information can be sensitive, authentication and security are fundamental parts of the application.

The platform includes:

- User registration
- User login
- Password hashing using bcrypt
- JWT-based authentication
- Protected backend endpoints
- Session management
- Email OTP verification
- Password recovery
- Secure password reset
- Environment-based configuration

Authentication ensures that protected application functionality is associated with the authenticated user.

Sensitive credentials are not intended to be stored directly in the source code.

---

## 12. Backend Architecture

The backend is implemented using Python and FastAPI.

FastAPI provides the REST API layer between the Streamlit application and the underlying services.

The backend handles functionality such as:

- Authentication
- User verification
- Mood analysis
- Wellness chat
- Questionnaire processing
- Database operations
- Protected API requests

The architecture separates the user interface from backend processing, allowing the application components to evolve independently.

---

## 13. Database

PostgreSQL is used as the application's persistent database.

The database manages information required by the platform, including:

- User accounts
- OTP records
- Mood logs
- Questionnaire responses

The database layer is separated from the frontend and API logic to provide a structured persistence layer for the application.

---

## 14. Technology Stack

Programming Language:

Python

Frontend:

Streamlit

Backend:

FastAPI  
Uvicorn

Artificial Intelligence and NLP:

Natural Language Processing  
Sentiment Analysis  
Emotion Detection  
spaCy  
VADER Sentiment  
Transformers  
Language Detection  
Translation and multilingual processing

Database:

PostgreSQL  
psycopg2

Authentication and Security:

JWT  
bcrypt  
OTP verification  
Environment-based secrets

Data Processing and Visualization:

Pandas  
Matplotlib  
Seaborn

Reporting:

ReportLab

Deployment:

Streamlit Community Cloud  
FastAPI backend  
PostgreSQL / Neon database

---

## 15. Project Architecture

The application follows a layered architecture.

The Streamlit frontend provides the user interface.

The FastAPI backend provides the application and API layer.

The NLP pipeline performs language processing and analysis.

The authentication layer protects user-specific functionality.

The PostgreSQL database provides persistent storage.

Conceptually, the application works as:

Frontend
→ FastAPI Backend
→ Authentication / Application Services
→ NLP and AI Processing
→ PostgreSQL Database

This separation makes the application easier to maintain, test, and extend.

---

## 16. Project Structure

```text
AI-Based-Employee-Wellness-Management-Platform/

├── .devcontainer/

├── Milestone1/

├── Milestone2/

├── Milestone3/

├── Milestone4/
│
├── .dockerignore
├── .env.example
├── .gitignore
├── DEPLOYMENT.md
├── Dockerfile.backend
├── Dockerfile.frontend
├── docker-compose.yml
├── README.md
│
├── app.py
├── auth.py
├── backend.py
├── db.py
├── email_utils.py
├── nlp_pipeline.py
├── recommendations.py
├── security.py
│
└── requirements.txt
