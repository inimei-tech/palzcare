# PalzCare

> **Nachbarschaftshilfe aus der Pfalz — fair vergütet, lokal verankert.**

PalzCare verbindet Menschen mit Hilfebedarf mit fairen, **bezahlten** Helfer:innen in der Region Pfalz. Kein Ehrenamt. Keine anonyme Plattform. Echte Nachbarschaft.

---

## Was ist PalzCare?

Eine Matching-Plattform für Alltagshilfe in der Pfalz: Einkaufen, Haushalt, Gartenarbeit, Kinderbetreuung, Begleitung zu Terminen. Hilfesuchende finden verlässliche Unterstützung — Helfende verdienen fair für ihre Zeit.

**Abgrenzung:**
- Kein HILVER/SAM (dort: rein ehrenamtlich)
- Kein nebenan.de (dort: allgemeiner Marktplatz, kein Fokus auf Hilfe)
- PalzCare: spezialisiert, bezahlt, verifiziert, regional

---

## Status

**Pre-Launch / Validierungsphase**

- Live-Website: [palzcare.de](https://palzcare.de)
- App-Prototype: [palzcare.de/app](https://palzcare.de/app) ← HTML-Prototype, läuft als Custom HTML Block in WordPress
- Pool-Registrierung: [palzcare.de/jetzt-eintragen](https://palzcare.de/jetzt-eintragen)
- Umfrage: [palzcare.de/umfrage](https://palzcare.de/umfrage)

Matching läuft aktuell **manuell** via WhatsApp — die technische Plattform wird parallel aufgebaut.

---

## Zielgruppen

### Phase 1 — Mütter (aktiv)
Junge Mütter als Hilfesuchende + Helfende (Studierende, Teilzeitsuchende, Rentner:innen). Digital-affin, erreichbar über WhatsApp, Instagram, QR-Codes, Kita/Schule-Netzwerke.

### Phase 2 — Senior:innen (geplant)
Ältere Menschen mit Unterstützungsbedarf. Erfordert andere Kanäle (Amtsblatt, Direktansprache, Flyer mit Rücksendeumschlag) — wird gestartet, sobald Phase 1 etabliert ist.

---

## Tech Stack

| Bereich | Tool |
|---|---|
| Website | WordPress (Blocksy Theme + Kadence Blocks) |
| App-Prototype | Vanilla HTML/CSS/JS (Single File) |
| Formulare | CryptPad (End-to-End verschlüsselt) |
| Datenbank/CRM | Notion (aktuell, mit DSGVO-Einschränkungen bekannt) |
| Chatbot | Botpress (floating button auf Homepage) |
| Automatisierung | n8n (geplant) |
| App-Entwicklung | Cursor AI (geplant) |
| CI/CD | GitHub (dieses Repository) |
| Kontakt | palzcare@proton.me |

**Geplanter Stack (Custom App):**
- Frontend: React (via Cursor AI)
- Backend: Node.js
- Datenbank: Supabase (PostgreSQL, DSGVO-konform)
- Hosting: app.palzcare.de

---

## Sicherheitskonzept

PalzCare bringt Fremde zu vulnerablen Menschen — Sicherheit ist nicht optional:

1. SMS-Verifikation (in Deutschland ID-verknüpft)
2. Erweitertes Führungszeugnis
3. Bidirektionales Bewertungssystem
4. Geplant: Video-Interview, Premium-Zertifizierung

---

## Brand

| Element | Wert |
|---|---|
| Primärfarbe | Bordeaux `#9B2556` |
| Akzentfarbe | Mint/Türkis `#5BBFB5` |
| Neutralfarbe | Anthrazit `#2D2D2D` |
| Fonts | Lora (Serif) + Source Sans 3 |
| Tonalität | Warm, vertrauensvoll, regional |
| Nutzer-Ansprache | Sie (formell) |
| Gründerin-Stimme | "Ich" (Soloprojekt — kein "Wir") |

---

## Repository-Struktur

```
palzcare/
├── app/
│   └── index.html          # HTML-Prototype (läuft unter palzcare.de/app)
├── docs/
│   ├── ARCHITECTURE.md     # Technische Architektur & Roadmap
│   ├── PRIVACY.md          # DSGVO-Konzept & Datenschutz
│   └── MATCHING.md         # Matching-Logik (manuell → automatisch)
├── assets/
│   └── logo.png
├── .env.example
├── CONTRIBUTING.md
└── README.md
```

---

## Datenschutz / DSGVO

- Formulare: CryptPad (End-to-End verschlüsselt — auch der Betreiber hat keinen Zugriff)
- Kontakt: Proton Mail (verschlüsselt)
- Notion als temporärer Datenspeicher (AVV vorhanden, kein E2E)
- Ziel: vollständige Migration auf selbstgehostete Infrastruktur mit dem Custom App Build

---

## Gründerin

**Gülsen Kitzel (Gülli)** — Sologründerin, Mutter, Musikerin aus Maxdorf, Pfalz.

Weitere Projekte: [Inimei Tech](https://inimei01.com) · PFALZ | WEBSITES®

---

## Mitmachen / Contributing

Dieses Projekt ist ein Soloprojekt in der Frühphase. Developer-Recruiting läuft.

Interesse? → palzcare@proton.me

Detaillierte Guidelines: [CONTRIBUTING.md](./CONTRIBUTING.md)

---

## Lizenz

Alle Rechte vorbehalten — © 2026 Gülsen Kitzel / PalzCare
