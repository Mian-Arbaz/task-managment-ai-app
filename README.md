<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/00abd0c8-4e98-4681-bd96-5323ae3c1bc2" /> task-managment-ai-app
Full-stack task managment app with AI-powered task suggestion. 

---

markdown
# Task Management AI App

A **full-stack web application** for managing tasks with **AI-powered suggestions**.  
Built to showcase skills in **Node.js, React, MongoDB, and Generative AI (Python with Hugging Face)**.

---

## 🚀 Features

- 🔐 **User Authentication** with JWT  
- 📝 **Task Management** – Create, Read, Update, Delete  
- 🤖 **AI Task Suggester** – Enter a goal (e.g., “Build a website”) → Get actionable subtasks  
- 📱 **Responsive UI** built with Tailwind CSS  
- ⚡ Clean UX with loading & error states

---

## 🛠️ Tech Stack

| Layer      | Technology                        |
|------------|----------------------------------|
| Frontend   | React, HTML/CSS/JS, Tailwind CSS |
| Backend    | Node.js, Express, MongoDB (Mongoose) |
| AI Service | Python, Transformers (mock LLaMA-like suggestions) |
| Deployment | Vercel (Frontend), Render (Backend), MongoDB Atlas |

---

## 📦 Project Structure

```

/frontend   → React app + Tailwind
/backend    → Node.js + Express API
/ai         → Python AI suggester

````

---

## 🧰 Setup Instructions

### 1️⃣ Prerequisites
- [Node.js](https://nodejs.org/) v18+
- [Python](https://www.python.org/) 3.10+
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) account (free)
- Git

---

### 2️⃣ Backend Setup
```bash
cd backend
npm init -y
npm install express mongoose jsonwebtoken bcryptjs cors dotenv
````

Create a `.env` file:

```env
MONGO_URI=your_mongo_atlas_uri
JWT_SECRET=your_secret
```

Run the server:

```bash
node server.js
```

#### REST Endpoints

* `POST /api/auth/register`
* `POST /api/auth/login`
* `GET /api/tasks`
* `POST /api/tasks`
* `PUT /api/tasks/:id`
* `DELETE /api/tasks/:id`
* `POST /api/ai/suggest`

---

### 3️⃣ Frontend Setup

```bash
cd frontend
npx create-react-app .
npm install
```

* Integrate Tailwind CSS
* Update `API_BASE` in your config to point to the backend
* Start the app:

```bash
npm start
```

---

### 4️⃣ AI Setup

```bash
cd ai
pip install transformers torch
```

* Create `ai_suggest.py` that accepts a goal and returns a list of subtasks.
* Backend calls this script to get AI suggestions.

---

### 5️⃣ Deployment

* **Frontend:** Push to GitHub → Deploy on [Vercel](https://vercel.com)
* **Backend:** Deploy Node.js API on [Render](https://render.com)
* **Database:** Use [MongoDB Atlas](https://www.mongodb.com/atlas)

---

## 🧪 Usage

1. Register or log in.
2. Create tasks manually or enter a goal to generate subtasks via AI.
3. Mark tasks as done, edit, or delete them.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to improve.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

### ✨ Author

> **Your Name** – [yourwebsite.com](https://yourwebsite.com)

```

