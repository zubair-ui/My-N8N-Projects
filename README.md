# My N8N Projects

This repository contains my personal **n8n workflow collection**, where I experiment, automate, and learn automation development using [n8n](https://n8n.io/).  
Each folder contains a workflow JSON file that can be directly imported into your self-hosted or cloud n8n instance.

---

## Projects Overview

### 1) First N8n Workflow

A simple AI-powered workflow integrating **Google Gemini Chat Model** with **LangChain Agent**, **memory buffer**, and a **calculator tool**.  
This was my first experiment with n8n’s AI Agent framework to test conversational memory and tool usage.

**Highlights:**

- Uses **Google Gemini (PaLM)** for chat-based AI responses.
- Includes **memory persistence** and **calculation capabilities**.
- Serves as a base template for future AI workflows.

---

### 2) Calendar Planner Agent

An intelligent calendar assistant built with **LangChain Agent + Google Calendar** integration.  
It can find available time slots and create events automatically via AI conversation.

**Highlights:**

- Uses **Google Calendar API** (OAuth2).
- AI agent determines and schedules events dynamically.
- Built-in memory for contextual conversation flow.

---

### 3) Daily Weather Digest (Email)

Automatically sends a daily and tomorrow weather report for **Karachi** at noon via email.  
Data is fetched from the **Open-Meteo API** and formatted into a colorful HTML email.

**Highlights:**

- Scheduled daily trigger at **12 PM**.
- Fetches live weather + daily forecast.
- HTML email with emojis, weather icons, and adaptive background colors.
- Can be customized for any city by changing latitude/longitude.

---

### 4) Daily Tech News Digest

Sends the **top 3 technology headlines** daily via email using the **NewsData.io** API.  
The workflow formats articles into a minimal, light-themed HTML newsletter.

**Highlights:**

- Scheduled daily trigger at **12 PM**.
- Fetches latest tech headlines (top 3).
- Sends clean HTML email digest via SMTP.
- 💡 **Note:** The API key has been removed.  
  ➤ Visit [NewsData.io](https://newsdata.io/) to get your free key and replace it in the HTTP Request URL:
  ```
  https://newsdata.io/api/1/news?apikey=YOURAPIKEY&category=technology&language=en
  ```

---

## License

This repository is for **learning and personal automation** purposes.  
Feel free to fork and experiment — attribution is appreciated.
