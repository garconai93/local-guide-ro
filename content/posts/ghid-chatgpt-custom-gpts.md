---
title: "Ghid ChatGPT Custom GPTs: Creează asistenți virtuali personalizați"
date: 2026-04-01
draft: false
description: "Ghid complet pentru Custom GPTs în ChatGPT. Cum să creezi asistenți virtuali personalizați pentru afacerea ta, educație sau productivitate — fără programare."
keywords: ["ChatGPT", "Custom GPTs", "GPT Builder", "AI assistant", "prompt engineering", "ChatGPT Plus", "automation"]
image: "chatgpt-custom-gpts.jpg"
tags: ["ChatGPT", "AI", "Custom GPTs", "Automatizare", "Tutorial"]
readingTime: "13 min"
---

# 🤖 Ghid ChatGPT Custom GPTs: Creează asistenți virtuali personalizați

Custom GPTs sunt versiuni personalizate ale ChatGPT pe care le poți crea fără să fii programator. Poți antrena un GPT să fie consultant de marketing, asistent juridic, profesor de limbi străine sau orice alt rol. Acest ghid îți arată cum să le creezi și să le optimizezi.

---

## 🌟 Ce sunt Custom GPTs?

Custom GPTs (Generative Pre-trained Transformers) sunt variante ale ChatGPT pe care le configurezi tu:
- **Instrucțiuni personalizate** (System Prompt)
- **Cunoștințe specifice** (Knowledge base)
- **Acțiuni** (Actions — se conectează la API-uri)
- **Capabilități activate/dezactivate**

---

## 🏗️ Partea 1: Cum creezi un Custom GPT

### Pasul 1: Accesează GPT Builder

1. Login pe [chat.openai.com](https://chat.openai.com)
2. Click pe **„Explore"** în sidebar
3. Click pe **„Create a GPT"**
4. Se deschide GPT Editor

### Pasul 2: Configurează „Configure"

**Create tab:**
```
- Profile picture (optional)
- Name: [Numele asistentului]
- Description: [Ce face]
```

**Configure tab:**
```
- Instructions: [System prompt detaliat]
- Conversation starters: [Întrebări indicative]
- Knowledge: [Fisiere upload]
- Capabilities: [Web browsing, DALL-E, Code interpreter]
- Actions: [Pentru conectare API]
```

---

## 📝 Partea 2: System Prompt — Inima Custom GPT-ului

### Structura unui System Prompt eficient

```
# Role
Ești [ROL], specializat în [DOMENIU].

# Personalitate
- Ton: [formal/casual/prietenos]
- Stil: [concise/detaliate/explicative]
- Limbaj: [română/engleză/ambele]

# Expertiză
Ești expert în:
1. [Domeniu 1]
2. [Domeniu 2]
3. [Domeniu 3]

# Comportament
## Ce faci:
- [Acțiune pozitivă 1]
- [Acțiune pozitivă 2]

## Ce NU faci:
- [Limitare 1]
- [Limitare 2]

# Output Format
Răspunzi în format:
- [Markdown cu headings]
- [Liste bullet]
- [Tabele când e relevant]
```

### Exemple de Custom GPT prompts

**1. Copywriting Assistant:**
```
Ești Expert Copywriter cu 15 ani experiență.
Tone: convingător, clar, orientat pe rezultate.
- Creezi headline-uri care captarea atenția
- Scrii beneficii, nu caracteristici
- Incluzi CTA clar în fiecare text
- Respecti structura: Hook → Problem → Solution → CTA
NU folosești jargon inutil sau superlative exagerate.
```

**2. Teacher AI:**
```
Ești Tutor Personal cu rabdare nelimitată.
- Explici conceptele în mai multe moduri
- Adapți limbajul la nivelul elevului
- Dai exemple concrete și analogii
- Creezi exerciții practice
- Verifici înțelegerea cu întrebări de control
Nu dai răspunsuri directe la exerciții — ghidezi spre răspuns.
```

---

## 📚 Partea 3: Knowledge — Baza de cunoștințe

### Ce poți încărca

| Tip fișier | Limită | Conținut |
|------------|--------|----------|
| PDF | 500 pagini | Documente, cărți |
| TXT | 10MB | Texte |
| DOCX | - | Documente Word |
| CSV | - | Date tabelare |
| JSON | - | Date structurate |

### Best practices Knowledge

1. **Curăță documentele** — înlătură ce nu e relevant
2. **Structură clară** — HEADING-uri, liste
3. **Index-rează** — GPT poate căuta în Knowledge
4. **Actualizează periodic** — versiuni proaspete

### Ce să pui în Knowledge

✅ **Da:**
- Documentație produs/serviciu
- Proceduri interne
- FAQ
- Exemple de proiecte
- Prețuri, pachete

❌ **Nu:**
- Date personale clienți
- Parole sau credentials
- Informații confidențiale

---

## 🔗 Partea 4: Actions — Conectare la lumea reală

Actions permit GPT-ului să facă acțiuni în lumea reală:

### Tipuri de Actions

| Action | Ce face |
|--------|--------|
| **API call** | Preia sau trimite date la un API |
| **Web search** | Caută informații pe web |
| **Generate image** | Creează imagini cu DALL-E |

### Exemplu: Weather GPT
```json
{
  "name": "weather_check",
  "description": "Verifică vremea pentru o locație",
  "parameters": {
    "type": "object",
    "properties": {
      "location": {
        "type": "string",
        "description": "Orașul pentru vreme"
      }
    }
  },
  "action": "http://api.weather.com/v3/wx/current"
}
```

---

## 🎯 Partea 5: Prompts pentru Custom GPTs populare

### 1. SEO Content Writer
```
Creezi conținut SEO optimizat pentru Google.
Pentru fiecare articol:
1. Keyword research (principala + secundare)
2. Title tag optimizat (<60 caractere)
3. Meta description (150-160 caractere)
4. Headings H1, H2, H3 cu keywords
5. Content 1500+ cuvinte, informațional
6. Internal + external links
7. FAQ section
```

### 2. Code Reviewer
```
Ești Senior Developer cu 10+ ani experiență.
Faci code review pe [limbaj selectat]:
- Security vulnerabilities
- Performance issues
- Best practices
- Code readability
- Testing coverage
Oferi feedback specific cu exemple de îmbunătățire.
```

### 3. Personal Trainer
```
Ești Antrenor Personal Certificat.
 creezi:
- Plan antrenament săptămânal (obiectiv: [scop])
- Explicații tehnici exerciții
- Warm-up și cool-down
- Progresie încărcătură
- Video demo (prin DALL-E pentru ilustrații)
Întrebi despre: echipament, accidentări, nivel experiență.
```

### 4. Travel Planner
```
Ești Expert în Călătorii cu cunoștințe vaste despre [destinație].
Planifici itinerarii complete:
- Zile cu activități detaliate
- Locuri de mâncare (buget: [buget])
- Transport între puncte
- Sfaturi locale (off the beaten path)
- Buget estimat breakdown
```

---

## 💰 Partea 6: Monetizare cu Custom GPTs

### Modele de venit

| Model | Descriere |
|-------|-----------|
| **Abonament** | $20/lună per utilizator |
| **Freemium** | Versiune gratuită + Premium |
| **B2B** | License pentru companii |

### Custom GPTs populare pentru vânzare

- [ resume Builder](https://chat.openai.com/gpts) — constructori de CV
- **Email Campaign Generator** — pentru marketeri
- **Legal Document Drafter** — contracte, politici
- **Financial Advisor** — planificare buget
- **Language Tutor** — lecții personalizate

---

## 🔗 Resurse

💻 **Instrumente:**
- [ChatGPT](https://chat.openai.com) — necesită Plus ($20/lună)
- [GPT Store](https://openai.com/blog/gpts) — descoperă GPTs
- [Custom GPT Documentation](https://help.openai.com) — tutoriale oficiale

📚 **Cărți (affiliate):**
- [Engineering Prompts - Anton Osika](https://www.amazon.it) — prompting sistematic
- [The AI Product Manager - Hiro Arai](https://www.amazon.it) — produse AI

---

## 💛 Susține acest ghid

Dacă ți-a fost util, poți să susții proiectul:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru comunitatea românească*
