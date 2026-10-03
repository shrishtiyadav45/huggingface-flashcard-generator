 Hugging Face Flashcard Generator

A simple Generative AI-powered Flashcard Generator that uses the **Hugging Face API** to automatically create study flashcards from a given topic or text.

The application helps students convert study material into short **questions and answers**, making revision and learning easier.

---

## 📌 Features

* ✨ AI-generated flashcards
* 📝 Generate flashcards from a topic or study text
* 🤗 Uses Hugging Face AI models
* ⚡ Fast and simple generation
* 🎓 Useful for students and exam preparation
* 💻 Simple web-based interface
* 🔐 API token stored securely using environment variables
* 📱 Easy-to-use frontend

---

## 🛠️ Technologies Used

### Frontend

* HTML
* CSS
* JavaScript

### Backend

* Python
* Flask

### AI

* Hugging Face API
* Hugging Face Inference API

### Other Tools

* Python-dotenv
* GitHub
* VS Code

---

## 🏗️ Project Structure

```text
huggingface-flashcard-generator/
│
├── backend/
│   ├── app.py
│   └── requirements.txt
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── README.md
└── .gitignore
```

---

## ⚙️ How the Project Works

The application follows a simple flow:

```text
User enters a topic/text
        ↓
Frontend sends the request
        ↓
Flask Backend receives the input
        ↓
Backend sends the prompt to Hugging Face API
        ↓
Hugging Face AI generates flashcards
        ↓
Backend processes the response
        ↓
Flashcards are displayed on the website
```

### Step-by-step

1. The user enters a **topic or study material** in the web interface.
2. JavaScript sends the user's input to the Flask backend.
3. The Flask backend creates an AI prompt for generating flashcards.
4. The backend securely uses the **Hugging Face API token**.
5. The request is sent to the selected Hugging Face model.
6. The AI generates questions and answers based on the input.
7. The backend sends the generated result back to the frontend.
8. The flashcards are displayed to the user.

---

## 🔑 Hugging Face API Token

The Hugging Face token is required to communicate with the Hugging Face API.

For security, the token should **not** be written directly inside the Python code.

Create a `.env` file inside the `backend` folder:

```text
HF_TOKEN=your_hugging_face_token
```

Replace `your_hugging_face_token` with your actual Hugging Face token.

### ⚠️ Important

Never upload the `.env` file to GitHub.

The `.gitignore` file should contain:

```text
.env
venv/
.venv/
__pycache__/
*.pyc
```

---

## 💻 Installation and Setup

### 1. Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Move into the project directory:

```bash
cd huggingface-flashcard-generator
```

---

### 2. Create a Virtual Environment

Open the terminal inside the project folder and run:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

---

### 3. Install Dependencies

Go to the backend folder:

```bash
cd backend
```

Install the required Python packages:

```bash
pip install -r requirements.txt
```

---

### 4. Configure the Hugging Face Token

Create a file named:

```text
.env
```

inside the `backend` folder.

Add:

```text
HF_TOKEN=your_hugging_face_token
```

Do not share or upload this token publicly.

---

## ▶️ Running the Application

From the `backend` folder, run:

```bash
python app.py
```

After the Flask server starts, open the local URL shown in the terminal, for example:

```text
http://127.0.0.1:5000
```

Open this address in your web browser.

---

## 🧠 Flashcard Generation

For example, the user can enter:

```text
Topic: Photosynthesis
```

The AI can generate flashcards such as:

```text
Question:
What is photosynthesis?

Answer:
Photosynthesis is the process by which green plants
convert light energy into chemical energy.
```

The generated flashcards can then be used for quick revision.

---

## 📂 Important Files

### `backend/app.py`

Contains the Flask backend logic, API routes, Hugging Face API communication, and flashcard generation logic.

### `backend/requirements.txt`

Contains the Python dependencies required to run the backend.

### `frontend/index.html`

Contains the structure of the flashcard generator webpage.

### `frontend/style.css`

Contains the styling and visual design of the application.

### `frontend/script.js`

Handles user interaction, sends requests to the backend, and displays generated flashcards.

### `.env`

Stores the Hugging Face API token locally.

**This file must not be uploaded to GitHub.**

### `.gitignore`

Prevents sensitive and unnecessary files such as `.env`, `venv`, and `__pycache__` from being uploaded to GitHub.

---

## 🔒 Security

API credentials are stored using environment variables instead of being hard-coded into the application.

The following files should never be committed to the repository:

* `.env`
* API keys
* Access tokens
* Passwords
* Virtual environment files
* Temporary cache files

---

## 🚀 Future Improvements

Possible future improvements include:

* 📚 Generate flashcards from uploaded PDF files
* 🎯 Difficulty levels such as Easy, Medium, and Hard
* 🔢 User-selected number of flashcards
* 🔄 Regenerate flashcards
* 💾 Save generated flashcards
* 📊 Track learning progress
* 🌙 Dark mode
* 📱 Improved mobile responsiveness

---

## 🎯 Purpose of the Project

The main purpose of this project is to demonstrate how **Generative AI can be integrated into a web application** to create useful educational content automatically.

It combines a simple web frontend, a Python Flask backend, and the Hugging Face API to create an AI-powered learning tool.

---

## 👩‍💻 Project

**Hugging Face Flashcard Generator**

Built as a Generative AI learning project using:

**HTML + CSS + JavaScript + Python Flask + Hugging Face API**

---

## 📄 License

This project is created for educational and learning purposes.
