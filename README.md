# 📚 StudyVault — Your 4-Year Learning Companion

A personal knowledge vault for university students. Write notes, build flashcards, quiz yourself — all saved automatically in your browser.

---

## 🚀 HOW TO PUT THIS ON GITHUB (Step by step — no experience needed)

### Step 1 — Create a GitHub account
1. Go to **https://github.com**
2. Click **"Sign up"**
3. Fill in your username, email, and password
4. Verify your email

---

### Step 2 — Create a new repository (this is like a folder on GitHub)
1. After logging in, click the **green "New"** button (top left), OR go to **https://github.com/new**
2. Fill in the form:
   - **Repository name:** `studyvault` (or anything you like)
   - **Description:** My personal study app (optional)
   - ✅ Check **"Public"** (so GitHub Pages works for free)
   - ✅ Check **"Add a README file"**
3. Click the green **"Create repository"** button at the bottom

---

### Step 3 — Install Git on your computer
> Git is a program that lets you "upload" files to GitHub.

**On Windows:**
1. Go to **https://git-scm.com/download/win**
2. Download and run the installer
3. Click "Next" on everything — the default settings are fine
4. When done, search for **"Git Bash"** in your Start menu and open it

**On Mac:**
1. Open **Terminal** (search for it in Spotlight)
2. Type `git --version` and press Enter
3. If it says "command not found", follow the prompt to install it

---

### Step 4 — Tell Git who you are (one time only)
Open **Git Bash** (Windows) or **Terminal** (Mac) and type these commands. Press Enter after each one.

Replace the name and email with YOUR GitHub name/email:

```bash
git config --global user.name "YourName"
git config --global user.email "youremail@example.com"
```

---

### Step 5 — Download your repository to your computer
Still in Git Bash/Terminal, type:

```bash
git clone https://github.com/YOUR_USERNAME/studyvault.git
```

Replace `YOUR_USERNAME` with your actual GitHub username. This creates a folder called `studyvault` on your computer.

---

### Step 6 — Copy the index.html file into that folder
1. Find the `studyvault` folder that was just created (it's wherever your terminal was pointing, usually your user folder or Desktop)
2. Copy the `index.html` file from wherever you saved it into the `studyvault` folder
3. **Also delete the README.md** that's already in the folder (or overwrite it with this one)

---

### Step 7 — Upload the file to GitHub
Back in Git Bash/Terminal, navigate into the folder:

```bash
cd studyvault
```

Then run these 3 commands in order:

```bash
git add .
git commit -m "Add StudyVault app"
git push
```

It may ask for your GitHub username and password. For the password, you actually need a **Personal Access Token** — follow Step 7b below.

---

### Step 7b — Create a Personal Access Token (GitHub's password replacement)
1. Go to **https://github.com/settings/tokens/new**
2. Give it a name like "studyvault"
3. Set expiration to "No expiration"
4. Check the box next to **"repo"**
5. Click **"Generate token"** at the bottom
6. **COPY the token** — it looks like `ghp_xxxxxxxxxxxx`
7. Use this token as your password when Git asks

---

### Step 8 — Turn on GitHub Pages (make your website live!)
1. Go to your repository on GitHub: `https://github.com/YOUR_USERNAME/studyvault`
2. Click **"Settings"** (top menu)
3. Click **"Pages"** (left sidebar)
4. Under **"Source"**, click the dropdown and select **"main"**
5. Click **Save**
6. Wait 1-2 minutes, then your site will be live at:
   ```
   https://YOUR_USERNAME.github.io/studyvault/
   ```

🎉 **That's it! Your StudyVault is online!**

---

## 📖 HOW TO USE STUDYVAULT

### Adding Content
```
+ Add Year  →  e.g. "Year 1 (2024–2025)"
    └── Add Semester  →  e.g. "Semester 1"
            └── Add Subject  →  e.g. "Introduction to Programming"
                    └── Add Chapter  →  e.g. "Chapter 1: Variables & Data Types"
```

Everything is in the **left sidebar**. Click the + buttons.

### Notes Tab 📝
- Click on a chapter to open it
- Type directly in the editor
- Use the toolbar to format: **bold**, *italic*, headings, lists, code blocks, tables
- **Auto-saves automatically** as you type
- Click **🔊 Listen** to have your notes read aloud (text-to-speech!)

### Flashcards Tab 🃏
- Click "+ Add Card" → type the question (front) and answer (back)
- Click **"Study Now"** to enter flip-card study mode
- Use ← → arrow keys or click the card to flip
- Click "🔀 Shuffle" to randomize order
- **Space bar** = flip card

### Quiz Tab ✏️
- Click "+ Add Question" → type question + options (Option A is always correct)
- Click **"Start Quiz"** for a randomized multiple-choice test
- Get instant feedback + explanations after each answer
- See your final score at the end

### Export / Import
- Click **⬇ Export** to download your data as a `.json` backup file
- Click **⬆ Import** to restore from a backup

### Keyboard Shortcuts
| Key | Action |
|-----|--------|
| `Ctrl+S` | Save manually |
| `Space` | Flip flashcard (in study mode) |
| `→` | Next flashcard |
| `←` | Previous flashcard |
| `Esc` | Close popup |

---

## 🔄 HOW TO UPDATE THE WEBSITE LATER

Whenever you change `index.html`, run these commands again:

```bash
cd studyvault
git add .
git commit -m "Update notes"
git push
```

Wait 1-2 minutes and your live website updates automatically!

---

## ⚠️ IMPORTANT NOTES

- **Your notes are saved in your browser** (localStorage). They won't disappear unless you clear browser data.
- **Always export a backup** before clearing browser data or switching computers.
- **To use on another computer**: Export your data, copy the `.json` file to the new computer, and use Import.
- The website is stored on GitHub — but your *notes data* lives in your browser. GitHub just hosts the app itself.

---

*Built with ❤️ for first-year university students. Good luck with your studies!*
