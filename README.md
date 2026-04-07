# 📖 English Janala

> **Learn English Vocabulary — Level by Level** — An interactive vocabulary learning app powered by a live API with pronunciation, search, and save features!

🚀 [Visit the Live App](https://ahsanul-islam-083.github.io/english-janala-app/)

---

## 📖 Overview

**English Janala** is a browser-based vocabulary learning app that fetches English words level by level from a live API. Users can browse lessons, view word meanings and pronunciations, hear words spoken aloud, save favourites, and search across the entire vocabulary — all in one clean, interactive UI.

---

## 🖼️ Screenshot

> <img width="1900" height="980" alt="image" src="https://github.com/user-attachments/assets/081444e0-b5db-4f28-a90e-196f90e67b23" />
> <img width="1900" height="974" alt="image" src="https://github.com/user-attachments/assets/1750cb22-60c5-472e-bb81-a629d0474442" />


---

## 🚀 Features

- 📚 **Level-based lessons** — dynamically generated lesson buttons from the API
- 🃏 **Word cards** — displays word, meaning, pronunciation, and action buttons
- 🔊 **Voice pronunciation** — hear any word spoken aloud with one click
- 🔍 **Search functionality** — search across all words in real time
- ❤️ **Save words** — bookmark favourite words to a personal saved section
- 🔄 **Loading spinner** — smooth feedback while vocabulary data is fetching
- ⚠️ **Error handling** — gracefully handles missing or invalid API data
- 🎯 **Active button highlight** — clearly shows which lesson is currently selected

---

## ⚡ API Endpoints

| Endpoint | Description |
|---|---|
| `GET /api/levels/all` | Fetch all lesson levels |
| `GET /api/level/{id}` | Fetch all words for a specific level |
| `GET /api/word/{id}` | Fetch details for a specific word |
| `GET /api/words/all` | Fetch all words |

**Base URL:** `https://openapi.programming-hero.com`

```bash
# Example requests
GET https://openapi.programming-hero.com/api/levels/all
GET https://openapi.programming-hero.com/api/level/5
GET https://openapi.programming-hero.com/api/word/5
GET https://openapi.programming-hero.com/api/words/all
```

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling and layout |
| Vanilla JavaScript | App logic and API calls |
| Fetch API | Async data fetching |
| Web Speech API | Voice pronunciation |

---

## 🏃 Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/ahsanul-islam-083/english-janala-app.git
   cd english-janala-app
   ```

2. **Open in your browser**
   ```bash
   # Simply open index.html in any browser
   open index.html
   ```
   > No server or build step needed — it's pure HTML, CSS, and JS!

---

## 🎮 How to Use

| Action | Result |
|---|---|
| Click a lesson button | Loads all words for that level |
| Click the 🔊 icon | Pronounces the word aloud |
| Click the details icon | Opens a modal with full word info |
| Click ❤️ on a card | Saves the word to your saved section |
| Type in the search box | Filters words across all vocabulary |

---

## 🔊 Voice Pronunciation

The app uses the browser's built-in Web Speech API for audio pronunciation:

```js
function pronounceWord(word) {
  const utterance = new SpeechSynthesisUtterance(word);
  utterance.lang = "en-EN"; // English
  window.speechSynthesis.speak(utterance);
}
```

---

## 📁 Project Structure

```
english-janala-app/
├── index.html        # Main HTML file
├── styles/
│   └── style.css     # App styles
├── script/
│   └── app.js        # Core app logic
└── assets/
    └── logo.png      # App logo
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for bug fixes, new features, or design improvements.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> 💡 *Learn a little every day — vocabulary is the key to fluency!*
