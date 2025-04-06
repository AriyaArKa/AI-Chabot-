# 🩺 Virtual AI Assistant (Doctor)

A modern, responsive web-based chatbot that simulates interaction with a virtual doctor named **Dr. Yasir**. Powered by the **Groq LLaMA3 8B** AI model, this assistant provides answers to medical queries in real time.

---

## 🌟 Features

- 🧠 AI-generated doctor responses using Groq LLaMA3  
- 💬 Real-time user & bot chat interface  
- 🌙 Dark-themed, responsive UI with Bootstrap 5  
- ⚡ Built-in scrollable chat window  
- 🔐 Secure back-end request using PHP + `cURL`

---

## 📁 File Structure

project-root/ │ ├── index.html # Frontend HTML, CSS, and JS ├── api.php # Backend PHP for Groq API integration └── README.md # Documentation

yaml
Copy
Edit

---

## 🎯 How It Works

1. **User Input:** User types a message in the input field.
2. **Send Request:** The message and role prompt are sent via JavaScript to the PHP backend.
3. **API Call:** `api.php` sends the input to Groq's LLaMA3 model via HTTP POST request.
4. **AI Response:** The model responds in the voice of "Dr. Yasir".
5. **Display Message:** The reply is shown in the chat interface under "Dr. Yasir".

---

## 🧠 Technologies Used

### 🖥️ Frontend
- HTML5, CSS3
- Bootstrap 5.3.3
- Google Fonts: [Inter](https://fonts.google.com/specimen/Inter)
- Vanilla JavaScript

### 🔙 Backend
- PHP with `cURL`
- Groq API (LLaMA3-8B-8192 model)

---

## ⚙️ Setup Instructions

### Prerequisites
- PHP installed (≥ v7.4)
- Internet access
- Groq API key

### Step-by-Step

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/virtual-doctor-chatbot.git
   cd virtual-doctor-chatbot
Update API Key Open api.php and replace:

php
Copy
Edit
$secretKey = 'YOUR_API_KEY_HERE';
Run the Project Locally

bash
Copy
Edit
php -S localhost:3000
Then open your browser at:
👉 http://localhost:3000

🛡️ Security Note
The API key is currently hardcoded:

php
Copy
Edit
$secretKey = 'gsk_xxx...';
🔐 For production, move this to an environment variable and load it securely to avoid exposing your key.

💬 Example Conversation
User:

What are the symptoms of high blood pressure?

Dr. Yasir:

High blood pressure often has no symptoms, but some people may experience headaches, dizziness, or blurred vision...

🧩 Future Enhancements
Save conversation history

Add voice input (speech-to-text)

Support multiple medical roles (e.g., cardiologist, pediatrician)

Use environment variables for API keys

Add loading indicator per message (streaming support)

📜 License
This project is licensed under the MIT License. Feel free to use, modify, and distribute it.

🙌 Credits
Groq API

Bootstrap

Google Fonts - Inter