# Technische Architektur & Roadmap

## Aktueller Zustand (Prototype)

```
palzcare.de (WordPress)
├── Homepage
├── /jetzt-eintragen  → CryptPad Pool-Formular (embed)
├── /umfrage          → CryptPad Umfrage-Formular (embed)
└── /app              → HTML-Prototype (Single File, Custom HTML Block)
```

Matching: vollständig manuell via WhatsApp  
Daten: CryptPad (E2E verschlüsselt) → manueller Export → Notion

---

## Zielarchitektur (Custom App)

```
app.palzcare.de
├── Frontend (React, Mobile-first)
│   ├── Registrierung / Login
│   ├── Profil (Helfer / Hilfesuchende)
│   ├── Hilfegesuch aufgeben
│   ├── Helfer finden (Standort + Kategorie)
│   ├── Matching & Anfragen
│   └── Bewertungssystem
└── Backend (Node.js)
    ├── Auth (SMS-Verifikation)
    ├── Matching-Logik
    ├── Benachrichtigungen (Push)
    └── API

Datenbank: Supabase (PostgreSQL, EU-Hosting, DSGVO)
```

---

## Roadmap

### Phase 1 — Validierung (aktiv)
- Pool füllen via CryptPad-Formulare
- Manuelles Matching via WhatsApp
- Prototype unter palzcare.de/app live

### Phase 2 — Custom App (geplant, Cursor AI)
- Authentifizierung (SMS)
- Nutzerprofile (Helfer / Hilfesuchende)
- Hilfegesuch + Matching
- In-App Messaging
- Benachrichtigungen

### Phase 3 — Skalierung
- Erweitertes Führungszeugnis-Workflow
- Zahlungsintegration (Stripe)
- Bewertungssystem (bidirektional)
- Senior:innen-Phase (Phase 2 Zielgruppe)

---

## Sicherheitskonzept

Stufe 1: SMS-Verifikation (DE: ID-verknüpft)  
Stufe 2: Erweitertes Führungszeugnis (Upload + Verifikation)  
Stufe 3: Bewertungen (bidirektional, nach jedem Einsatz)  
Geplant: Video-Interview für Premium-Helfer:innen

---

## DSGVO-Anforderungen

- Kein US-Cloud-Provider für personenbezogene Daten
- E2E-Verschlüsselung für Formulare (CryptPad) und Kommunikation (Proton Mail)
- AVV mit allen Drittanbietern
- Recht auf Löschung implementiert
- Keine Weitergabe an Dritte
