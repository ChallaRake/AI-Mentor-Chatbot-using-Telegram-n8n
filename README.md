# 🤖 AI Mentor Chatbot — n8n + Telegram + Gemini

This project is an automated AI-based chatbot designed to help students clarify doubts in subjects like Python, EDA, Machine Learning, and Deep Learning. It is built using **n8n**, integrated with **Telegram Bot API**, and powered by the **Google Gemini AI Model**.  
The bot interacts with users conversationally, collects input, and generates accurate, friendly AI responses.

---

## 📌 Features

- ✔️ Works through Telegram messaging  
- ✔️ Recognizes user greetings and responds interactively  
- ✔️ Collects subject selection via form dropdown  
- ✔️ Captures free-text academic doubts  
- ✔️ AI-powered responses using Gemini  
- ✔️ Conversation memory for context continuity  
- ✔️ Beginner-friendly tone and structured answers  

---

## 🛠️ Tech Stack

| Component | Technology Used |
|----------|----------------|
| Automation Platform | **n8n** |
| Messaging Interface | **Telegram Bot API** |
| AI Model | **Google Gemini (via LangChain)** |
| Memory System | LangChain Conversation Memory |
| Integration Method | REST Webhook + Form-based Input |

---

## 🗂️ Workflow Overview

The workflow follows the steps below to guide the user through an interactive experience:

1. **Telegram Trigger**  
   The bot listens for any incoming message from a user and starts the workflow.

2. **Greeting Detection (If Node)**  
   The system checks whether the user has sent a greeting (hi/hello/hey).  
   If not, the workflow ends.

3. **Ask for Subject (Interactive Form)**  
   The user is prompted to select a subject from a dropdown menu.

4. **Collect User Doubt (Free Text Input)**  
   Once a subject is selected, the bot asks:  
   _"What is your doubt in <subject>?"_

5. **AI Processing (LangChain Agent + Gemini)**  
   The AI model receives:
   - The selected subject  
   - The user’s doubt  
   - The system prompt with tone and rules  

   It generates a clear and student-friendly response.

6. **Response Delivery (Telegram Text Message)**  
   The final answer is sent back to the user directly in Telegram.

7. **Conversation Memory**  
   The system stores short-term history to support natural conversation.

---

## 📦 Installation & Setup

### 1️⃣ Install Tools

- Install **n8n**
- Create a **Telegram Bot** using @BotFather
- Generate a **Google Gemini API Key**

---

### 2️⃣ Configure Credentials in n8n

| Credential Type | Required |
|----------------|----------|
| Telegram API Key | ✔️ |
| Google Gemini API Key | ✔️ |

---

### 3️⃣ Import the Workflow

Use the exported JSON file in:

```bash
AI Mentor Chatbot Project.json
```
---

## 🧠 Memory & Behavior

- Stores up to 50 previous messages
- Maintains tone as supportive and beginner-friendly
- Requests clarification if user input is incomplete

---

## 📹 Demo Video

👉 **Watch the full workflow demo here:**  
### [*AI Mentor Chatbot Automation*](https://www.linkedin.com/posts/challa-rakesh-reddy_automation-n8n-telegrambot-activity-7398699428133552128-_0gw?utm_source=share&utm_medium=member_desktop&rcm=ACoAAD7NTjAB5LIcCGe6w75x6giyS2sV95rQD14)

---

<img width="1625" height="803" alt="Screenshot 2025-11-22 175846" src="https://github.com/user-attachments/assets/11b71a16-73bb-4fe4-81f6-a0e1fc33c303" />


