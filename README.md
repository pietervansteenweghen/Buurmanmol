# Mystery Button 🔴

A single-page site with a pulsing red button that plays a random audio clip.

## Project Structure

```
mystery-button/
├── index.html        ← the whole site
├── image.png         ← your background image (add this!)
└── audio/
    ├── 01.mp3
    ├── 02.mp3
    ├── 03.mp3
    ...
    └── 15.mp3
```

## Setup

### 1. Add your background image
Drop your image into the project root and name it **`image.png`**
(or edit the `url('image.png')` line in index.html to match your filename)

### 2. Add your audio files
Drop your 15 MP3s into the `audio/` folder, named:
`01.mp3`, `02.mp3`, `03.mp3` ... `15.mp3`

> If you prefer different filenames, edit the `tracks` array in index.html.

---

## Deploy to Vercel (free, ~60 seconds)

### Option A — Drag & Drop (no GitHub needed)
1. Go to [vercel.com](https://vercel.com) and sign in
2. Click **"Add New → Project"**
3. Choose **"Deploy from your local folder"** (drag-and-drop zone)
4. Drag the entire `mystery-button/` folder onto the page
5. Click **Deploy** — done ✓

### Option B — Via GitHub
1. Create a new GitHub repo and push this folder
2. Go to [vercel.com](https://vercel.com), click **"Add New → Project"**
3. Import your GitHub repo
4. No build settings needed (it's a static site) — click **Deploy** ✓

---

## Customization

| What | Where in index.html |
|------|---------------------|
| Background image filename | `url('image.png')` in `#bg` CSS |
| Button size | `width` / `height` on `#btn` |
| Number of tracks | `const TOTAL = 15` |
| Track filenames | `const tracks = [...]` array |
| Show track names instead of numbers | Replace `Track ${idx+1} of ${TOTAL}` with your own label |
