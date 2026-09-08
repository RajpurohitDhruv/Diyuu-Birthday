# 🎀 Pikuuu's Birthday Surprise Site

Already filled in with your real content and her 10 photos. The flow is:

1. Passcode lock (`Pikuuu`) + hint
2. Hero welcome message
3. Your personalised messages, one at a time
4. The big final wish line
5. A short transition line
6. 6 tap-to-open wishes
7. 10 photo memories with your captions
8. Song player
9. Final closing words + your signature

Everything is in **one file**: `index.html`. No coding needed to edit it —
but you're welcome to tweak anything.

---

## 1. Edit your content

Open `index.html` in any text editor (Notepad, VS Code, even Google Docs'
"plain text" mode works in a pinch). Scroll down to the line that says:

```
STEP 1: EDIT YOUR CONFIG
```

You'll see a block called `CONFIG = { ... }`. Change the text between the
quotes `" "` for each part:

- `passcode` — the word/number she has to type to unlock it
- `passcodeHint` — a clue for her
- `welcomeTitle` / `welcomeSubtitle` — what she sees right after unlocking
- `messages` — add/remove/edit lines, each one shows one at a time
- `photos` — filename + caption for each photo (see step 2)
- `song` — filename, title, artist
- `wishes` — exactly 6 short lines, each behind a flip card
- `finalTitle` / `finalText` / `finalSignature` — the very last screen

To add or remove a message/photo/wish, copy an existing line inside the
`{ }` brackets and edit it, or delete a whole line. Just make sure commas
between entries stay in place.

**Wishes must stay at exactly 6** to match the 2×3 grid layout — the wish
text currently in the config was pulled from your screen recording. If your
screenshot has different exact wording, just edit the 6 `text` lines inside
`wishes: [ ... ]`.

## 2. Photos

Your 10 photos are already in the `photos` folder, numbered `1.jpg`
through `10.jpg` in the order you gave, with your captions already typed
into the config. If you want to swap a photo, just replace that numbered
file with a new one (keep the same filename), or add more entries to the
`photos` list in the config.

If a photo file ever goes missing, the site shows a friendly placeholder
instead of breaking.

## 3. Add your song

Put one MP3 file next to `index.html` and name it `song.mp3` (or change
`song.src` in the config to match whatever you named it). Keep the file
reasonably small (under ~8MB) so it loads quickly on her phone.

## 4. Preview it

Just double-click `index.html` to open it in your browser and click
through everything. (The song may not autoplay from a double-clicked file
in some browsers due to security rules — that's normal, it'll work fine
once hosted online.)

## 5. Host it & get a link

Easiest free options, no account needed to start:

**Netlify Drop (fastest)**
1. Go to https://app.netlify.com/drop
2. Drag your whole folder (`index.html`, `photos/`, `song.mp3`) onto the page
3. It gives you a live link instantly — copy and send it to her 💛

**GitHub Pages**
1. Create a new GitHub repo, upload these files
2. Go to Settings → Pages → set source to your main branch
3. Your link will be `https://yourusername.github.io/repo-name/`

Either way — once it's live, open the link yourself first on your phone to
double check the passcode, photos, and song all work, then send it to her.

---

Made for a birthday surprise. Enjoy 🎂
