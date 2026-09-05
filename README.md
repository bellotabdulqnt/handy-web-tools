# Web Tools

Three browser-based tools I designed and built for my own use as a student, then
refined through daily use. Each is a single self-contained HTML file — no build step,
no framework, no server, no account.

**Live:** https://bellotabdulqnt.github.io/handy-web-tools/

---

## Contract Law · Casebook

A 150-card revision deck for CIL 524, structured as a casebook rather than a card pile.

- Eight chapters with a Roman-numeral table of contents, jumpable at any point
- **Mastery tracking** — mark a card as known and it drops out of rotation; a gauge
  shows progress against the full deck
- **Review-only mode** to drill just the cards still marked "still learning"
- Per-card hints, revealable before the answer
- Full-text search across every question and answer
- Shuffle, category filtering, and a "show all cards again" reset
- Keyboard shortcuts throughout: space to flip, arrows to navigate, `M` to mark,
  `/` to focus search, `Esc` to close dialogs
- Swipe navigation and tap-to-flip on mobile
- Light and dark themes, remembered between sessions

**Design notes.** Revising for BUS 440 and CIL 524, I hit the same wall in both:
paragraph after paragraph, almost nothing retained. As an engineering student I was
used to working problems and being told immediately whether I'd got it right, and neither
course offered that. I built the Casebook to force contract law into that shape — question first,
answer second, mastery tracked. Contract law went first because that exam came sooner.

The editorial serif typography is deliberate. Legal material read as a casebook holds
attention differently from the same content in a generic flashcard app, and the deck
gets used for hours at a stretch.

---

## BUS 440 · Mastery Console

A 90-card deck covering management fundamentals, theories and roles, TQM, and
leadership and communication.

Built on the same engine as the Casebook, retargeted: category chips with icons instead
of a chaptered table of contents, and a technical typographic treatment rather than an
editorial one — because the material is frameworks and definitions, not case law.

- Mastery tracking, review-only mode, hints, search, shuffle
- Category filtering by chip
- Same keyboard shortcuts and swipe navigation
- Dark mode toggle

**Design notes.** Building the second deck was the useful part. Separating what was
genuinely reusable — the card engine, mastery state, navigation — from what had to
change for a different subject is what turned a one-off into something I could ship
twice. However, two decks is the point where copy-pasting the engine stops being sensible.
If a third deck was needed, that would mean pulling the card data into its own file and
loading it in, so one fix updates every deck.

---

## Training Checklist

A four-day gym session tracker built for use on a phone, in a gym, with one hand.

- Four tabbed days — Push (Mon), Pull (Wed), Upper (Fri), Lower (Sat) — each
  colour-coded
- Every exercise carries sets, reps, target RPE, rest interval and a form cue
- **Checkbox and weight-log state persists automatically.** Lock the phone mid-set,
  come back, nothing is lost
- Live progress counter and bar per day
- Supersets visually grouped with a coloured bar and A1/A2 labels
- **Footnoted equipment alternatives** on every exercise — two or three substitutes
  each, so an occupied or missing machine doesn't end the session
- Per-day reset

**Design notes.** The two decisions that shaped this were about failure conditions
rather than features. Gym sessions get interrupted, so nothing is held in memory that
isn't written to storage the moment it changes. And equipment in a shared gym is
routinely unavailable, so substitutions are inline on the page rather than something
the user has to go and look up mid-session.

Training content is adapted from Jeff Nippard's Push-Pull-Legs programming, supplemented
with published research on exercise selection. The programme design is his; the
interface, tracking system and equipment-alternative structure are mine.

**Next:** session history across weeks, so progressive overload is visible rather than
remembered.

---

## On how these were built

I'm a mechanical engineer, not a software engineer. My contribution here is the product
side — deciding what these needed to do, designing the interface and interaction flow,
testing them in real use and iterating. I used AI assistance and adapted existing code
for the implementation. I'm currently learning Python properly so that side is my own
too.

---

## Contact

Bello Abdulsalam Temiloluwafe — bellotabdul@gmail.com — https://www.linkedin.com/in/abdulsalam-bello-temiloluwafe/
