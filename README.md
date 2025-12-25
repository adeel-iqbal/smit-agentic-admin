# 🎓 SMIT Agentic Admin

> **AI-Powered Autonomous Student Management System**  
> Built with LangGraph Multi-Agent Architecture | Real-Time Database Operations | Automated Communications

[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/)
[![LangGraph](https://img.shields.io/badge/LangGraph-Latest-green.svg)](https://langchain-ai.github.io/langgraph/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.104+-teal.svg)](https://fastapi.tiangolo.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-15+-blue.svg)](https://www.postgresql.org/)

---

## 📋 Overview

**SMIT Agentic Admin** is an enterprise-grade autonomous administration system designed and built for **Saylani Mass IT Training (SMIT)**, this intelligent platform leverages advanced multi-agent AI architecture to automate student management, database operations, and mass communications through a conversational interface.

### 🎯 Key Highlights

- **🤖 Multi-Agent AI System** - LangGraph-powered autonomous decision-making
- **💬 Natural Language Interface** - Query databases and trigger actions conversationally
- **📧 Automated Communications** - Bulk emails via Gmail API & WhatsApp via Twilio
- **🎤 Voice-Enabled** - Full duplex voice interface with Speech-to-Text (STT) input & Text-to-Speech (TTS) responses
- **⚡ Real-Time Operations** - WebSocket-based instant updates
- **🗄️ Intelligent Database Management** - Dynamic SQL generation with safety checks
- **📊 Live Data Visualization** - HTML tables rendered in real-time

---

## 🚀 Features

### Core Capabilities

| Feature | Description |
|---------|-------------|
| **Natural Language Queries** | Ask questions like *"Show unpaid students"* - AI generates and executes SQL |
| **Automated Email Campaigns** | Send personalized fee reminders and attendance warnings to hundreds of students |
| **WhatsApp Integration** | Bulk WhatsApp messaging via Twilio API |
| **Voice Assistant** | Speak queries via STT (Web Speech API) and receive audio responses via TTS (Edge-TTS) |
| **Dynamic Course Management** | Update student courses, batches, and schedules autonomously |
| **Schema Introspection** | AI automatically discovers database structure |
| **Parallel Processing** | Send 100+ emails/messages concurrently |
| **Draft Management** | Create Gmail drafts for review before sending |

### Technical Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    Frontend (WebUI)                     │
│          HTML5 + CSS3 + JavaScript + WebSocket          │
└────────────────────┬────────────────────────────────────┘
                     │
            ┌────────▼────────┐
            │   FastAPI Server │
            │   (WebSocket)    │
            └────────┬─────────┘
                     │
        ┌────────────▼───────────────┐
        │   LangGraph Multi-Agent    │
        │   (OpenAI GPT-4o-mini)     │
        └────────┬───────────────────┘
                 │
    ┌────────────┼────────────┬──────────────┐
    │            │            │              │
┌───▼───┐  ┌────▼────┐  ┌────▼─────┐  ┌────▼────┐
│ Gmail │  │ Twilio  │  │ Supabase │  │ Edge-TTS│
│  API  │  │WhatsApp │  │PostgreSQL│  │  Voice  │
└───────┘  └─────────┘  └──────────┘  └─────────┘
```

---

## 📸 Screenshots

### User Interface & Conversational Queries

- Main Dashboard
- Natural Language Query
- Live Data Visualization
- Bulk Communication
- Voice-Enabled Chat
- Real-Time Status

<table>
  <tr>
    <td align="center">
      <img src="shots/preview1.png" width="400px" alt="Dashboard Overview"/>
    </td>
    <td align="center">
      <img src="shots/preview2.png" width="400px" alt="Database Query"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="shots/preview3.png" width="400px" alt="Data Results"/>
    </td>
    <td align="center">
      <img src="shots/preview4.png" width="400px" alt="Bulk Operations"/>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="shots/preview5.png" width="400px" alt="Voice Interface"/>
    </td>
    <td align="center">
      <img src="shots/preview6.png" width="400px" alt="System Status"/>
    </td>
  </tr>
</table>

### Database Architecture (Supabase PostgreSQL)

- Database Schema
- Student Management Tables
- Live Query Execution

<table>
  <tr>
    <td align="center">
      <img src="shots/preview7.png" width="400px" alt="Database Schema"/>
    </td>
    <td align="center">
      <img src="shots/preview8.png" width="400px" alt="Student Records"/>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="2">
      <img src="shots/preview9.png" width="400px" alt="Query Execution"/>
    </td>
  </tr>
</table>

### Communication Results

<table>
  <tr>
    <td align="center">
      <img src="shots/preview10.jpeg" width="300px" alt="WhatsApp Message"/>
      <br /><b>WhatsApp Message Received (Twilio)</b>
    </td>
    <td align="center">
      <img src="shots/preview11.jpeg" width="300px" alt="Email Draft"/>
      <br /><b>Drafted Fee Reminder Template</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img src="shots/preview12.jpeg" width="300px" alt="Drafts Folder"/>
      <br /><b>All Drafts in Gmail</b>
    </td>
    <td align="center">
      <img src="shots/preview13.jpeg" width="300px" alt="Email Template"/>
      <br /><b>Drafter Low Attendance Warning Template</b>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="2">
      <img src="shots/preview14.jpeg" width="300px" alt="Sent Messages"/>
      <br /><b>Successfully Sent Emails</b>
    </td>
  </tr>
</table>

---

## 🛠️ Technology Stack

### Backend
- **LangGraph** - Multi-agent orchestration & workflow management
- **LangChain** - LLM integration & tool binding
- **FastAPI** - High-performance async web framework
- **OpenAI GPT-4o-mini** - Natural language understanding
- **SQLAlchemy** - Database ORM & connection pooling
- **Supabase PostgreSQL** - Cloud-hosted relational database

### Communication APIs
- **Gmail API** - OAuth2-authenticated email sending
- **Twilio WhatsApp API** - Business messaging integration
- **Edge-TTS** - Microsoft's neural text-to-speech engine (TTS)
- **Web Speech API** - Native browser speech-to-text (STT)

### Frontend
- **WebSocket** - Real-time bidirectional communication
- **Web Speech API** - Browser-native speech recognition (STT)
- **Vanilla JavaScript** - No framework overhead, pure performance
- **Responsive CSS** - Mobile-first adaptive design
- **Font Awesome** - Professional iconography

---

## 📦 System Requirements

```yaml
Python: 3.11+
PostgreSQL: 15+
Node.js: Not required (pure vanilla JS)
Storage: 100MB minimum
RAM: 2GB minimum (4GB recommended)
Internet: Required for API calls
```

---

## ⚙️ Configuration Overview

The system uses the following integrations:

### 🗄️ Database
- PostgreSQL hosted on Supabase
- Connection pooling with SQLAlchemy
- Automatic schema introspection

### 📧 Gmail Integration
- OAuth 2.0 authentication flow
- Gmail API scopes: `send`, `compose`, `modify`
- Parallel email dispatch (10 concurrent threads)

### 📱 WhatsApp Integration
- Twilio API for WhatsApp Business
- Rate-limited messaging (0.3s delay)
- Support for international phone formats

### 🎤 Voice Features
- **STT (Speech-to-Text)**: Web Speech API for voice input
- **TTS (Text-to-Speech)**: Edge-TTS with Irish Female voice (Emily)
- 55% speed increase for natural conversational flow
- Automatic audio streaming via WebSocket
- Real-time transcription of user commands

---

## 🧠 AI Agent Architecture

### LangGraph Multi-Agent System

The system employs a **tool-calling agent** with the following capabilities:

```python
Tools Available:
├── inspect_database()      # Schema discovery
├── list_courses()          # Course enumeration  
├── query_db(sql)           # Safe SELECT execution
├── manipulate_db(sql)      # UPDATE/INSERT/DELETE
├── draft_email(...)        # Gmail draft creation
├── send_bulk_emails(...)   # Parallel email dispatch
├── send_bulk_whatsapp(...) # Parallel WhatsApp messaging
└── send_single_whatsapp(...) # Direct message sending
```

### Intelligent Decision Flow

1. **User Input** → Natural language query
2. **Schema Check** → Agent inspects database if uncertain
3. **SQL Generation** → Constructs safe, optimized queries
4. **Execution** → Runs query with connection pooling
5. **Response Formatting** → HTML tables for UI + voice summary
6. **Action Triggers** → Automatically drafts/sends communications

---

## 📊 Use Cases

### 1️⃣ **Fee Management**
```
User: "Show all unpaid students in AI & DS course"
AI: [Queries DB] → [Displays 3 students] → "Found 3 unpaid students from the AI & Data Science Course"
User: "Email them"
AI: [Sends 3 personalized fee reminder emails in parallel]
```

### 2️⃣ **Attendance Tracking**
```
User: "Find students with attendance below 80%"
AI: [Joins students + courses tables] → "Found 12 students with attendance below 80%"
User: "Draft them"
AI: [Creates 12 Gmail drafts with attendance data]
```

### 3️⃣ **Batch Management**
```
User: "Move Ahmed's slot from Mon-Wed-Fri to Tue-Thur, if seats available"
AI: [Finds target batch] → [Updates batch_id] → [Auto-adjusts seat counts]
```

### 4️⃣ **WhatsApp Campaigns**
```
User: "Send WhatsApp to 033239***** saying 'Your next class is tomorrow'"
AI: [Formats number] → [Sends via Twilio] → "✅ Message sent"
```

---

## 🎯 Performance Metrics

| Metric | Value |
|--------|-------|
| **Average Response Time** | 2-4 seconds |
| **Bulk Email Speed** | 100 emails in ~15 seconds |
| **Database Query Time** | <500ms (with indexes) |
| **Concurrent Connections** | 20 simultaneous users |
| **WebSocket Latency** | <100ms |
| **Voice Synthesis** | ~1.5s for 240 characters |

---

## 🏆 Project Context

This system was developed during my tenure as an **AI/ML Intern at SaylaniTech**, following my certification in **AI & Data Science from Saylani Mass IT Training (SMIT)**. The project showcases enterprise-level AI engineering, full-stack development, and production-ready system design.

### Built For
**Saylani Mass IT Training (SMIT)**  
Pakistan's largest non-profit IT training institute, serving 100,000+ students annually across 10+ cities.

---

## 💼 Custom Development & Licensing

### 🚀 Want This For Your Institute?

This system is available as a customizable product for educational institutions, training centers, and organizations managing large student databases. Whether you need this exact solution or something tailored to your specific requirements, I offer:

- ✅ **Custom Deployment** - Tailored to your infrastructure
- ✅ **Feature Extensions** - SMS integration, LMS connections, payment gateways and more
- ✅ **White-Label Branding** - Your logo, colors, domain
- ✅ **Training & Support** - Full documentation & onboarding
- ✅ **Multi-Tenant Architecture** - Host multiple institutes on one platform

### 📫 Contact Me

**Adeel Iqbal Memon**  
AI/ML Engineer | Full-Stack Developer

- 📧 Email: [adeelmemon096@yahoo.com](mailto:adeelmemon096@yahoo.com)
- 💼 LinkedIn: [linkedin.com/in/adeeliqbalmemon](https://linkedin.com/in/adeeliqbalmemon)
- 🐙 GitHub: [@adeel-iqbal](https://github.com/adeel-iqbal)

> 💡 **Enterprise Inquiries Welcome** - I provide consultancy for AI-powered automation solutions, LangGraph implementations, and scalable multi-agent systems.

---

## 🙏 Acknowledgments

- **Saylani Welfare Trust** - For world-class free IT education
- **LangChain Team** - For the incredible LangGraph framework
- **OpenAI** - For GPT-4o-mini API access
- **Supabase** - For reliable PostgreSQL hosting

---

## ⭐ Support This Project

If you find this project useful, please consider:
- Giving it a ⭐ on GitHub
- Sharing it with your network
- Contributing feedback or ideas
- Reaching out for collaboration

---

<div align="center">

**Built with ❤️ by Adeel Iqbal Memon**

*Empowering education through AI automation*

[⬆ Back to Top](#-smit-agentic-admin)

</div>
