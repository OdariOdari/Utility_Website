# 📘 Utilities Suite — Multi‑Tool Web App

A **multi‑page website** built with **HTML, CSS, Vanilla JavaScript** (no frameworks), providing a set of productive tools:

- 💸 **Expense Tracker** (with chart visualization)
- ✅ **To‑Do List**
- ⏱️ **Pomodoro Timer**
- 📏 **Unit Converter**
- 🔐 **Password Generator + Strength Checker**
- 📝 **Markdown Previewer**
- 💱 **Currency Converter**
- 🥇 **Gold Price Calculator**

All tools run **locally in your browser** — no backend required. Data persists using **localStorage** where applicable.

---

## 🚀 Features

### 1. **Expense Tracker**
- Input **amount, description, category**
- Displays entries in a table  
- Deletes entries individually  
- Shows **total expense**  
- Visualizes spending by category using **Chart.js doughnut chart**  
- Saves all data in `localStorage`

### 2. **To‑Do List**
- Add, edit, delete tasks  
- Mark as completed (with strike‑through)  
- Filters: **All / Active / Completed**  
- Displays task stats  
- Data persisted in `localStorage`

### 3. **Pomodoro Timer**
- Default **25/5 min work/break** cycles  
- Customizable durations + cycles  
- Start, pause, reset functionality  
- SVG circular progress animation  
- Beep sound when intervals end  

### 4. **Unit Converter**
- Converts **Length, Weight, Temperature**  
- Supports metric + imperial units  
- Instant conversion while typing  

### 5. **Password Generator**
- Options: uppercase, lowercase, numbers, symbols, length slider  
- One‑click generate + copy to clipboard  
- Built‑in password strength checker  

### 6. **Markdown Previewer**
- Split‑screen live preview  
- Supports:  
  - Headings (`# H1 … ###### H6`)  
  - Bold (`**bold**`), Italic (`*italic*`)  
  - Inline code & blocks (`` `code` `` and ``` ``` )  
  - Lists (ordered & unordered)  
  - Links `[text](url)`  
  - Images `![alt](url)`  
  - Blockquotes (`>`)  
  - Horizontal rules (`---`)  

### 7. **Currency Converter**
- Uses **Frankfurter API** for live exchange rates  
- Converts between supported world currencies  
- Shows last updated timestamp  
- Gracefully handles network errors  

### 8. **Gold Price Calculator**
- Enter **weight in grams or ounces**  
- Select any **currency** (loaded via Frankfurter API)  
- Uses fallback of **$2000/oz in USD** (demo)  
- Auto converts USD value into selected currency  
- Displays last updated timestamp  
- ✨ Can integrate with **Metals API** or **GoldAPI** for live gold prices (swap out the fake value in `gold.js`)  

---

## 📂 Project Structure
```
/project-root
│
├── index.html                  ← Homepage
├── expense-tracker.html
├── todo.html
├── pomodoro.html
├── unit-converter.html
├── password-generator.html
├── markdown.html
├── currency-converter.html
├── gold-price.html
│
├── /css
│   └── styles.css              ← Global styles (dark/light theme)
│
├── /js
│   ├── main.js                 ← Homepage animations + theme
│   ├── expense.js              ← Expense Tracker logic
│   ├── todo.js                 ← To‑Do List logic
│   ├── pomodoro.js             ← Pomodoro Timer logic
│   ├── converter.js            ← Unit Converter logic
│   ├── password.js             ← Password Generator logic
│   ├── markdown.js             ← Markdown Preview logic
│   ├── currency.js             ← Currency Converter logic
│   └── gold.js                 ← Gold Price Calculator logic
│
└── /assets                     ← (optional: images, icons)
```

---

## 🎨 Theming
- Supports **Dark/Light mode toggle** 🌗  
- Theme choice saves in `localStorage`  
- Consistent design across all tools  

---

## ⚙️ How to Run

### Option 1: Open directly
- Simply **double‑click `index.html`** to open in your browser.
- Works offline for most tools.
- Some features (Currency Converter & Gold Price Calculator) require **internet**.

### Option 2: Run via Local Web Server (Recommended)
Some browsers restrict API calls from local files. Use:

#### Python
```bash
cd project-root
python -m http.server 8000
```
Visit 👉 `http://localhost:8000`

#### Node.js
```bash
npm install -g serve
serve .
```

#### VS Code
- Install **Live Server** extension
- Right click → **Open with Live Server**

---

## 🔗 APIs Used
- [**Frankfurter API**](https://www.frankfurter.app/) → live currency exchange rates  
- (Optional) [**Metals API**](https://metals-api.com) or [GoldAPI](https://www.goldapi.io) → live gold price integration  

---

## 🛡️ Tech Stack
- Pure **HTML5**
- **CSS3** (flexbox/grid, custom theme, animations, responsive design)
- **Vanilla JavaScript**
- [**Chart.js**](https://www.chartjs.org/) → Expense Tracker visualization  

---

⚡ Fast, lightweight, private — everything runs in your browser.  

