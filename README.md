# 🍽️ Spice Garden — Restaurant Telegram Bot

A smart restaurant bot built using Make.com, Groq AI (LLaMA), and Google Sheets.
No code. Full automation.

---

## 🤖 What it Does

- User apna naam batata hai → Bot welcome karta hai aur menu dikhata hai
- User order karta hai → Bot confirm karta hai aur Google Sheet mein save karta hai
- User "menu" maangta hai → Bot menu dikhata hai
- Random message → Bot guide karta hai

---

## ⚙️ Tech Stack

| Tool          | Use                        |
|---------------|----------------------------|
| Telegram Bot  | User interface             |
| Make.com      | Automation platform        |
| Groq API      | AI (LLaMA 3.3 70B model)   |
| Google Sheets | Order storage              |

---

## 🔁 Flow

```
User Message
     ↓
Telegram Bot
     ↓
Make.com Scenario
     ↓
Groq AI (3 Rules)
     ↓
Router
├── Order → Google Sheets + Confirm
└── Other → Reply Only
```

---

## 📋 3 Rules (Prompt Engineering)

```
RULE 1: Naam bataye → Welcome + Menu
RULE 2: Order kare  → Confirm + Sheet Save
RULE 3: Kuch aur    → Guide karo
```

---

## 📊 Google Sheet Structure

| Timestamp | User | Order |
|-----------|------|-------|
| 06/06/2026 14:32 | Nakul | Butter Chicken x1, Naan x2 |

---

## 📸 Screenshots

### Telegram Bot Chat
![Telegram Chat](screenshots/Screenshot 2026-06-06 212156.png)

### Make.com Scenario
![Scenario](screenshots/Screenshot 2026-06-06 212557.png)

### Google Sheet
![Sheet](screenshots/Screenshot 2026-06-06 211852.png)
---

## 🚀 How it Works

1. User sends message on Telegram
2. Make.com webhook triggers
3. Groq AI processes message
4. Router decides — order or not
5. If order → Save to Google Sheets
6. Reply sent back to user

---

## 👨‍💻 Built By

Nakul Adhave
[LinkedIn](https://linkedin.com/in/nakul-adhave-a82294330) |
[GitHub](https://github.com/nakuladhave)
