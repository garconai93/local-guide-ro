---
title: "Ghid Notion Baze de Date: CRM personal, tracker financiar și inventar"
date: 2026-04-01
draft: false
description: "Ghid avansat Notion pentru baze de date. Învață să creezi CRM personal, tracker de cheltuieli, inventar și alte sisteme de organizare puternice."
keywords: ["Notion", "baze de date", "CRM personal", "tracker financiar", "Notion database", "organizare"]
image: "notion-database.jpg"
tags: ["Notion", "Baze de Date", "CRM", "Tutorial Avansat"]
readingTime: "13 min"
---

# 🗃️ Ghid Notion Baze de Date: CRM personal, tracker financiar și inventar

Bazele de date din Notion sunt ceea ce diferențiază Notion de o simplă aplicație de note. Cu ele poți crea sisteme complexe de organizare — de la CRM personal la tracker de cheltuieli. Acest ghid te învață cum să le stăpânești.

---

## 🔑 Ce sunt Bazele de Date în Notion?

O **bază de date** în Notion este o colecție de **intrări** (rows) cu **proprietăți** (columns) pe care le poți vizualiza în mai multe moduri:

| Vizualizare | Folosește când |
|-------------|----------------|
| **Table** | Date structurate, sortable, filtrabile |
| **Board** (Kanban) | Task-uri cu status |
| **Gallery** | Carduri vizuale (clienți, produse) |
| **Calendar** | Date limită, deadline-uri |
| **List** | Liste simple |
| **Timeline** | Proiecte pe perioade lungi |

---

## 📊 CRM Personal — Gestionarea Relațiilor

### Structura bazei de date

Creează o bază de date **Gallery** sau **Table** numită „Contacte":

| Proprietate | Tip | Descriere |
|-------------|-----|-----------|
| Nume | Text | Numele persoanei |
| Email | Email | Adresa de email |
| Telefon | Telefon | Număr de telefon |
| Categorie | Select | Client / Furnizor / Prieten / Potențial |
| Ultimul contact | Date | Când ai vorbit ultima dată |
| Valoare | Număr | Valoare potențială (B2B) |
| Notițe | Text lung | Detalii despre conversații |
| Tag-uri | Multi-select | Interese, industry, sursă |

### Relații între baze

Poți lega baza „Contacte" de alte baze:

```
Contacte ← → Întâlniri (cine a participat)
Contacte ← → Task-uri (ce ai de făcut cu el)
Contacte ← → Note (convorbiri, întâlniri)
```

### Formula utilă: Zile de la ultimul contact

```
dateBetween(prop("Astăzi"), prop("Ultimul contact"), "days")
```

Adaugă o coloană „Zile de inactivitate" care îți spune automat când trebuie să reiei legătura.

---

## 💰 Tracker de Cheltuieli în Notion

### Baza de date „Tranzacții"

| Proprietate | Tip |
|------------|-----|
| Data | Date |
| Sumă | Număr (format: Lei) |
| Categorie | Select (Mâncare, Transport, Entertainment...) |
| Subcategorie | Select |
| Cont | Select (Cash, Card, Revolut...) |
| Descriere | Text |
| Recurent | Checkbox |
| Etichete | Multi-select |

### Vizualizări utile

1. **Table** — toate tranzacțiile, sortate pe dată
2. **Group by Categorie** — cât cheltuiești pe fiecare categorie
3. **Calendar** — vizualizare pe lună
4. **Sumar** — folosește formula pentru totaluri

### Formula: Total pe categorie

```
sum(prop("Sumă"), prop("Categorie") = "Mâncare")
```

Sau creează o pagină separată de **dashboard** cu grafice:

```markdown
## Sumar [Luna curentă]

🍔 Mâncare: {{sum filtered by category "Mâncare"}}
🚗 Transport: {{sum filtered by category "Transport"}}
🎬 Entertainment: {{sum filtered by category "Entertainment"}}

Total: {{grand total}}
```

---

## 📦 Sistem de Inventar

### Baza de date „Produse"

| Proprietate | Tip |
|------------|-----|
| Nume produs | Text |
| Cod SKU | Text |
| Categorie | Select |
| Cantitate | Număr |
| Preț achiziție | Număr |
| Preț vânzare | Număr |
| Locatie | Select (Magazie, Raft, etc.) |
| Furnizor | Relation → Contacte |
| Stoc minim | Număr |
| Status | Select (În stoc, Stoc scăzut, Comandă) |
| Data ultimei intrări | Date |

### Formula: Status automat

```
if(prop("Cantitate") = 0, "Închis", 
if(prop("Cantitate") < prop("Stoc minim"), "⚠️ Stoc scăzut", "✅ OK"))
```

### Relații

```
Produse → Intrări (istoric achiziții)
Produse → Ieșiri (vânzări/livrări)
Produse → Comenzi (ce urmează să vină)
```

---

## 📅 Calendar și Timeline

### Calendar de sarcini

Creează o bază de date cu:
- Task (text)
- Dată limită (date)
- Prioritate (select: p1-p4)
- Categorie (select)
- Status (select: Todo, In Progress, Done)

### Timeline pentru proiecte

Folosește vizualizarea **Timeline** pentru a vedea:
- Durata fiecărei faze
- Overlap-uri
- Deadline-uri critice

---

## 🔗 Resurse

💻 **Instrumente:**
- [Notion](https://www.notion.so) — gratuit pentru uz personal
- [Notion API](https://developers.notion.com) — automatizări avansate
- [Notion Templates](https://www.notion.so/templates) — șabloane gratuite

📚 **Cărți (affiliate):**
- [The Data Detective - Tim Harford](https://www.amazon.it) — date și insight-uri
- [Numsense! - L. A. & K. Yeo](https://www.amazon.it) — data science pentru non-tehnici

---

## 💛 Susține acest ghid

Dacă ți-a fost util, poți să susții proiectul:

- 💛 [Donează pe Ko-fi](https://ko-fi.com/garconai93)
- 📦 [Cumpără de pe Amazon prin link-ul nostru](https://www.amazon.it) — ne ajuți fără costuri în plus

---

*Creat cu ❤️ pentru comunitatea românească*
