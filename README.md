# ⚔️ ClashControl

**ClashControl** is a lightweight coordination and scoring system built for coding competitions, debugging rounds, and symposium tech events.

It allows **multiple coordinators to manage participants, update scores, track completion times, and generate leaderboards in real time** from their phones.

ClashControl is designed for environments where **fast scoring, simplicity, and reliability** are more important than complex infrastructure.

---

## 🚀 Features

- 📱 **Mobile-Friendly Dashboard** – Coordinators can update scores easily from phones  
- ➕ **Quick Score Updates** – Add or subtract points instantly  
- 🏁 **Finish Tracking** – Record completion time when participants finish  
- 🏆 **Live Leaderboard** – Admin panel displays sorted rankings  
- 📊 **Batch Support** – Run multiple batches for large events  
- 📁 **CSV Export** – Export results after each batch  
- 📋 **Excel-Based Storage** – Simple `.xlsx` file used as database  
- ⚡ **Lightweight & Fast** – Minimal dependencies, easy to deploy locally  

---

## 🎯 Use Cases

ClashControl works great for:

- 💻 Coding competitions  
- 🐞 Debugging rounds  
- 🧠 Programming contests  
- 🏫 College symposium events  
- 🛠 Hackathons  

Multiple coordinators can **update scores simultaneously**, while the admin panel shows a **live leaderboard**.

---

## 🛠 Tech Stack

### Backend
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="Python"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" height="40" alt="Flask"/>
</p>

### Frontend
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="40" alt="HTML"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="40" alt="CSS"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="40" alt="JavaScript"/>
</p>

### Data Storage
<p>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" height="40" alt="Pandas"/>
</p>

- Excel (.xlsx)
- Pandas
- OpenPyXL

---

## 📁 Project Structure

```text
clashcontrol/
│
├── app.py                 # Main Flask server
├── config.py              # Configuration settings
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
│
├── data/
│   └── players.xlsx       # Excel "database"
│
├── templates/             # HTML templates
│   ├── base.html
│   ├── login.html
│   ├── dashboard.html
│   └── admin.html
│
├── static/
│   ├── css/
│   │   └── style.css
│   │
│   ├── js/
│   │   ├── dashboard.js
│   │   └── admin.js
│   │
│   └── icons/
│
├── utils/
│   ├── excel.py           # Excel read/write functions
│   └── export.py          # CSV export utilities
│
└── exports/               # Generated CSV exports
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/clashcontrol.git
cd clashcontrol
```

Create a virtual environment (recommended):

```bash
python -m venv venv
```

Activate the environment:

**Linux / macOS**
```bash
source venv/bin/activate
```

**Windows**
```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running ClashControl

Start the server:

```bash
python app.py
```

Open the application:

```
http://localhost:5000
```

To allow coordinators on the same network to connect:

```python
app.run(host="0.0.0.0", port=5000)
```

Then share your local IP address:

```
http://YOUR_LOCAL_IP:5000
```

---

## 📊 Excel Data Format

The `players.xlsx` file acts as the system database.

Recommended columns:

| name  | score | status   | finish_time | batch | created_at |
|-------|------|----------|-------------|------|------------|
| Rahul | 30   | solving  | -           | 1    | 10:05      |
| Ajay  | 45   | finished | 05:12       | 1    | 10:07      |

---

## 🏆 Admin Panel

The leaderboard can be accessed at:

```
/admin
```

The admin panel displays:

- 🥇 Player rankings  
- 📊 Scores  
- ⏱ Finish times  
- 📍 Current status (solving / finished)

---

## 📤 Export Results

Export the leaderboard as CSV:

```
/export
```

Exported files will be stored in the **exports/** directory.

---

## 🔮 Future Improvements

Potential upgrades for ClashControl:

- 🔄 Real-time updates using WebSockets  
- 🔐 Coordinator authentication  
- 🎯 Multiple events and rounds support  
- 📺 Projector-friendly leaderboard display  
- 📷 QR check-in for participants  
- 📡 Offline-first synchronization  

---

## 👨‍💻 Author

### Vibhakar S
Built to simplify coordination of competitive coding events.

**ClashControl — Command Your Competition ⚔️**