# AS_352 Swine Production Flashcard Quiz

A lightweight, single‑page web app to study **247 verified multiple‑choice questions** from the AS_352 Swine Production course. Built with TailwindCSS and vanilla JS — simple enough to host directly on GitHub Pages.

## 📂 Files
- **index.html** → the web app (flashcard interface)
- **as352_verified_qna_FINAL.json** → dataset (all verified Q&A)

## 🚀 Usage
1. Create a repo (e.g., `as352-flashcards`) and put these two files in the repo root.
2. Commit & push.
3. Enable **GitHub Pages** in repo settings:
   - Source = your default branch (`main` or `master`)
   - Folder = `/root`
4. Visit your GitHub Pages URL → quiz auto‑loads.

### Run locally
Double‑click `index.html` or serve:
```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## 📑 Dataset Format
Each entry in `as352_verified_qna_FINAL.json` looks like:
```json
{
  "number": 1,
  "question": "…",
  "options": ["A", "B", "C", "D"],
  "answer": 0,
  "answer_text": "A",
  "support_1": "optional short snippet",
  "support_2": "optional short snippet"
}
```

## 🎮 Features
- Flashcard style → question on top, options below.
- Instant feedback → ✅ correct / ❌ wrong with correct highlighted.
- Auto‑next toggle, shuffle, and sound effects.
- Score + progress bar.
- End‑of‑session review with your answer vs correct answer.
- Export progress or reset anytime.

## 📜 License
Free to use and modify for study and educational purposes.
