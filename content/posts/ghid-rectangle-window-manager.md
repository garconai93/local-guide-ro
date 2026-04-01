---
title: "Ghid Rectangle: Window Manager gratuit pentru Mac — organizează ferestre ca un pro"
date: 2026-04-01
draft: false
description: "Ghid complet Rectangle pentru Mac. Window manager gratuit care împarte ecranul, maximizează și aranjează ferestrele cu shortcut-uri rapide. Alternative la Magnet și Meteor."
keywords: ["Rectangle", "window manager", "Mac", "organizare ferestre", "productivitate", "macOS", "split screen"]
image: "rectangle-window-manager.jpg"
tags: ["Rectangle", "Mac", "Window Manager", "Productivitate", "Tutorial"]
readingTime: "8 min"
---

# 🪟 Ghid Rectangle: Window Manager pentru Mac — Organizează ferestrele ca un pro

Rectangle este un **window manager gratuit pentru macOS** care îți permite să aranjezi ferestrele cu shortcut-uri rapide — fără să plătești pentru Magnet sau să folosești aplicații scumpe. Dacă lucrezi cu mai multe ferestre, Rectangle îți economisește minute în fiecare zi.

---

## 🌟 De ce ai nevoie de un Window Manager?

### Problema: Ferestre haotice

```
❌ Manual: Drag cu mouse-ul, ineffficient
❌ Snap Windows (doar half screen)
❌ Mission Control ajută, dar nu suficient
```

### Soluția: Window Manager

```
✅ Cu Rectangle: Un shortcut = fereastra exact unde vrei
✅ Keyboard-driven = rapid și precis
✅ Free și open source = fără costuri
```

---

## 📥 Partea 1: Instalare și Setup

### Instalează Rectangle

1. **App Store** (gratuit) — versiune basic
   - [Rectangle on App Store](https://apps.apple.com/app/rectangle/id1610985658)
   
2. **GitHub** (complet, recomandat) — última versiune
   - [Rectangle on GitHub](https://github.com/rxhanson/Rectangle)

### Permisiuni necesare

După instalare, Rectangle cere:
```
1. Accessibility permissions
   System Preferences → Security & Privacy → Privacy → Accessibility
   → Adaugă Rectangle în listă

2. Screen Recording (unele funcții)
   System Preferences → Security & Privacy → Privacy → Screen Recording
   → Adaugă Rectangle
```

⚠️ Fără aceste permisiuni, Rectangle nu poate mișca ferestrele.

---

## ⌨️ Partea 2: Scurtături de tastatură

### Scurtături principale

| Scurtătură | Acțiune |
|------------|---------|
| `⌘ + ⌥ + ←` | Stânga jumatate |
| `⌘ + ⌥ + →` | Dreapta jumătate |
| `⌘ + ⌥ + ↑` | Sus jumatate |
| `⌘ + ⌥ + ↓` | Jos jumătate |
| `⌘ + ⌥ + Return` | Center |
| `⌘ + ⌥ + M` | Maximize |

### Preset-uri rapide

| Scurtătură | Acțiune |
|------------|---------|
| `⌘ + ⌥ + 1` | Left third |
| `⌘ + ⌥ + 2` | Left two-thirds |
| `⌘ + ⌥ + 3` | Right third |
| `⌘ + ⌥ + 4` | Right two-thirds |
| `⌘ + ⌥ + ,` | Smaller |
| `� + ⌥ + .` | Larger |

### Screen edges (Snap Zones)

După ce activezi edge snapping, poți:
```
┌─────────────────────────────┐
│       Top Half (↑)          │
├──────────┬──────────────────┤
│          │                  │
│ Left     │    Right         │
│ Half     │    Half          │
│ (←)      │    (→)           │
│          │                  │
├──────────┴──────────────────┤
│       Bottom Half (↓)       │
└─────────────────────────────┘
```

---

## 🎯 Partea 3: Funcții avansate

### 1. Almost Maximized

`⌘ + ⌥ + M` maximizează dar **lasă title bar vizibilă**:
- Poți încă să dai drap și drop
- Vezi numele fișierului
- Mai ușor de reposiționat

### 2. Thirds

Rectangle împarte ecranul în **treimi**:
```
┌───────┬───────┬───────┐
│  1/3  │  1/3  │  1/3  │
│  Left │ Center│ Right │
└───────┴───────┴───────┘
```

**Use case:** 3 documente side-by-side pentru research

### 3. Trailing Snapping

Funcția „Trail" permité multi-monitor:
1. Drag o fereastră spre margine
2. Se activează snap zone
3. Drop unde vrei

### 4. Multi-Monitor

Pentru mai multe monitoare:
- `⌘ + ⌥ + N` — mută fereastra la monitorul următor
- Snap functions lucrează per monitor
- Fiecare monitor are propriile zone

---

## 📐 Partea 4: Configurare avansată

### Rectangle → Preferences

```
📐 General
├── Launch at login ✅
├── Show menu bar icon ✅
└── Show dock icon (optional)

⌨️ Shortcuts
├── Vezi toate shortcut-urile
├── Re-assign dacă intră în conflict
└── Disable shortcuts nedorite

🖥️ Multipe Monitors
├── Enable trailing snap zones
└── Remember window position per app

⚙️ Misc
├── Animation duration (ms)
├── Cursor snap proximity
└── Additional padding
```

### 커stom window sizes

Poți defini dimensiuni custom:
```
1. Preferințe → Sizes
2. Adaugă size nou
3. Setează % din ecran
4. Setează shortcut
```

---

## 🔄 Partea 5: Alternative comparate

| App | Preț | Extra Features |
|-----|------|----------------|
| **Rectangle** | ✅ Gratis | Suficient pentru majoritate |
| **Magnet** | $6.99 | Scurtături + Snap |
| **Mosaic** | $9.99 | Layout-uri preset |
| **Amethyst** | ✅ Gratis, Open Source | Tiling WM avansat |
| **yabai** | ✅ Gratis, CLI | Extrem de configurabil |

### Când să alegi altceva

| Situație | Recomandare |
|----------|-------------|
| Vrei gratuit + simplu | **Rectangle** ✅ |
| Vrei paid, support | **Magnet** |
| Tiling WM style | **Amethyst** |
| CLI/config files | **yabai** |

---

## 💡 Sfaturi pentru workflow

### Setup ideal pentru development

```
┌─────────────────┬─────────────────┐
│                 │                 │
│   VS Code       │   Browser       │
│   (Code)        │   (Docs)        │
│                 │                 │
├─────────────────┼─────────────────┤
│                 │                 │
│   Terminal      │   Slack         │
│   (Commands)    │   (Chat)       │
│                 │                 │
└─────────────────┴─────────────────┘
```

### Setup ideal pentru writing

```
┌─────────────────────────────────┐
│                                 │
│        Document                │
│        (Microsoft Word)         │
│                                 │
├─────────────────────────────────┤
│                                 │
│   Research (Browser)            │
│                                 │
└─────────────────────────────────┘
```

---

## 🔗 Resurse

💻 **Instrumente:**
- [Rectangle - App Store](https://apps.apple.com/app/rectangle/id1610985658) — gratuit
- [Rectangle - GitHub](https://github.com/rxhanson/Rectangle) — latest version
- [Rectangle Pro](https://rectangleapp.com/pro) — $8, extra features

📚 **Cărți (affiliate):**
- [The Productivity Project - Chris Bailey](https://www.amazon.it) — tehnici practice
- [Deep Work - Cal Newport](https://www.amazon.it) — concentrare profundă

---

## 💛 Susține acest ghid

Dacă ți-a fost util, poți să susții proiectul:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru comunitatea românească*
