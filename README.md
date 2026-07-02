# 🌤 Daily Weather Report to Telegram using n8n

An automated workflow built with **n8n** that retrieves the latest weather information from the **Open-Meteo API** and sends a formatted daily weather report directly to **Telegram**.

This project demonstrates API integration, scheduled automation, data transformation, and Telegram bot notifications using only free services.

---

## 📌 Overview

This workflow automatically performs the following tasks:

- Runs every day at a scheduled time.
- Retrieves the latest weather data from the Open-Meteo API.
- Extracts the current weather information.
- Converts weather codes into readable weather conditions.
- Sends a formatted weather report to Telegram.

---

## 🚀 Features

- ⏰ Daily scheduled execution
- 🌤 Real-time weather updates
- 🌡 Displays temperature, humidity, wind speed, and weather conditions
- 📲 Telegram notification
- 🌐 Free Open-Meteo API
- 🔑 No API key required
- 💯 Fully automated

---

## 🛠 Tech Stack

- n8n
- Open-Meteo API
- HTTP Request
- Code Node (JavaScript)
- Telegram Bot API

---

## 📂 Workflow

```text
Schedule Trigger
        │
        ▼
HTTP Request
        │
        ▼
Edit Fields (Set)
        │
        ▼
Code
        │
        ▼
Telegram
```

---

## ⚙️ Workflow Explanation

### 1. Schedule Trigger

Automatically runs the workflow every day at the configured time.

---

### 2. HTTP Request

Retrieves the latest weather information from the Open-Meteo API.

**API Endpoint**

```
https://api.open-meteo.com/v1/forecast
```

**Method**

```
GET
```

**Authentication**

```
None
```

---

### 3. Edit Fields (Set)

Extracts only the required weather information from the API response, including:

- Temperature
- Relative Humidity
- Wind Speed
- Weather Code

---

### 4. Code

Converts the weather code into a human-readable weather condition.

Examples:

- ☀️ Clear Sky
- 🌤 Mainly Clear
- ⛅ Partly Cloudy
- ☁️ Overcast
- 🌧 Rain
- ⛈ Thunderstorm

It also formats the final weather report before sending it to Telegram.

---

### 5. Telegram

Sends the formatted weather report directly to your Telegram account.

---

## 📱 Example Output

```
🌤 Daily Weather Report

📍 Cebu City

🌡 Temperature: 29°C
💧 Humidity: 76%
🌬 Wind Speed: 11 km/h
☁️ Weather: ⛅ Partly Cloudy

Have a wonderful day!

🤖 Generated automatically with n8n.
```

---

## 📁 Project Structure

```
Daily-Weather-Report/
│
├── README.md
├── workflow.json
└── screenshots/
    ├── workflow.png
    ├── workflow-execution.png
    └── telegram-output.png
```

---

## 📸 Screenshots

Include the following screenshots:

- Workflow Editor
- Successful Workflow Execution
- Telegram Output

Example:

```
screenshots/
    workflow.png
    workflow-execution.png
    telegram-output.png
```

---

## 💡 Use Cases

- Daily weather monitoring
- Morning weather updates
- Travel planning
- Outdoor activity planning
- Learning API integration with n8n
- Portfolio automation project

---

## 🔮 Future Improvements

- Support multiple locations
- 7-day weather forecast
- Rain and storm alerts
- Save weather history to Google Sheets
- Send weather reports via Email or Discord
- Generate AI-powered weather summaries
- Add weather charts and graphs

---

## 📚 What I Learned

This project helped me gain hands-on experience with:

- Workflow automation using n8n
- REST API integration
- HTTP Request node
- JSON parsing
- Data transformation
- JavaScript Code node
- Telegram Bot integration
- Scheduled workflows

---

## 🏷 Skills Demonstrated

- n8n
- Workflow Automation
- REST API
- HTTP Request
- JSON Parsing
- JavaScript
- Data Transformation
- Telegram Bot API
- Scheduled Automation
- No-Code / Low-Code Development

---

## 📄 License

This project is licensed under the MIT License.

---

⭐ If you found this project helpful, consider giving it a star!
