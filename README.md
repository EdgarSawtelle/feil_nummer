# Feil nummer

*En historie i en telefon — a story told through a phone.*

A Norwegian-learning game for A2–B1 learners. You've just moved to Trondheim with your four-year-old daughter Maya. Your new SIM card used to belong to Silje Haugland, 26, who changed her number three weeks ago. Her messages keep arriving: from her teenage brother Jonas, from her grandmother Gunvor, and from someone she doesn't want to hear from. You read and reply in Norwegian, and the people you write to remember what you say.

It is a follow-up to the detective game *Mørkt vann*.

## Play

Open `index.html` in a browser. Everything is in that one file: no install, no internet connection needed after it loads, no account.

It is designed for an iPhone (Safari) and a Boox Note Air (Android e-ink colour) but works in any modern browser. The design is e-ink first: no animations, high contrast, large serif text and large tap targets.

## Put it online with GitHub Pages

1. Create a new repository on GitHub.
2. Upload `index.html` (and this README) to the root of the repository.
3. Go to **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, and save.
4. After a minute the game is live at `https://<your-username>.github.io/<repository-name>/`.

On iPhone, open that address in Safari and use **Share → Add to Home Screen** to get an app-like icon.

## How it plays

- **The whole story happens on the phone.** Open Meldinger, E-post, Kalender, Notater and the bank app to follow what arrives. «Neste dag →» moves time forward when the day is done.
- **Tap any Norwegian word** for its meaning in context, dictionary form, word class and forms, a grammar note, an example, the Bokmål form of dialect and slang, and pronunciation. «⋯» on a message translates the whole message.
- **Reply in three ways:** pick a suggestion (small talk only), build the sentence from word tiles, or type it yourself. Typing earns the most stars and warmer reactions.
- **Check before you send.** You see how the person would react, what went wrong (in English), and a corrected version. Capital letters, punctuation and small typos don't count against you. Hints, and later «Spør Gunvor», never block you; they only lower that reply's stars.
- **Learning tools:** "Dette lærer du" for each chapter, Mine ord (saved words), Glosekort (flashcards with spaced repetition, both directions), Mine feil (your mistakes grouped by grammar point, with practice rounds), and a short quiz after each chapter.

## Audio

Words and messages can be read aloud using the device's own Norwegian voice. The game works fully without audio.

- **iPhone / iPad:** Settings → Accessibility → Spoken Content → Voices → Norwegian → download a voice (e.g. Nora), then reload the page.
- **Android / Boox:** Settings → Language & input (on Boox: Settings → More settings) → Text-to-speech output → **Speech Services by Google** → gear icon → Install voice data → **Norsk bokmål**, then reload the page.

## Saving and moving your progress

Progress saves automatically in the browser you play in. To move it between devices (for example from iPhone to Boox), go to **Innstillinger → Eksporter**, copy the text, then on the other device go to **Innstillinger → Importer** and paste it.

Clearing the browser's website data deletes your progress, so export first if you want a backup.

## Contents

| Chapter | Level | Status |
|---|---|---|
| 1. Et nytt nummer | A2-1 | Playable |
| 2–8 | A2-1 to B1-3 | Outlined (plan, grammar focus and hook visible under «Kapitler») |

## For editing

All story content sits in one clearly marked **DATA SECTION** at the top of the `<script>` in `index.html`. A comment at the start of that section documents the format: chapters, days, messages, emails, calendar entries, tasks with accepted answers, checklists and hints, decisions and conditions, the quiz, and the glossary. The engine below the line `END OF DATA SECTION` doesn't need changes to add a chapter: replace a chapter's outline with its full data and set `status: "ready"`.

Every Norwegian word shown in the game needs a glossary entry. Dialect and slang entries include their Bokmål form.

Characters and companies in the story are invented. Skatteetaten, Helsenorge and NAV are real Norwegian public services.
