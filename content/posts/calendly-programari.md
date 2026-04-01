---
title: "Cum să-ți gestionezi programările cu Calendly"
date: 2026-04-01
draft: false
description: "Ghid complet pentru utilizarea Calendly: crearea de tipuri de programări, integrarea cu Google Calendar, embed pe website, automatizări și sfaturi pentru a maximiza eficiența."
keywords: ["Calendly", "programări", "calendar", "scheduler", "productivitate", "meetings"]
image: "calendly-cover.jpg"
tags: ["Calendly", "Programări", "Productivitate", "Tutorial"]
readingTime: 7 min
---

# 📅 Cum să-ți gestionezi programările cu Calendly

Calendly a revoluționat modul în care profesioniștii își gestionează programările, eliminând interminabilele往返 de email-uri pentru a găsi un moment potrivit. Cu Calendly, clienții, colegii sau partenerii pot programa singuri o întâlnire în câteva click-uri — direct în calendarul tău disponibil. În acest ghid complet, vei învăța cum să configurezi Calendly de la zero și cum să-l folosești pentru a-ți оптимиза calendarul și a atrage mai mulți clienți.

---

## 🌟 De ce Calendly?

### Avantaje principale

| Avantaj | Descriere |
|---------|-----------|
| **Zero email-uri** | Clienții programaă direct, fără confirmări |
| **Timezone smart** | Convertește automat în fusul orar al clientului |
| **Calendar sync** | Sincronizare cu Google, Outlook, iCloud |
| **Embed pe website** | Widget de programare direct pe pagină |
| **Tipuri multiple** | 15 min, 30 min, 60 min — diferite tipuri de meeting |
| **Automatizări** | Remind-uri, follow-up, integrare CRM |

### Cine folosește Calendly?

| Profesie | Utilizare |
|----------|-----------|
| **Sales** | Demo calls, discovery calls |
| **Recruiters** | Interviuri cu candidați |
| **Coaches/Consultants** | Sesiuni 1-on-1 cu clienți |
| **Freelancers** | Briefings cu clienți |
| **Executives** | Management de CEO calendar |

---

## 📋 Planuri disponibile

| Plan | Preț | Funcții |
|------|------|---------|
| **Free** | €0 | 1 tip de eveniment, sync 1 calendar |
| **Standard** | €8/user/lună | Tipuri multiple, embed, reminders |
| **Pro** | €16/user/lună | Custom branding, analytics, workflows |
| **Teams** | €20/user/lună | Paginated scheduling, admin controls |

---

## 🚀 Setup inițial — Ghid pas cu pas

### Pasul 1: Crearea contului

1. Accesează [calendly.com](https://calendly.com) și înregistrează-te
2. Conectează calendarul principal (Google sau Outlook)
3. Setează fusul orar preferat
4. Completează profilul public

### Pasul 2: Conectarea calendarului

**Pentru Google Calendar:**
1. Setări → Connected Calendars
2. Click **Connect a Calendar**
3. Autorizează acces în Google
4. Selectează calendarul de disponibilitate

**Pentru Outlook:**
1. Similar — conectează contul Microsoft
2. Sincronizarea este automată

### Pasul 3: Setarea disponibilității

**Weekly Availability:**

```
Luni: 09:00 - 12:00, 14:00 - 18:00
Marți: 09:00 - 12:00, 14:00 - 18:00
Miercuri: 09:00 - 12:00, 14:00 - 18:00
Joi: 09:00 - 12:00, 14:00 - 18:00
Vineri: 09:00 - 14:00
Sâmbătă-Duminică: Indisponibil
```

---

## 📆 Crearea tipurilor de programări

### Tipuri de evenimente

| Tip | Durată | Scop |
|-----|--------|------|
| **Intro Call** | 15 min | Primul contact, întrebări rapide |
| **Discovery Call** | 30 min | Evaluay client potențial |
| **Demo** | 45 min | Prezentare produs/serviciu |
| **Consulting** | 60 min | Sesiune de lucru |
| **Follow-up** | 15 min | Check-in după meeting |

### Crearea unui nou tip de eveniment

1. Click **Event Types** → **New Event Type**
2. Completează:

| Câmp | Ce să pui |
|------|----------|
| **Name** | „Discovery Call 30 minute" |
| **Slug** | „discovery-call" (apare în URL) |
| **Duration** | 30 minute |
| **Location** | Google Meet / Zoom / Phone / In-person |
| **Description** | Ce să știe clientul despre meeting |
| **Color** | Alege o culoare pentru identificare |

### Settings avansate

| Setare | Recomandare |
|--------|-------------|
| **Scheduling window** | Max 60 zile în avans |
| **Minimum notice** | 24 ore înainte |
| **Buffer time** | 5-15 min între meeting-uri |
| **Invitees limit** | 1 per slot (sau mai mulți) |
| **Questions** | Adaugă câmpuri (nume companie, topic) |

---

## 🔗 Integrarea cu video conferință

### Google Meet (gratuit)

1. Installează extensia Calendly Chrome
2. Sau conectează Google Calendar — Meet se generează automat

### Zoom

1. Integrations → Zoom
2. Click **Connect**
3. Autorizează acces
4. Zoom join links se generează automat

### Alte opțiuni

| Platformă | Setup |
|-----------|-------|
| **Microsoft Teams** | Integrare Zoom/Microsoft |
| **Whereby** |生成 meeting room link |
| **Phone/SMS** | Call-in number |
| **In-person** | Address sau locație |

---

## 🌐 Embed pe website

### Opțiunea 1: Inline embed

```html
<!-- Copiază codul din Calendly → Share → Add to Website -->
<div class="calendly-inline-widget" 
     data-url="https://calendly.com/username/discovery-call"
     style="min-width:320px;height:630px;">
</div>
<script type="text/javascript" src="https://assets.calendly.com/assets/external/widget.js"></script>
```

### Opțiunea 2: Popup din buton

```html
<button onclick="Calendly.initPopupWidget({url: 'https://calendly.com/username/discovery-call'});return false;">
  Programează un call
</button>
```

### Opțiunea 3: Link direct

Pur și simplu trimite link-ul:
```
https://calendly.com/username/discovery-call
```

---

## ⚙️ Automatizări și reminders

### Automatic reminders (Pro plan)

| Când | Ce se trimite |
|------|---------------|
| **24 ore înainte** | Email reminder + calendar invite |
| **15 min înainte** | SMS reminder (dacă e activat) |
| **După meeting** | Thank you email + feedback request |

### Workflows automation (Pro plan)

Creează automatizări like:

```
IF: New booking
THEN:
  - Adaug în CRM (HubSpot, Salesforce)
  - Trimit email de confirmare personalizat
  - Postez în Slack channel #sales-leads
```

### Follow-up emails

Personalizează email-ul de follow-up:

```markdown
Subiect: Mulțumesc pentru timpul de azi!

Bună {{name}},

Mulțumesc că ai avut timp să discutăm azi despre {{topic}}.

Următorii pași:
1. Îți trimit propunerea până mâine
2. Vorbești cu echipa
3. Revenim săptămâna viitoare

Ai întrebări până atunci? Răspunde direct la acest email.

Best,
[Numele tău]
```

---

## 📊 Analiză și optimizare

### Metrics disponibile (Pro plan)

| Metric | Ce spune |
|--------|----------|
| **Completion rate** | % din vizite care programează |
| **Avg. booking lead time** | Cu cât înainte programează |
| **Cancellation rate** | % anulări |
| **No-show rate** | % care nu s-au prezentat |
| **Top event types** | Care tip de meeting e cel mai cerut |

### Cum să-ți îmbunătățești rata de conversie

| Sfat | De ce funcționează |
|------|-------------------|
| Adaugă mai multe sloturi | Mai multe opțiuni = mai multe programări |
| Oferă mai multe tipuri | Fiecare vrea diferite durate |
| Adaugă social proof | „100+ clienți programați" |
| Email personalizat | Ăăează încrederea |
| SMS reminders | Reduce no-show-urile |

---

## 🔒 Setări de securitate și confidențialitate

### Gheți de scheduling

| Setare | Ce face |
|--------|---------|
| **Block before/after** | Nu programa în pauzele de prânz |
| **Max events per day** | Previne suprasolicitarea |
| **Hide event type** | Ascunde anumite tipuri de meeting |
| **Password protect** | Evenimentele necesită parolă |

### Răspunsuri automate

Pentru când ești indisponibil:

```
Bună! Tocmai am primit cererea ta de programare.

Din păcate, în perioada [DATE] sunt în concediu.
Revin în data de [DATA] și te voi contacta imediat.

Pentru urgențe, poți să-mi trimiți email la [email].

— [Nume]
```

---

## 🔗 Resurse și instrumente complementare

🛠️ **Instrumente:**
- [Calendly](https://calendly.com) — accesează platforma
- [Calendly Help](https://help.calendly.com) — documentație
- [Calendly API](https://developer.calendly.com/) — pentru dezvoltatori

📚 **Tutoriale:**
- [Calendly Academy](https://calendly.com/resources/online-training) — cursuri video
- [Calendly Blog](https://calendly.com/blog) — sfaturi și best practices

---

## 💛 Susține acest ghid

Dacă ti-a fost util acest ghid și vrei să susții proiectul Local Guide în Română:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru profesioniștii români care vor să-și elibereze timpul*
