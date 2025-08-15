# 📖 Lexora — English Dictionary

A fast, minimal **English dictionary** web app with a beautiful animated UI.  
Look up meanings, examples, synonyms, and pronunciation. Includes theme toggle and a **Word of the Day** feature.

🌐 **Live Demo:** [https://flyingvaibhav.github.io/lexora/](https://flyingvaibhav.github.io/lexora/)

---

## ✨ Features
- 🔍 **Search any English word** (press Enter to search)
- 📚 Shows:
  - Meaning and example
  - Synonyms *(click to search that synonym)*
  - Pronunciation with audio *(when available)*
- 🌟 **Word of the Day** on page load
- 🌓 Theme toggle (Light/Dark)
- 🎨 Subtle UI animations and animated background grid
- 📱 Responsive layout, keyboard friendly

---

## 🛠 Tech Stack
- **HTML, CSS, JavaScript** *(no frameworks)*
- **Icons:** Google Material Icons, Font Awesome
- **Font:** Google Fonts *(Poppins)*
- **API:** [Free Dictionary API](https://dictionaryapi.dev)

---

## 📂 Project Structure
lexora/
│── index.html # App markup (search bar, results, footer)
│── style.css # Styling, animations, grid background
│── script.js # App logic (fetch, render, audio, theme, Word of the Day)

yaml
Copy
Edit

---

## ⚙️ How It Works
1. When you type a word and press **Enter**, the app calls:
GET https://api.dictionaryapi.dev/api/v2/entries/en/<word>

yaml
Copy
Edit
2. The response is parsed to render:
- Part of speech + phonetics (text + audio)
- First definition + example
- Up to 5 synonyms *(clickable)*
3. The **speaker icon** plays audio if the API includes an audio URL.
4. The **theme toggle** switches between light and dark mode.
5. On load, a random **Word of the Day** is fetched from a small curated list.

---

## 🎨 Customization
- **Word of the Day list:** Edit `wordList` in `script.js`
- **Accent color & glow:** Tweak `--colors` or color values in `style.css`
- **Footer:** Update your name and LinkedIn URL in `index.html`

---

## 🛠 Troubleshooting
- 🔇 **No audio:** Some words don’t include audio; try another word.
- 📄 **Empty example/synonyms:** The API may not provide these for every word.
- 🌐 **API down/rate-limited:** The info text will show a friendly error; retry later.
- 🎭 **Icons not showing:** Ensure you’re online (icons/fonts load from a CDN).

---

## 🚀 Roadmap (Nice-to-haves)
- 💾 Save theme preference *(localStorage)*
- 📜 Search history *(localStorage + quick chips)*
- 📋 Copy to clipboard *(word + meaning)*
- ⏳ Loading spinner while fetching
- 📦 Offline cache for last results

---

## 🙏 Credits
- 📚 Dictionary API: [dictionaryapi.dev](https://dictionaryapi.dev)
- 🎨 Icons: [Google Material Icons](https://fonts.google.com/icons), [Font Awesome](https://fontawesome.com)
- ✍️ Font: [Google Fonts — Poppins](https://fonts.google.com/specimen/Poppins)

---

## 📜 License
Personal/educational use.  
Add a `LICENSE` file (e.g., MIT) if you want to open-source it.

---
> *"Words are, of course, the most powerful drug used by mankind." — Rudyard Kipling*
