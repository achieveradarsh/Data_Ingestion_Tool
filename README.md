
# AdventureConnect: ClickHouse ↔ Flat File Integration Tool

A web-based data ingestion tool that enables **bidirectional data flow** between a ClickHouse database and flat files (CSV). This application is ideal for seamless data export/import operations, complete with schema discovery, column selection, and record count reporting.

---

## Features

- [x] **Bidirectional Flow**
  - ClickHouse → Flat File
  - Flat File → ClickHouse
- [x] **User Interface**
  - Clean UI to select source, target, connection configs, columns, and ingest
- [x] **JWT-based Authentication** for ClickHouse source
- [x] **Schema Discovery & Column Selection**
- [x] **Efficient Data Handling** using batching
- [x] **Error Handling and Record Count Reporting**

---

## Tech Stack

- **Backend**: Python (Flask)
- **Frontend**: HTML, CSS, JavaScript (vanilla)
- **DB Support**: ClickHouse with JWT Token
- **Cloud Testing**: Compatible with ClickHouse Cloud or Docker

---

## Recommended Environment

> **Replit (Highly Recommended)**  
> Project runs smoothly on Replit's web IDE. Just clone the repo and run `main.py`.

---

## Setup Instructions

### 1. Clone the Repo
```bash
git clone https://github.com/yourusername/adventureconnect.git
cd adventureconnect
```

### 2. (Optional) Create Virtual Environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Application
```bash
python main.py
```

---

## Replit Instructions

1. Go to [Replit.com](https://replit.com)
2. Import from GitHub → paste the repo link
3. Click **Run** (will auto-detect `main.py` as entrypoint)

---

## Directory Structure

```
AdventureConnect/
│
├── app.py                   # Core Flask app logic
├── main.py                  # Entry point to run server
├── pyproject.toml           # Poetry project config
├── requirements.txt         # For local/Replit installs
├── templates/
│   └── index.html           # UI template
├── static/
│   ├── css/custom.css       # Styling
│   └── js/main.js           # Frontend logic
├── utils/
│   ├── clickhouse_client.py # ClickHouse client logic
│   ├── flat_file_client.py  # Flat file read/write
│   └── data_integrator.py   # Data transfer logic
├── uploads/                 # Sample or user-uploaded files
```

---

## Test Scenarios

1. **ClickHouse → Flat File** (selected columns)
2. **Flat File → ClickHouse** (selected columns into new table)
3. **JWT Token Connection Handling**
4. **Error Handling on Wrong Host/Token**
5. *(Bonus)* Multi-table join (UI not implemented, but supported in logic)

---

## AI Tools Used

This project used AI-based coding assistance (ChatGPT) for:

- Schema parsing logic
- JWT token integration
- UI design decisions
- Prompt file attached: `prompts.txt`

---

## License

MIT License  
© 2025 Adarsh Bangaram
