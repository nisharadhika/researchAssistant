# 🚀 AI-Powered Research Assistant (Chrome Extension + Spring Boot Backend)

An **innovative AI-powered research assistant Chrome extension** designed to **enhance research efficiency** directly within the browser.
This project demonstrates **full-stack AI integration** using **Chrome Extension frontend + Spring Boot backend + Google Gemini API**.
---

## ✨ Features

* 📝 **Summarization**
  Select text on any webpage and click the **Summarize button**. The extension sends the request to a backend server powered by **Spring Boot & Spring AI**, which communicates with **Google Gemini API** to return a concise summary.

* 📌 **In-Browser Note-Taking**
  Take and store personal notes within the extension itself. Notes are saved using **Local Storage**, ensuring they persist across browser sessions and navigation.

---

## 🏗️ Architecture Overview

**Frontend (Chrome Extension)**

* Built with **HTML, CSS, JavaScript**
* User interface implemented as a **Side Panel** in Chrome
* Handles text selection, note-taking, and sending requests to the backend

**Backend (Spring Boot + Spring AI)**

* REST APIs for summarization and data handling
* Built with:

  * `spring-boot-starter-web` → REST API development
  * `spring-boot-starter-webflux` → Async API calls with WebClient
  * `lombok` → Boilerplate code reduction
* Handles interaction with **Google Gemini API** for AI operations

**AI Model Integration**

* Integrates with **Google Gemini API**
* JSON-based request/response handling for operations like summarization
* Can be extended to support other AI models

---

## 📂 Project Structure

```
research-assistant/
│── extension/                # Chrome Extension frontend
│   ├── manifest.json
│   ├── popup.html
│   ├── styles.css
│   ├── script.js
│   ├── notes.js
│   └── theme-toggle.js
│
│── backend/                  # Spring Boot Backend
│   ├── src/main/java/com/... # API Controllers, Services
│   ├── pom.xml
│   └── application.properties
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 🔹 1. Clone the repository

```bash
git clone https://github.com/your-username/research-assistant.git
cd research-assistant
```

### 🔹 2. Setup the Backend (Spring Boot)

* Open the backend folder in **IntelliJ / VS Code**
* Install dependencies:

```bash
mvn clean install
```

* Add your **Google Gemini API Key** in `application.properties`:

```properties
gemini.api.key=YOUR_API_KEY
```

* Run the Spring Boot app:

```bash
mvn spring-boot:run
```

* Backend will be available at `http://localhost:8080`

### 🔹 3. Setup the Chrome Extension

* Open Chrome → `chrome://extensions/`
* Enable **Developer Mode** (top-right corner)
* Click **Load Unpacked** → Select the `extension/` folder
* The extension will appear in your browser toolbar 🎉

---

## 🖼️ Demo 

* 🔍 Text Selection & Summarization
* 📝 Notes Panel



https://github.com/user-attachments/assets/7c9ecc22-1f10-4560-a6d1-18e36e1f4e82


---

## 🚀 Future Enhancements

* 🔑 User Authentication (sync notes across devices)
* ☁️ Cloud Database support (instead of local storage)
* 📑 PDF summarization support
* 🗂️ Export notes in Markdown / PDF

---

## 👩‍💻 Tech Stack

* **Frontend**: HTML, CSS, JavaScript (Chrome Extension APIs)
* **Backend**: Spring Boot, Spring AI, WebFlux, Lombok
* **AI**: Google Gemini API
* **Storage**: Local Storage (Browser)

---

## 📌 Author

👩‍💻 Developed by Radhika 
