# leonnariley18-ui/transitions

*a morning commute journal and a night journaling toolkit — two practices, one repo*

No accounts. No subscriptions. No ads. No data sharing. PIN-protected, cloud-synced, hosted on GitHub Pages.

---

## what's in this repo

### transitions — `index.html`

A commute journal for both ends of the day. Morning: vibe check → question selection → writing space, built for the ride between your private world and the performance of the day. Afternoon: no vibe check, straight into a wind-down question picker → writing space, built for the ride home. Designed for the G train, works on any train.

**Live at:** `https://leonnariley18-ui.github.io/transitions/`

### night randomizer — `randomizer.html`

A pre-sleep question randomizer for physical journal practice. Mood-filtered, anchor-first, one re-roll available. Every question comes with a full paragraph explaining what it's doing for your nervous system. No data stored — pairs with a physical journal.

**Live at:** `https://leonnariley18-ui.github.io/transitions/randomizer.html`

---

## transitions — what it does

**Home** — a three-position slider switches between morning, afternoon, and history. A hero photo sits behind the top of the screen (sunrise for morning, dusk for afternoon) and the whole app re-themes to match — light and cool in the morning, warm and dusk-toned in the afternoon. Entry count (not a streak — no pressure).

### morning

**Vibe check** — how are you arriving today? Five options with clarifying descriptions:
- *scattered* — too much in the present
- *heavy* — something already landed
- *anxious* — bracing for what's coming
- *clear* — present and ready
- *okay* — just here, nothing particular

Your vibe shapes which questions surface first on the next screen.

**Question selection** — anchor always loads first. One more question from the bank, surfaced by vibe with the most relevant options at the top. Each question has an info button that explains exactly what it's doing for your nervous system. Cap of anchor + one — enough for a commute, never overwhelming. Skip to writing anytime.

### afternoon

The evening counterpart — winding down instead of gearing up. No vibe check; tap the anchor card straight into the question picker. Pick one or more questions (or none) from two pools: two afternoon-only questions, plus reworded evening versions of two morning-bank questions ("did I let good enough be enough *today*" instead of "what would good enough look like"). Marked with a moon and a small "at night" tag next to the app name.

### writing space

Free-form contenteditable field with full formatting, shared by both modes:
- Text fonts: Playfair Display, Montserrat, DM Sans, Poppins, Raleway, Merriweather, Roboto Slab
- Display fonts (title): Playfair Display, Oswald, Bebas Neue, Chewy, Bagel Fat One, Dancing Script
- Bold, italic, bullet list, font size up/down
- Text color (8 options) and highlight (6 options)
- Toolbar collapses and pulls out with one tap
- Selection is preserved when toolbar is open so formatting applies to the right text
- Title placeholder and save path follow whichever mode you're writing in

**Save draft** — mid-entry save that preserves everything (mode, vibe or selected questions, title, writing, font choices). Lock your phone, switch trains, get interrupted — come back exactly where you left off, in the same mode you left it in. Discard button on home screen clears the draft with one confirmation tap.

### history

A dedicated archive screen, one slider-tap away from home. Search by keyword, filter by mode (☀️ morning / 🌙 afternoon), vibe, and category — vibe filters dim automatically when only afternoon entries are shown, since afternoon entries don't carry a vibe. Read past entries in full (read-only). Export to .txt for sharing and pattern analysis. Kept visually neutral (gray, archival) on purpose — it doesn't shift with time of day the way the rest of the app does.

**Auto-generated entry context** — every entry logs "arrived heavy · wrote through protection + release" so when you read it back months later the full picture is there without any extra effort. Entries saved before afternoon mode existed have no `mode` field and are treated as morning everywhere — no migration needed.

**Sync dot** — top right corner of the writing screen. 🟢 green = synced, 🟡 amber = saving, 🔴 red = sync error.

---

## question bank

The anchor question appears every morning automatically before anything else — it is never a selectable option.

**anchor — every morning, always:**
*What do I want to protect about my energy today?* — category: protection

**second question — picked from the bank based on your vibe:**

| # | question | category | surfaces for |
|---|---|---|---|
| Q1 | What would good enough look like today? | self-compassion | scattered · heavy · okay |
| Q2 | What's one thing I'm bringing my full attention to today? | intention | scattered · clear |
| Q3 | What do I want to leave at the door before I walk in? | boundary | anxious · okay |
| Q4 | How do I want to feel by the time I arrive? | body scan | anxious |
| Q5 | What moment today am I most looking forward to? | presence | clear · okay |
| Q6 | Where am I most likely to lose myself today, and can I stay a little more present there? | awareness | clear |
| Q7 | What's one thing already in place today that I don't have to figure out? | grounding | scattered · anxious |
| Q8 | Is there anything I'm carrying from yesterday that isn't mine to carry today? | release | heavy |

**afternoon question bank** — no vibe-based surfacing; all options are shown at once, multi-select:

| # | question | category | source |
|---|---|---|---|
| Q9 | Where did today actually take me, versus where I thought it was going? | awareness | afternoon-only |
| Q10 | What does my body need in the next two hours? My spirit? My mind? | body scan | afternoon-only |
| Q1 (pm) | Did I let good enough be enough today? | self-compassion | reworded from Q1 |
| Q8 (pm) | Is there anything I'm carrying from today that isn't mine to bring home? | release | reworded from Q8 |

---

## night randomizer — what it does

A companion tool for physical journaling before sleep. No writing happens in the app — it surfaces the questions, explains the reasoning, and sends you to your journal.

**Anchor — every night, always:**
*Is there anything my body is still carrying that I can consciously release?*

The anchor sits at the top with its full reasoning paragraph visible at all times. Below it, you pick your mood and get a second question surfaced from the bank. One re-roll available if the question doesn't land.

**Mood options:** pretty good · in between · it was hard

**Night question bank — Q1 through Q15, labeled for physical journal use:**

| # | question | mood |
|---|---|---|
| Q1 | What did I handle today that I once thought I couldn't? | pretty good |
| Q2 | What moment today felt most like me? | pretty good |
| Q3 | What's one thing I'm proud of, even if it's tiny? | pretty good |
| Q4 | When did I show grace today — to someone else, or to myself? | pretty good |
| Q5 | Where did I show up for someone today, even in a small way? | pretty good · in between |
| Q6 | What did I give myself permission for today? | pretty good · in between |
| Q7 | What did my body need today, and did I listen? | in between · hard |
| Q8 | What moment today do I want to remember? | in between |
| Q9 | What was the emotional texture of today — and what drove it? | in between |
| Q10 | Where was I performing today, and where was I actually myself? | in between · hard |
| Q11 | Today was hard. What did I still manage, despite that? | hard |
| Q12 | What was hard today, and what does that say about what I care about? | hard |
| Q13 | What would I say to a friend who had the exact day I just had? | hard |
| Q14 | Did I let good enough be enough today? | hard |
| Q15 | What did my body need today, and did I listen? | hard |

Every question surfaces with its full reasoning paragraph explaining what it's doing for your nervous system — no info button needed, it just comes with the question.

A printable question key is also available for physical journal reference — printed and kept in the journal, not hosted online.

---

## tech stack

| | transitions | night randomizer |
|---|---|---|
| language | vanilla HTML/JS — single file | vanilla HTML/JS — single file |
| database | Supabase (PostgreSQL) | none — pairs with physical journal |
| auth | PIN-based (hashed token) | none |
| hosting | GitHub Pages | GitHub Pages |

---

## infrastructure

**Supabase project:** shared with cycle app (`sdvmycusfyavsuvsjvrv`)
**Table:** `transitions_data`

Same PIN as the cycle app. One PIN unlocks both. Data stored as a JSON array of entries per user — vibe, categories, title, body text, date, and context line all stored per entry.

The cycle repo's GitHub Actions workflow pings this Supabase project twice a week to prevent free-tier pauses.

---

## installing transitions on device

**Android (Chrome)**
1. Open Chrome → navigate to `https://leonnariley18-ui.github.io/transitions/`
2. Tap ⋮ menu → Add to Home Screen → Add

**iPhone/iPad (Safari only)**
1. Open Safari → navigate to `https://leonnariley18-ui.github.io/transitions/`
2. Tap Share → Add to Home Screen → Add

The night randomizer and question key are browser-only tools — bookmark them rather than installing.

---

## files in this repo

| file | what it is |
|---|---|
| `index.html` | transitions app — morning + afternoon journal, history screen |
| `bg-morning.jpg` | home screen hero photo, morning mode |
| `bg-afternoon.jpg` | home screen hero photo, afternoon mode |
| `manifest.json` | PWA manifest for home screen installation |
| `icon-192.png` | app icon 192px |
| `icon-512.png` | app icon 512px |
| `randomizer.html` | night journal question randomizer |
| `night-windows.jpg` | night journal hero photo, tonight tab |
| `night-moon.jpg` | night journal hero photo, past self tab |

---

## related apps

| app | repo | what it does |
|---|---|---|
| cycle | [leonnariley18-ui/cycle](https://github.com/leonnariley18-ui/cycle) | period and phase tracker |
| The Cloud | [leonnariley18-ui/the-cloud](https://github.com/leonnariley18-ui/the-cloud) | private terpene journal |

---

## future

- Anchor rotation — anchor question revisits seasonally based on what patterns emerge in the writing
- Pattern insights — which vibes cluster on which days, which question categories you reach for most
- cycle × transitions connection — surface your current phase on the transitions home screen so the morning practice is informed by where you are in your cycle
- Morning question bank expansion — new questions added as the practice evolves
- Night randomizer data — optional lightweight logging so night patterns can be analyzed alongside morning ones

---

*built entirely with [Claude](https://claude.ai) · single HTML files · no frameworks*  
