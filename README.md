# DOTfit Desk — MCP Integration


## 🚀 What is this?

**DOTfit Desk — MCP** is a desktop helper toolkit that bridges a local GUI tool with an MCP (Model Context Protocol) server demo.

The goal of this project is to showcase how a *user desktop interface* can interact with an MCP backend to fetch results and display them locally. The MCP demo included is based on a lightweight Python server.

This repository is **not just a notebook** — it's an app + a server designed to demonstrate a full cycle:  
🖥️ Desktop app → ⚙️ MCP server → 📦 result output

---

## 📌 Why this matters

Most AI demos are limited to *scripts or Jupyter notebooks*. This repo is structured as a **mini production flow**:

- UI/Frontend (HTML/CSS/JS)
- Backend server (MCP demo)
- IPC / communication pattern
- Real runnable application

This is a good base for:
✅ AI assistant UIs  
✅ Project templates for desktop-to-server communication  
✅ Prototyping logic with Python + MCP

---

## 🧠 Features

- 💻 **Desktop UI** (HTML/CSS frontend)
- 📡 **MCP demo server** written in Python
- 🔗 Communication bridge between UI and backend
- 🧪 Demo workflow included

---

## 🔧 Requirements

Install Python 3.8+:

```bash
python --version
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🏃 How to Run

### 1️⃣ Start the MCP demo server

```bash
cd mcp-server-demo
python main.py
```

This spins up the backend that the desktop app talks to.

---

### 2️⃣ Open the Desktop UI

Open `index.html` in your browser or local desktop app shell.

```bash
open index.html
```

---

### 🔍 How It Works

```
[Desktop UI]  <– fetch requests –>  [MCP Server]
```

The UI sends structured requests to the local MCP server. The server responds with processed output.

This pattern can be extended to:
✔ External APIs  
✔ AI models  
✔ Local OS interactions  

---

## 📁 Repo Structure

```
/
├── mcp-server-demo     🚀 Python MCP backend
├── Final_DOTfitDesk_exe 🧰 Executable build of the desktop UI
├── README.md           📘 You're here
├── assets/             🖼 UI resources
└── index.html          🧩 Desktop entry
```

---

## 📌 Improvements You Could Add

If you want to level this up:

✔ Add a real AI backend (FastAPI + GPT-based logic)  
✔ Package the UI into an Electron/desktop app  
✔ Dockerize the MCP server  
✔ Add tests and CI/CD  
✔ Provide real use cases (OCR, Chat UI, tool integration)

---

## 📞 Contributing

If you build something cool on top of this:
- Create an issue
- Submit a friendly pull request
- Add your demo link in the README
