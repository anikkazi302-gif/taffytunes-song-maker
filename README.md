# TaffyTunes Song Maker 🎵🐥

Make an **original English nursery-rhyme song** for a 1-minute kids' Short (9:16 vertical) — with Taffy.

Pick a topic, and the tool gives you everything you need to make the video:

- 🎤 **The HOOK** — the song's first sung line, shown big
- 📜 **Full lyrics** — 4 short verses + a repeating chorus, with one copyable action per verse
- 🏷️ **SEO title** — in the proven TaffyTunes shape
- 📝 **Description** — short, ready to paste into YouTube Studio
- #️⃣ **Hashtag block** — the fixed TaffyTunes block plus the topic tag
- 🎵 **Music-fit hint** — which mood of copyright-free track fits the topic

Everything runs **in your browser**. No account, no server, no build step, no paid API. It works offline.

## The 12 topics

| # | Topic | Mood | Hook (first sung line) |
|---|-------|------|------------------------|
| 1 | Bath Time 🛁 | Cheerful | Splish, splash, bubbles in the air! |
| 2 | Brushing Teeth 🪥 | Playful | Brush, brush, brush your teeth! |
| 3 | Bedtime 🌙 | Calm | Twinkle, twinkle, time for bed! |
| 4 | Animals 🐾 | Playful | Roar like a lion, stomp, stomp, stomp! |
| 5 | Numbers 🔢 | Cheerful | One, two, three, let's count with me! |
| 6 | Colors 🎨 | Cheerful | Red, blue, yellow, green — colors all around! |
| 7 | Family 👨‍👩‍👧 | Cheerful | Mommy, Daddy, love you so! |
| 8 | Food 🍎 | Playful | Yum, yum, yum, what's for lunch? |
| 9 | Rain ☔ | Calm | Pitter-patter, rain is falling down! |
| 10 | Playground 🛝 | Dance | Swing, slide, climb — let's play today! |
| 11 | ABC 🔤 | Cheerful | A, B, C, let's sing with me! |
| 12 | Good Manners 🌟 | Cheerful | Please and thank you, magic words! |

## How the lyrics are built

Every song follows the same proven structure:

1. **Hook** — the first sung line. It is also the question in the title, so the video starts with the song in the very first second. No greeting, no logo, no intro.
2. **Chorus** — 4 short lines that repeat after every verse, so kids can sing along by the second listen.
3. **Verse 1–4** — 4 short lines each. Every verse has **one copyable action** (for example "Splash the water", "Hop like a bunny", "Point to something red") that a child can copy while watching.

The full lyric sheet the tool shows repeats the chorus after every verse, so what you copy is a complete, singable song.

## How the SEO text is built

**Title shape** (always the same shape, only the topic words change):

```
[Moment]! [Direct question]? | [Topic] Song with Taffy | Nursery Rhymes for Toddlers & Preschoolers
```

Example (Bath Time):

```
Splish Splash Time! Can You Wash Your Toes with Taffy? | Bath Time Song with Taffy | Nursery Rhymes for Toddlers & Preschoolers
```

**Description** — a short paragraph that starts with the hook in quotes, says the song is original and made for toddlers and preschoolers, and ends with a subscribe line.

**Hashtag block** — always this fixed block, with only the topic tag changing:

```
#TaffyTunes #NurseryRhymes #KidsSongs #Shorts #ToddlerLearning #PreschoolLearning #SingAlong #BabySongs #ChildrensSongs #[Topic]Song
```

Example (Bath Time): the last tag is `#BathTimeSong`.

## Music-fit moods

Each topic carries a mood, and the tool tells you what kind of copyright-free track fits:

| Mood | Meaning | Use for |
|------|---------|---------|
| Cheerful | Bright, bouncy track — fast, happy feel | Bath Time, Numbers, Colors, Family, ABC, Good Manners |
| Playful | Bouncy, giggly track — fun and light | Brushing Teeth, Animals, Food |
| Calm | Soft, gentle track — slow and soothing | Bedtime, Rain |
| Dance | Upbeat dance track — clap and move along | Playground |

Rule the tool reminds you of: use a **different** copyright-free track in every video, and put that track's credit line in the description.

## How to use it — step by step

1. Open `index.html` in any modern browser (Chrome, Firefox, Edge, Safari — desktop or phone). No install, no server.
2. **Step 1 — Pick a topic.** Tap one of the 12 topic buttons. It turns yellow when selected, and a music-fit hint appears underneath.
   - Don't know which one? Press **🎲 Surprise me** — it picks a random topic and generates the song at once.
3. Press **✨ Generate my song**.
4. **Step 2 — Your song.** The page shows, in order:
   - The **HOOK** in a big yellow box — this is the first line Taffy sings.
   - The **full lyrics** (hook + chorus + 4 verses, chorus repeating).
   - The **SEO title**.
   - The **description**.
   - The **hashtags**.
   - The **music fit** (mood + what kind of track to use).
5. Copy what you need with the **📋 Copy** button under each block. The button briefly turns green and says "✅ Copied!".
6. Paste into your video plan / YouTube Studio. Pick a different topic and generate again for the next Short.

### Copy buttons

There is one copy button per block: **Copy lyrics**, **Copy title**, **Copy description**, **Copy hashtags**. Each copies exactly the text shown in its block — nothing else. If your browser blocks the modern clipboard API, the tool falls back to the classic copy method automatically.

## How to run it

There is nothing to install and nothing to build.

- **Double-click `index.html`** — it opens in your browser and works.
- **Or serve it:** `python3 -m http.server` in this folder, then open `http://localhost:8000`.
- **Or host it:** copy this folder to any static host (GitHub Pages, Netlify, Vercel). It is one HTML file; no backend is needed.
- It works **offline** — there are no external scripts, fonts, or images. All styling is plain CSS in the file.

## File list

```
taffytunes-song-maker/
├── index.html   — the whole app: page, styling, all 12 topics, all lyrics, generator logic
├── README.md    — this file
└── LICENSE      — MIT License
```

## Original lyrics

All lyrics in this tool are **original** — written for this project. They copy no existing song, rhyme, or character. You may use the generated lyrics in your own videos.

## How to contribute

Contributions are welcome — new topics, better lyrics, new features. The flow is the standard GitHub flow:

1. **Fork** this repository (the Fork button, top right on GitHub).
2. **Clone** your fork to your computer: `git clone https://github.com/YOUR-USERNAME/taffytunes-song-maker.git`
3. **Create a branch** for your change: `git checkout -b add-new-topic`
4. **Make your change** in `index.html` (everything lives in that one file) and test it by opening the file in a browser.
5. **Commit** with a clear message: `git commit -m "Add 'Sharing Snacks' topic"`
6. **Push** to your fork: `git push origin add-new-topic`
7. **Open a Pull Request** on GitHub, describing what you changed and why.

### Adding a new topic

Add one object to the `TOPICS` array in `index.html`. Every field is required — no field may be left empty:

```js
{
  id: "sharing",                       // short, lowercase, no spaces — used internally
  name: "Sharing Snacks",              // shown on the button and in the title
  emoji: "🍪",                          // shown on the button
  mood: "cheerful",                    // one of: cheerful | calm | playful | dance
  moment: "Snack Time!",               // first half of the SEO title
  question: "Can You Share Your Snacks with Taffy?",  // second half of the SEO title
  hook: "Share, share, share a snack!",// first sung line
  chorus: [ "line 1", "line 2", "line 3", "line 4" ],  // exactly 4 lines
  verses: [                            // exactly 4 verses
    { action: "Pass the plate", lines: [ "line 1", "line 2", "line 3", "line 4" ] },
    { action: "Take a bite",    lines: [ "line 1", "line 2", "line 3", "line 4" ] },
    { action: "Say thank you",  lines: [ "line 1", "line 2", "line 3", "line 4" ] },
    { action: "Share again",    lines: [ "line 1", "line 2", "line 3", "line 4" ] }
  ]
}
```

Rules for new lyrics: original words only (never copy a published song), simple words a toddler can follow, one copyable action per verse, and a hook that works as the very first sung line.

### Adding a new mood

Add an entry to the `MOODS` object in `index.html` with a `label` and a `hint` (one or two sentences saying what kind of track fits), then use its key as a topic's `mood`.

### Reporting a bug

Open an Issue on GitHub: say which browser you used, which topic you picked, and what went wrong (a screenshot helps).

## License

MIT License — see [LICENSE](LICENSE). Free to use, copy, modify and share, including for commercial videos.
