# 🇷🇴 Local Guide în Română

Ghiduri detaliate în limba română pentru aplicații și instrumente populare.

🌐 **Live Site:** https://garconai93.github.io/local-guide-ro/

---

## 🚀 Începe rapid

### Cerințe
- [Go](https://go.dev/) ≥ 1.20
- [Hugo Extended](https://gohugo.io/installation/) ≥ 0.123.0

### Instalare locală

```bash
# Clonează repo
git clone https://github.com/garconai93/local-guide-ro.git
cd local-guide-ro

# Instalează tema (submodule)
git submodule update --init --recursive

# Rulează serverul de dezvoltare
hugo server
```

Site-ul va fi disponibil la: `http://localhost:1313`

---

## 📝 Cum să adaugi un ghid nou

### Metoda 1 — Manual

1. Creează un fișier nou în `content/posts/`:

```bash
hugo new content posts/numele-ghidului.md
```

2. Completează frontmatter-ul și conținutul:

```markdown
---
title: "Titlul Ghidului"
date: 2026-04-01
draft: false
description: "Descriere scurtă a ghidului"
keywords: ["cuvânt", "cheie"]
tags: ["Tag1", "Tag2"]
---

# Titlul Ghidului

Conținutul markdown...
```

3. Trimite un **Pull Request** pe GitHub!

### Metoda 2 — Online

1. Fork acest repo
2. Adaugă fișierul direct din interfața GitHub
3. Trimite Pull Request

---

## 📋 Frontmatter — opțiuni disponibile

| Câmp | Descriere | Exemplu |
|------|-----------|---------|
| `title` | Titlul ghidului | `"Cum să folosești Canva"` |
| `date` | Data publicării | `2026-04-01` |
| `draft` | Draft sau publicat | `false` |
| `description` | Descriere SEO | `"Ghid complet..."` |
| `keywords` | Cuvinte cheie SEO | `["Canva", "design"]` |
| `tags` | Etichete pentru categorizare | `["Design", "Tutorial"]` |
| `image` | imagine copertă (opțional) | `"canva-cover.jpg"` |

---

## 🎨 Personalizare

### Modifică titlul și descrierea
Editează `hugo.toml`:

```toml
title = "Numele Tău de Site"
[params]
  description = "Descrierea site-ului tău"
```

### Adaugă link-uri de affiliate/donații
Tot în `hugo.toml`:

```toml
[[params.links]]
  name = "Donează pe Ko-fi"
  url = "https://ko-fi.com/username"
  icon = "💛"
    
[[params.links]]
  name = "Amazon Affiliate"
  url = "https://www.amazon.it"
  icon = "📦"
```

---

## 🌐 Deployment automat

Site-ul este configurat pentru **GitHub Pages** cu GitHub Actions.

La fiecare push pe `main`, site-ul se reconstruiește și publică automat.

### Configurare (dacă repo-ul e fork)

1. Mergi la **Settings → Pages**
2. La "Build and deployment" → Source: **GitHub Actions**
3. Push o modificare și workflow-ul va porni automat

---

## 📚 Plan de conținut

| Aplicație | Status | Prioritate |
|-----------|--------|------------|
| Notion | ✅ Ghid exemplu | - |
| Canva | 📋 De făcut | Înaltă |
| ChatGPT | 📋 De făcut | Înaltă |
| Obsidian | 📋 De făcut | Medie |
| Obsidian Shell Commands | 📋 De făcut | Medie |
| Canva Docs | 📋 De făcut | Medie |
| Leonardo.ai | 📋 De făcut | Medie |
| Gemini CLI | 📋 De făcut | Medie |
| Hemingway App | 📋 De făcut | Scăzută |
| Notion API | 📋 De făcut | Medie |

---

## 💰 Monetizare

### Affiliate Links
Site-ul suportă link-uri affiliate în ghiduri. Exemple:
- Amazon (cărți, software)
- Software subscriptions (Notion Pro, Canva Pro)

### Donații
Buton de donație Ko-fi / Revolut configurat în header și pagini.

---

## 📂 Structura proiectului

```
local-guide-ro/
├── content/
│   ├── posts/          # Ghidurile (markdown)
│   └── about.md         # Pagina "Despre"
├── themes/
│   └── PaperMod/        # Tema Hugo (submodule)
├── hugo.toml            # Configurația site-ului
├── README.md            # Documentația (acest fișier)
└── .github/
    └── workflows/       # GitHub Actions pentru deployment
```

---

## 🛠️ Tehnologii folosite

- **Hugo Extended** — generator site static
- **PaperMod** — tema responsive și rapidă
- **GitHub Pages** — hosting gratuit
- **GitHub Actions** — deployment automat

---

## 📄 Licență

MIT — folosește liber, modifică, distribuie.

---

*Creat cu ❤️ pentru comunitatea românească*

**Autor:** Garcon (@garconai93)
