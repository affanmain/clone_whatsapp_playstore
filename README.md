# Google Play & WhatsApp Web — UI Clones

Two self-contained, single-file HTML front-end clones. No build step, no dependencies, no backend — just open the files in a browser.

## Files

| File | Description |
|------|-------------|
| `Play Store.html` | A responsive Google Play Store mock with browse tabs, categories, search, and an app-detail overlay. |
| `WhatsApp.html` | A WhatsApp Web mock with chat list, message threads, simulated replies, emoji picker, and light/dark themes. |

## Usage

1. Download both files.
2. Open either file directly in any modern browser (Chrome, Edge, Firefox, Safari).
3. No server, installation, or internet connection required.

## Features

### Play Store (`Play Store.html`)
- Sections: **Games, Apps, Movies, Books, Kids**
- Tabs: **For you, Top charts, Categories, New**
- Featured hero carousel, horizontal card rows, ranked lists
- Live search across name / developer / genre
- App detail overlay with stats, screenshots, and "Install" simulation
- Install progress states (Installing → Open)
- Genre filtering, similar-app suggestions

### WhatsApp (`WhatsApp.html`)
- Two-pane layout: chat list + conversation view (responsive; single-pane on mobile)
- Simulated incoming replies with typing indicators
- Message delivery ticks (sent → delivered → read)
- Emoji picker, auto-growing composer, Enter-to-send
- Light/dark theme toggle
- Chats and theme persist via `localStorage`

## Notes

- These are **UI demos only** — there is no real installation, messaging, or network activity.
- All data (apps, chats) is hard-coded in the file's JavaScript for demonstration purposes.
- Play Store: install buttons are visual simulations (~1.6s).
- WhatsApp: clearing browser storage resets chats to the seeded conversations.

## Customization

- **Play Store:** edit the `APPS` array in the `<script>` block to add/change apps, icons, ratings, and descriptions.
- **WhatsApp:** edit `seedData()` to change contacts and messages, or adjust `EMOJIS` and theme CSS variables in `:root` / `[data-theme="dark"]`.