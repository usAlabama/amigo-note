# 📘 Notepad ....🖍

A powerful, privacy-focused text editor that runs entirely in your browser — no server, no tracking, no installation required.

## ✨ Features

### 🎨 Design & Themes
- **3 preset themes**: Light, Dark, Sepia
- **Custom color mode**: Pick any background color — text auto-adjusts for contrast
- **Smooth transitions**: All UI changes animate smoothly
- **Responsive layout**: Works on desktop, tablet, and mobile

### ✍️ Rich Text Formatting
- Bold, Italic, Bold+Italic
- Underline, Strikethrough, Monospace
- Hidden text (click to reveal)
- Links, Blockquotes
- One-click insert: 200+ special characters & emojis

### 🌐 Multi-Language Interface
- Switch UI language instantly: **English / Русский / Українська**
- Independent spellcheck language selector (EN/RU/UA)
- All interface text, buttons, and messages are localized

### 🔀 Split View Mode
- Toggle between single and dual-pane layout
- Left pane: Draft / Right pane: Final version
- Optional scroll sync between panes

### 💾 Export & Save
- Export to: `.txt`, `.md`, `.js`, `.html`, `.json`
- Auto-save to browser localStorage (offline-first)
- One-click copy to clipboard

### 🔒 Privacy & Offline
- 100% client-side — no data leaves your device
- Works without internet after first load
- No analytics, no cookies, no tracking

## ⚙️ Customization

### Change the Favicon (Tab Icon)

## Find this line in `<head>`:
```html
<link rel="icon" type="image/svg+xml" href="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'><rect width='100' height='100' fill='%233b82f6' rx='14'/><text x='50' y='72' font-size='65' font-weight='700' font-family='system-ui,sans-serif' fill='white' text-anchor='middle'>N</text></svg>">

## Edit the values to customize:

🟢 Green + "P" fill='%2310b981' >P</text>
🟣 Purple + "✓" fill='%238b5cf6' >✓</text>
⚫ Dark + "✎" fill='%231e293b' >✎</text>

💡 Tip: %23 is the URL-encoded # symbol. Always keep rx='14' for rounded corners.

## Change Default Settings

## Edit the DEFAULT_SETTINGS object in the <script> section:

const DEFAULT_SETTINGS = {
    theme: 'light',           // 'light' | 'dark' | 'sepia' | 'custom'
    dialogColor: '#ffffff',   // Default editor background
    fontSize: 16,             // Default font size (10-32)
    splitMode: false,         // Start with split view?
    customThemeColor: '#10b981', // Default custom theme color
    interfaceLang: 'en'       // 'en' | 'ru' | 'uk'
};

## 🛠️ Tech Stack
Pure HTML5, CSS3, Vanilla JavaScript (no frameworks)
CSS Custom Properties for theming
contenteditable + execCommand for rich text
localStorage for persistence
Blob API for file exports
WCAG-compliant contrast calculations
