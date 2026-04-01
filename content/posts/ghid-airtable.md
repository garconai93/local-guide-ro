---
title: "Ghid Airtable: Baze de date simple și gratuite pentru oricine"
date: 2026-04-01
draft: false
description: "Ghid complet Airtable. Cum să creezi baze de date online gratuite pentru inventar, CRM,项目管理 și multe altele — fără cunoștințe tehnice."
keywords: ["Airtable", "baze de date", "gratuit", "inventar", "CRM", "organizare", "Airtable tutorial"]
image: "airtable-baze-de-date.jpg"
tags: ["Airtable", "Baze de Date", "Tutorial", "Organizare"]
readingTime: "11 min"
---

# 🗄️ Ghid Airtable: Baze de date simple și gratuite pentru oricine

Airtable combină simplitatea unui spreadsheet cu puterea unei baze de date relaționale. Este perfect pentru cei care vor organizare avansată fără să fie programmează. Acest ghid îți arată cum să creezi sisteme puternice în Airtable.

---

## 🌟 De ce Airtable?

| Avantaj | Descriere |
|---------|-----------|
| 🎨 Interfață familiară | Ca un Excel/Google Sheets, dar mai puternic |
| 🔗 Relații între tabele | Linked records ca o adevărată bază de date |
| 📱 Aplicații mobile | iOS și Android excelente |
| 🔌 Automatizări | Automate, Sync, Blocks |
| 💰 Plan gratuit generos | Până la 1200 records/tabel, 2GB storage |

---

## 📊 Tipuri de câmpuri (Fields)

Airtable are zeci de tipuri de câmpuri. Iată cele mai importante:

| Tip de câmp | Ce face |
|-------------|---------|
| **Single line text** | Texte scurte |
| **Long text** | Descrieri, note |
| **Number** | Numere cu validare |
| **Currency** | Lei, Euro, Dolari |
| **Date** | Calendar picker |
| **Attachment** | Fișiere, poze |
| **Checkbox** | Da/Nu |
| **Multiple select** | Etichete multiple |
| **Link to another record** | Relații între tabele |
| **Formula** | Calcule automate |
| **Rollup** | Agregă date din relații |
| **Lookup** | Afișează date din tabele legate |
| **Autonumber** | ID-uri automate |

---

## 🏗️ Proiect 1: CRM Simple pentru Freelancer

### Structură de tabele

**Tabel 1: Clienți**
| Câmp | Tip |
|------|-----|
| Nume | Single line text |
| Email | Email |
| Telefon | Phone |
| Companie | Single line text |
| Status | Single select (Potențial, Activ, Inactiv) |
| Note | Long text |
| Proiecte | Link to Proiecte |

**Tabel 2: Proiecte**
| Câmp | Tip |
|------|-----|
| Nume proiect | Single line text |
| Client | Link to Clienți |
| Status | Single select (Bugetare, În lucru, Finalizat, Facturat) |
| Buget | Currency |
| Deadline | Date |
| Descriere | Long text |

**Tabel 3: Facturi**
| Câmp | Tip |
|------|-----|
| Număr factură | Autonumber |
| Client | Link to Clienți |
| Proiect | Link to Proiecte |
| Sumă | Currency |
| Status | Single select (Proforma, Emisă, Plătită) |
| Data emitere | Date |
| Data scadență | Date |

---

## 📦 Proiect 2: Inventar E-commerce

### Tabel 1: Produse
| Câmp | Tip |
|------|-----|
| Nume | Single line text |
| SKU | Single line text |
| Categorie | Single select |
| Preț | Currency |
| Stoc | Number |
| Stoc minim | Number |
| Furnizor | Link to Furnizori |
| Status stoc | Formula |

**Formula pentru Status stoc:**
```
IF({Stoc} = 0, "Închis", IF({Stoc} < {Stoc minim}, "⚠️ Scăzut", "✅ OK"))
```

### Tabel 2: Furnizori
| Câmp | Tip |
|------|-----|
| Nume | Single line text |
| Contact | Single line text |
| Email | Email |
| Telefon | Phone |
| Timp livrare | Number (zile) |

---

## 📋 Proiect 3: Content Calendar

### Structură

**Tabel: Content Calendar**
| Câmp | Tip |
|------|-----|
| Titlu postare | Single line text |
| Platformă | Multi-select (Instagram, TikTok, Blog, YouTube) |
| Status | Single select (Idee, Scheduled, Live, Archived) |
| Dată publicare | Date |
| Categorie | Single select |
| Hashtags | Long text |
| Note | Long text |
| Materiale | Attachment |
| Link postare | URL |

### Grupare și filtrare

- **Group by Platformă** — vezi ce publici pe fiecare
- **Group by Status** — ce urmează, ce e gata
- **Calendar view** — vizualizare pe săptămâni/luni

---

## 🤖 Automatizări (Automations)

Airtable Automations sunt gratuite și extrem de utile:

### Exemple de automatizări

| Trigger | Acțiune |
|---------|---------|
| Când stoc < minim | Trimite email alertă |
| Când Status devine „Finalizat" | Creează task în Slack |
| Când se adaugă record nou | Trimite notificare |
| Când deadline se apropie | Adaugă reminder |

### Cum creezi o automatizare

1. Click pe **Automations** în meniu
2. Click **Create automation**
3. Alege **Trigger** (când se întâmplă ceva)
4. Adaugă **Actions** (ce să facă)
5. Activează și gata

---

## 📱 Airtable Apps (Blocks)

Blocks sunt aplicații în Airtable:

### Blocks populare

- **Chart** — grafice din datele tale
- **Map** — pentru adrese, locații
- **Timeline** — pentru proiecte
- **Pivot Table** — analiză avansată
- **Merge Records** — combină duplicate

---

## 🔗 Resurse

💻 **Instrumente:**
- [Airtable](https://airtable.com) — gratuit pentru început
- [Airtable Templates](https://airtable.com/templates) — șabloane gata făcute
- [Airtable Universe](https://airtable.com/universes) — exemple comunitate

📚 **Cărți (affiliate):**
- [The Personal MBA - Josh Kaufman](https://www.amazon.it) — fundamentals de business
- [Sprints - Jake Knapp](https://www.amazon.it) — cum să rezolvi probleme rapid

---

## 💛 Susține acest ghid

Dacă ți-a fost util, poți să susții proiectul:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru comunitatea românească*
