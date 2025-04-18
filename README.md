# 🩺 Virtual AI Assistant (Doctor) – Chat App using LLaMA 3 API

A lightweight, stylish, and responsive web-based chatbot application built with PHP, JavaScript, and Bootstrap. This project integrates **Groq's LLaMA 3 model** to simulate a virtual doctor—Dr. Yasir—who provides intelligent responses based on user queries.

---

## 🔍 Features

- 🧠 AI-Powered Doctor (Dr. Yasir) using LLaMA 3 (8B) model  
- 💬 Chat-style user interface with dark theme  
- ⚡ Instant AJAX responses with loading indicator  
- ✅ Form validation and error handling  
- 🎯 Clean and modern UI using Bootstrap 5 and custom styles

---

## 🛠️ Tech Stack

| Frontend | Backend | AI Model |
|----------|---------|----------|
| HTML, CSS, JS (Vanilla) | PHP (API call via `cURL`) | LLaMA 3 (via Groq API) |
| Bootstrap 5 | JSON handling | `llama3-8b-8192` |

---

## 🚀 How It Works

1. User types a query into the input field.
2. JavaScript fetches the response via a PHP script (`api.php`) using the Groq API.
3. The backend uses the provided `role` and `prompt` to query the LLaMA 3 model.
4. The model's response is displayed dynamically in a chat bubble.

---

## 📂 Project Structure

```
📁 your-project-root/
├── api.php           # PHP script to connect with Groq's LLaMA 3 model
├── index.html        # Main frontend interface
├── style (inline)    # Custom dark theme styles
```

---

## 🧪 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/AriyaArKa/AI-Chabot.git
cd AI-Chabot
```

### 2. Configure the API Key

Edit `api.php` and replace the placeholder:

```php
$secretKey = 'YOUR_GROQ_API_KEY_HERE';
```

> 🔐 **Important**: Never expose this key on the frontend or commit it to public repositories.

### 3. Run Locally

You can use any local server like XAMPP, WAMP, or PHP’s built-in server:

```bash
php -S localhost:3000
```

Visit: [http://localhost:3000](http://localhost:3000)

---

## 🖼️ Screenshots

### Index Page

![Index_Page](images/pic1.png)

### Chat Page

![Chat Page](images/pic2.png)
![Chat Page](images/pic3.png)

---

## ✅ Example Role & Prompt

The system instructs the model to act as:

```txt
Role: "You act as a Doctor named Yasir."
Prompt: "I have a headache and fever. What should I do?"
```

Expected response will be from **Dr. Yasir**, offering medical guidance powered by LLaMA 3.

---

## ⚠️ Disclaimer

This app is for **educational/demo purposes only** and should not be used for actual medical advice or diagnosis.

---

## 📃 License

MIT License

---

## 🙌 Acknowledgements

- [Groq API](https://console.groq.com/) for ultra-fast LLaMA 3 inference
- [Bootstrap 5](https://getbootstrap.com/) for beautiful UI components