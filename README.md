# OpsMarine Frontend

A lightweight, fast frontend for the OpsMarine application. It ships with a clean HTML/JS structure, Tailwind CSS for styling, and a simple mock API (`db.json`) for quick prototyping and UI development. 

---
## ✨ Highlights

- **Tailwind CSS** for rapid, consistent styling.
  
- **Simple, component-friendly structure** under `src/`.

- **Mock API via** `db.json`—perfect for local development without a live backend. 

- **Plain HTML entry** (`index.html`)—works with any static server.

---

## 📁 Project Structure

Frontend-opsmarine_front/

├─ public/                 # Static assets

├─ src/                    # App source (components, routes, utilities)

│  └─ routes/              # Page/view modules and client-side routing glue

├─ db.json                 # Mock API data (use with json-server)

├─ index.html              # App entry

├─ tailwind.config.js      # Tailwind configuration

├─ postcss.config.js       # PostCSS configuration

├─ package.json            # Scripts & dependencies

└─ README.md

----

## 🧭 Routing

This project keeps page/views under `src/routes/`. A typical pattern is:

- Each **route module** handles rendering for a page/section.

- A tiny **client-side router** (hash-based or path-based) decides which module to mount.

- Shared UI (headers, sidebars) live in `src/` as reusable pieces.

---

## 🧩 Styling

Tailwind CSS is preconfigured (see `tailwind.config.js` and `postcss.config.js`).
Use utility classes directly in HTML/JS templates for rapid iteration.

---

## 🔌 Environment & Config

- **API base URL**: Point your fetch calls to the mock server (e.g., `http://localhost:7001`) during development.

- **Production**: Swap to your real backend URL or a proxy as needed.

  ----

## 🧪 Tips

- Keep UI chunks small and composable inside `src/`.

- Co-locate small styles or templates with the feature that uses them.

- For larger pages, split logic into helpers (e.g., `src/utils/`) to keep `routes/` clean.

  ----

## 🛠️ Scripts (examples)

Check `package.json` for the exact script names in your repo; if you prefer a dev server workflow, add:
```bash
{
  "scripts": {
    "dev": "serve .",
    "api": "json-server --watch db.json --port 7001",
    "build": "echo \"No build step needed for plain HTML/JS\""
  }
}
```
----

## 🤝 Contributing

Pull requests are welcome!

- Open an Issue for bugs/enhancements.

- Keep PRs focused and include a short description or screenshots for UI changes.

----
## 📬 Contact

- **Author**: Ali Razi

- **Email**: ali.razi9292@gmail.com

- **LinkedIn**: linkedin.com/in/alirazi1992

