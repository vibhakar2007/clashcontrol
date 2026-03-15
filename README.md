<p align="center">
  <h1 align="center">⚔️ ClashControl</h1>
  <p align="center">
    Lightweight contest coordination system for coding competitions and symposium events.
  </p>
</p>

<p align="center">

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Python](https://img.shields.io/badge/backend-Django-green)
![NextJS](https://img.shields.io/badge/frontend-Next.js-black)
![Database](https://img.shields.io/badge/database-SQLite-blue)
![Status](https://img.shields.io/badge/status-active-success)

</p>

---

# ⚔️ ClashControl

**ClashControl** is a lightweight contest coordination system designed for **coding competitions, debugging rounds, and college symposium events**.

It allows **multiple coordinators to manage participants, update scores, record completion times, and track leaderboards in real time** using their mobile devices.

The system is built to run **locally on a single machine**, allowing events to be conducted even **without internet access**.

---

# 🚀 Key Features

📱 **Mobile-friendly coordinator dashboard**  
➕ **Quick score updates** for participants  
⏱ **Finish time tracking** for tie-breaking  
🏆 **Live leaderboard for administrators**  
📦 **Batch support** for large events  
📊 **CSV export** for results and records  
🖥 **Local network hosting** for offline competitions

---

# 🛠 Tech Stack

## Frontend

<p>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nextjs/nextjs-original.svg" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tailwindcss/tailwindcss-original.svg" height="40"/>
</p>

## Backend

<p>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" height="40"/>
</p>

## Database

<p>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sqlite/sqlite-original.svg" height="40"/>
</p>


---

# 📁 Project Structure

```
clashcontrol/
│
├── README.md
├── LICENSE
│
├── backend/
│   ├── manage.py
|   ├── requirements.txt
│   ├── db.sqlite3
│   │
│   ├── clashcontrol/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   ├── asgi.py
│   │   └── wsgi.py
│   │
│   ├── apps/
│   │   ├── users/
│   │   ├── participants/
│   │   ├── scoring/
│   │   └── events/
│   │
│   └── api/
│       ├── views.py
│       └── serializers.py
│
├── frontend/
│   ├── package.json
│   ├── next.config.js
│   ├── tailwind.config.js
│   │
│   ├── public/
│   │
│   └── src/
│       ├── app/
│       │   ├── page.tsx
│       │   ├── coordinator/
│       │   └── admin/
│       │
│       ├── components/
│       ├── lib/
│       └── styles/
│
└── exports/
```

---

# ⚙️ Installation

Clone the repository

```bash
git clone https://github.com/vibhakar2007/clashcontrol.git
cd clashcontrol
```

---

# ▶️ Running the Backend

Navigate to backend directory

```bash
cd backend
```

Create virtual environment

```bash
python -m venv venv
```

Activate environment

Windows

```
venv\Scripts\activate
```

Linux / macOS

```
source venv/bin/activate
```

Install dependencies

```
pip install -r requirements.txt
```

Run migrations

```
python manage.py migrate
```

Start server

```
python manage.py runserver
```

Backend runs at:

```
http://localhost:8000
```

---

# ▶️ Running the Frontend

Open another terminal

```bash
cd frontend
```

Install dependencies

```
npm install
```

Start development server

```
npm run dev
```

Frontend runs at:

```
http://localhost:3000
```

---

# 📱 Using ClashControl During Events

1️⃣ Start backend server  
2️⃣ Start frontend server  
3️⃣ Connect all coordinator devices to the same network  
4️⃣ Coordinators open the dashboard from their phones  
5️⃣ Admin monitors leaderboard in real time

---

# 📊 Planned Features

- Real-time leaderboard updates  
- QR code participant check-in  
- Multi-event management  
- Role-based authentication  
- Event analytics  
- Standalone desktop installer

---

# 📜 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for details.

---

# 👨‍💻 Author

Developed by **Vibhakar S**

ClashControl was created to simplify coordination of **coding competitions and symposium technical events**.

---

<p align="center">
  ⚔️ Command Your Competition with ClashControl
</p>