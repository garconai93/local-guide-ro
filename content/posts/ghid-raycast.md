---
title: "Ghid Raycast: Launcher-ul suprem pentru Mac — productivitate în seconds"
date: 2026-04-01
draft: false
description: "Ghid complet Raycast pentru Mac. Launcher rapid, snippets, window management, clipboard history și automation. Înlocuiește Spotlight cu Raycast pentru productivitate maximă."
keywords: ["Raycast", "Mac", "launcher", "productivitate", "snippets", "clipboard", "window management", "macOS"]
image: "raycast-launcher.jpg"
tags: ["Raycast", "Mac", "Productivitate", "Launcher", "Tutorial"]
readingTime: "10 min"
---

# 🚀 Ghid Raycast: Launcher-ul suprem pentru Mac

Raycast este un launcher pentru macOS care înlocuiește Spotlight cu **viteze amețitoare**, **extensii puternice** și **automatizări**. Dacă petreci timp navigând prin foldere sau căutând fișiere, Raycast îți economisește minute în fiecare zi. Acest ghid te transformă în utilizator Raycast expert.

---

## 🌟 De ce Raycast? Spotlight vs Raycast

| Funcție | Spotlight | Raycast |
|---------|-----------|---------|
| Viteză | Rapid | **Mai rapid** (Rust vs Objective-C) |
| Clipboard history | Nu | **Da, nelimitat** |
| Snippets | Nu | **Da** |
| Window management | Nu | **Da (内置)** |
| Extensions | Nu | **100+ extensii** |
| Window Snapping | Nu | **Da** |
| Price | Free | **Gratuit + Pro ($8/lună)** |

---

## ⚡ Partea 1: Instalare și setup

### Instalează Raycast

1. Descarcă de pe [raycast.com](https://raycast.com)
2. Instalează aplicația
3. La prima rulare, Raycast te ghidează:
   - Setează shortcut-ul (⌘ + Space implicit)
   - Importă din Spotlight (opțional)
   - Instalează extensii populare

### Setup inițial

```
1. ⌘ + , (sau click pe icon → Preferences)
2. General → Setări display
3. Appearance → Lumină/întuneric
4. Extensions → Instalează cele necesare
5. Advanced → Configurare avansată
```

---

## 🔍 Partea 2: Căutare și navigare

### Comenzi de bază

| Scurtătură | Acțiune |
|------------|---------|
| `⌘ + Space` | Deschide Raycast |
| `Esc` | Închide Raycast |
| `↑ ↓` | Navigatează rezultate |
| `Enter` | Selectează |
| `⌘ + Enter` | Open în Finder |
| `⌘ + Y` | Quick Look (previzualizare) |

### Tipuri de căutare

#### 1. Aplicații
```
Tastează numele app-ului → Enter pentru a deschide
```

#### 2. Fișiere
```
"nume fisier" → caută în sistem
```

#### 3. Calculatoare
```
234 * 567 → rezultat instant
100 EUR in USD → convertire
```

#### 4. Conversii
```
100 km in miles
22 celsius in fahrenheit
```

#### 5. Comenzi de sistem
```
"wifi" → toggle wireless
"bluetooth" → toggle
"volume 50%" → setează volumul
```

---

## 📋 Partea 3: Clipboard History — Frânt întrerupt?

Clipboard History este **cel mai mare selling point** al Raycast:

### Funcționare

```
⌘ + Shift + V → deschide clipboard history
```

### Ce stochează

- Texte copiate
- Images (până la 1MB)
- Links
- Code snippets
- Fișiere (shortcuts)

### Features avansate

| Funcție | Descriere |
|---------|-----------|
| **Search** | Caută în istoricul clipboard |
| **Pin** | Fixed items care nu dispar |
| **Favorites** | Păstrează cele mai folosite |
| **Ignore apps** | Nu înregistra anumite apps |

### Settings pentru Clipboard

```
Preferences → Extensions → Clipboard History
- Max items: 2000
- Store images: Da
- Clear after: 30 zile
- Ignore apps: [AppStore, etc.]
```

---

## ✂️ Partea 4: Snippets — Texte predefinite

Snippets îți permit să înlocuiești texte lungi cu **shortcuts**:

### Setup Snippets

1. Raycast → Extensions → Snippets
2. Click **+** pentru a adăuga
3. Completează:

```
Title: Adresa email
Trigger: /email
Content: john.doe@email.com
```

### Exemple utile de Snippets

| Trigger | Content |
|---------|---------|
| `/addr` | Adresa ta completă |
| `/sig` | Signatura email |
| `/iban` | Contul IBAN |
| `/ccc` | Cod fiscal |
| `/wifi` | WiFi name + password |
| `/md` | Template Markdown |

### Variable Snippets

```javascript
{{date}} // Data curentă
{{time}} // Ora curentă
{{clipboard}} // Conținutul clipboard-ului
{{cursor}} // Unde se oprește cursorul
```

---

## 🪟 Partea 5: Window Management

Raycast are **window management încorporat**:

### Comenzi window

| Trigger | Acțiune |
|---------|---------|
| `window left` | Mută fereastra în stânga |
| `window right` | Mută fereastra în dreapta |
| `window top` | Mută sus |
| `window bottom` | Mută jos |
| `window center` | Centrează |
| `window full` | Full screen |
| `window quarter` | Un sfert din ecran |

### Preset layouts

```
Preferences → Window Management → layouts
Creezeșă layout-uri custom pentru monitorul tău
```

---

## ⚡ Partea 6: Extensions (Store)

Raycast Extensions extind funcționalitatea:

### Extensions esențiale

| Extension | Ce face |
|-----------|---------|
| **1Password** | Accesează parole |
| **Notion** | Quick add tasks |
| **GitHub** | Quick search repos |
| **Figma** | Browse files |
| **Spotify** | Control music |
| **VS Code** | Open projects |
| **Google Chrome** | Bookmarks, tabs |

### Instalează Extensions

```
1. ⌘ + , → Extensions
2. Browse Store
3. Click Install
4. Configure (unele necesită API keys)
```

---

## 🔗 Partea 7: Script Commands

Script Commands permit automatizări custom:

### Exemple de Script Commands

```bash
#!/bin/bash
# Nou fișier în Desktop
touch ~/Desktop/"$1".txt
echo "✅ Creat $1.txt"
```

### Script-uri populare

| Script | Funcție |
|--------|--------|
| **New File** | Creează fișier rapid |
| **Git Status** | Vezi status repo |
| **Kill Port** | Oprește proces pe port |
| **IP Address** | Afișează IP-urile |

---

## 🔗 Resurse

💻 **Instrumente:**
- [Raycast](https://raycast.com) — gratuit (Pro opțional)
- [Raycast Store](https://raycast.com/store) — extensions
- [Raycast API](https://raycast.com/developers) — pentru developers

📚 **Cărți (affiliate):**
- [Mac Power User - David Sparks](https://www.amazon.it) — tehnici avansate Mac
- [Thinking in Systems - Donella Meadows](https://www.amazon.it) — sisteme și productivitate

---

## 💛 Susține acest ghid

Dacă ți-a fost util, poți să susții proiectul:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru comunitatea românească*
