# 🚗 Smart Vehicle Management System with ANPR

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![YOLOv8](https://img.shields.io/badge/YOLOv8-FFCC00?style=for-the-badge&logo=ultralytics&logoColor=black)

A high-performance **Automatic Number Plate Recognition (ANPR)** system built to automate vehicle parking management, entry/exit logging, and data-driven analytics.

---

## ✨ Key Features

- 📸 **AI-Powered ANPR**: Automatic number plate extraction from uploaded images using YOLOv8 and EasyOCR.
- 📋 **Live Management Dashboard**: Real-time vehicle logging, search, and exit management.
- 📊 **Smart Analytics**: Interactive data visualization of parking trends, occupancy, and peak hours.
- 💰 **Automated Billing**: Dynamic parking charge calculation (₹30/hr) based on stay duration.
- 🔐 **Admin Security**: Secure authentication for system administrators.
- 📂 **Export Capability**: Export logs to CSV for record-keeping and auditing.

---

## 🛠️ Tech Stack

- **Backend**: Python, Flask, Flask-CORS
- **Frontend**: Jinja2 (Management UI), React + Vite (Analytics Dashboard)
- **Machine Learning**: YOLOv8 (Detection), EasyOCR (Recognition)
- **Database**: SQLite3
- **Visualization**: Recharts, Tailored CSS for Glassmorphism UI

---

## 🚀 Getting Started

### 1. Prerequisites
- Python 3.10+
- Node.js & npm

### 2. Setup Backend
```bash
# Navigate to project root
pip install -r requirements.txt

# Run the server
python backend/app.py
```

### 3. Setup Analytics Dashboard
```bash
# Navigate to analytics directory
cd analytics
npm install
npm run dev
```

---

## 🔄 Project Flow & Architecture

The system uses a **Hybrid Architecture**:
1. **Core CRUD**: Flask handles the direct management interface via Jinja2 templates.
2. **AI Processing**: Images are processed via an ML pipeline (YOLO -> OCR -> Regex).
3. **API Layer**: Flask serves a JSON API for the React-based analytics dashboard.

For a deep dive into the technical details, see [PROJECT_OVERVIEW.md](./PROJECT_OVERVIEW.md).

---

## 📂 Project Structure

```text
├── analytics/           # React + Vite Analytics Dashboard
├── backend/             # Flask API & ML Logic
│   ├── anpr.py          # AI Engine implementation
│   ├── app.py           # Core routes & DB logic
│   └── database.py      # SQLite Schema
├── frontend/            # HTML/Jinja2 Templates for Management UI
├── uploads/             # Temporary storage for ANPR images
└── PROJECT_OVERVIEW.md  # Detailed system architecture
```

---

## 📄 Commit History
This project followed a professional, logical commit workflow. You can view the full development log in [COMMIT_LOG.md](./COMMIT_LOG.md).

---

## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request.

---

## 📝 License
This project is open-source and available under the MIT License.
