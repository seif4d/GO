# GO 🚀 | Custom URL Shortener

Welcome to **GO**! 👋
This is a lightweight, maintenance-free URL shortener hosted 100% on **GitHub Pages**.

It allows me to turn long, ugly URLs into clean, short links using my own domain. 😎

---

## 🌟 How It Works

This project uses a clever "Static 404 Hack":
1. When a user visits a link that doesn't exist (e.g., `/GO/1`).
2. GitHub Pages triggers the `404.html` page.
3. The JavaScript inside `404.html` grabs the path (`1`).
4. It fetches `links.json` to find the matching URL.
5. It redirects the user instantly! ⚡️

---

## 🛠️ How to Add a New Link

Adding a new short link is super easy. Just edit the [`links.json`](./links.json) file:

1. Open `links.json`.
2. Add a new key-value pair: `"ShortCode": "TargetURL"`.
3. Commit the changes.

**Example:**
```json
{
  "1": "https://chatgpt.com",
  "fb": "https://facebook.com/seif4d",
  "portfolio": "https://seif4d.github.io"
}
```

Now the links will work like this:
- `seif4d.github.io/GO/1` ➡️ Redirects to ChatGPT
- `seif4d.github.io/GO/fb` ➡️ Redirects to Facebook

---

## 📂 File Structure

- **`links.json`**: 🗂 The database (where you store your links).
- **`404.html`**: ⚙️ The engine (handles the redirection logic).
- **`index.html`**: 🏠 The landing page (if someone visits the root URL).

---

## 🚀 Usage

Feel free to fork this repository to create your own URL shortener!

1. Fork the repo.
2. Enable **GitHub Pages** in Settings.
3. Update `links.json` with your own links.
4. Update the `repoName` variable in `404.html` if you change the repo name.

**Developed by Seif4d 👨‍💻**
