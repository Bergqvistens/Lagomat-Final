# Lagomat

Din personliga matguide för glutenfri och laktosfri matlagning.

**Live:** https://bergqvistens.github.io/Lagomat/

---

## Innehåll

| Fil | Beskrivning |
|---|---|
| `index.html` | Hela appen — startflöde, recept, Matskolan |
| `integritetspolicy.html` | Integritetspolicy (GDPR) |
| `logga.png` | Lagomat-logga, används i splashskärmen |
| `ikon-1-hand.png` | Introduktionssida 1 |
| `ikon-2-vag.png` | Introduktionssida 2 |
| `ikon-3-kalender.png` | Introduktionssida 3 |
| `CNAME` | Kopplar repot till lagomat.se |

Alla filer ligger i roten — inga undermappar.

---

## Funktioner

- **Onboarding** — splash, tre introduktionssidor, GDPR-korrekt cookie-samtycke
- **Personligt näringsbehov** — beräknas med Mifflin-St Jeor utifrån kön, ålder, vikt, längd, aktivitetsnivå och mål
- **30 recept** — 10 frukost, 10 lunch, 10 middag, samtliga glutenfria och laktosfria
- **Veckoplanering** — slumpa eller välj måltider, generera inköpslista
- **Matskolan** — brödguide, sockerskola, allergener, handmått, proteinguide
- **Streckkodsskanner** — produktuppslag via Open Food Facts
- **Loggning** — protein och kalorier per dag med historik

---

## Teknik

Byggd som en enda fristående HTML-fil. Inget byggsteg, ingen server, inga beroenden att installera.

- React 18 (UMD) + Babel standalone
- All data i `localStorage` — inget lämnar enheten
- Mobilanpassad, utvecklad och testad på Samsung Galaxy S24

---

## Utveckling

Öppna `index.html` i en webbläsare. Det är hela arbetsflödet.

**localStorage-nycklar:**

| Nyckel | Innehåll |
|---|---|
| `lagomat-profil` | Namn, kön, ålder, vikt, längd, aktivitet, mål |
| `lagomat_intro_klar` | Om introduktionen är genomgången |
| `lagomat_cookies_accepted` | Cookie-samtycke (true/false) |
| `lagomat_cookies_datum` | Tidsstämpel för samtycket |

Introduktionen kan visas igen via knappen längst ned i Info-fliken.

---

## Licens

© 2026 Bergqvistens. Alla rättigheter förbehållna.
