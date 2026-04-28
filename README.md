# 🚀 Daily Auto Commit with GitHub Actions

This repository uses **GitHub Actions** to automatically generate commits on a scheduled basis — no servers, no external tools.

---

## ✨ Features

* ⏰ Automatic commits based on a cron schedule
* 📝 Monthly log file generation (`logs/YYYY-MM.log`)
* 📌 Updates a `STATUS.md` file with latest run info
* 🔁 Fully automated using GitHub Actions

---

## ⚙️ How It Works

Every time the workflow runs:

1. A timestamp is added to a monthly log file
2. The `STATUS.md` file is updated
3. Changes are committed and pushed automatically

---

## 📂 Project Structure

```
.
├── .github/
│   └── workflows/
│       └── daily-commit.yml
├── logs/
│   └── YYYY-MM.log
├── STATUS.md
└── README.md
```

---

## ⏱️ Schedule

The workflow runs using a cron job:

```
0 0 * * *
```

🕒 This means it runs **daily at midnight (UTC)**.

---

## 🔐 Authentication

A **Personal Access Token (PAT)** is used to allow commits to be pushed as the repository owner instead of a bot.

---

## ▶️ Manual Run

You can trigger the workflow manually:

* Go to **Actions tab**
* Select **Daily Auto Commit**
* Click **Run workflow**

---

## 📊 Why This Project?

This project demonstrates:

* GitHub Actions automation
* CI/CD fundamentals
* Working with scheduled workflows

---

## 🧠 Future Improvements

* Add random commit messages
* Simulate real development activity
* Integrate with real projects
* Add notifications on failure

---

## 👩‍💻 Author

Created by **Hagar Mohammed**

---

