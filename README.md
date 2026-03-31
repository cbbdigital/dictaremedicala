# Dictare Medicală

Aplicație web de dictare vocală cu transcriere în limba română, optimizată pentru terminologie medicală (radiologie).

## Features

- 🎙️ Înregistrare vocală cu transcriere în timp real (Web Speech API, ro-RO)
- 📊 Vizualizare waveform live din microfon
- 🔢 Conversie automată numere românești → cifre ("șaptesprezece pe doi" → "17/2")
- 💾 Salvare înregistrări în Supabase (persistență 30 zile)
- 📋 Copiere rapidă text
- ⏸️ Pauză / Continuare / Stop

## Tech Stack

- **Frontend**: HTML/CSS/JS vanilla (zero dependencies, single file)
- **Font**: Outfit + DM Mono
- **Backend**: Supabase (PostgreSQL + Auth + RLS)
- **Hosting**: Netlify
- **Speech**: Web Speech API (Chrome recommended)

## Setup

1. Clone repo
2. Push to GitHub
3. Connect to Netlify (auto-deploy)
4. Supabase project already configured

## Supabase

- Project: `Dictare Medicală` (eu-central-1)
- Table: `recordings` (id, user_id, text, duration, created_at)
- Auth: Anonymous auto-signup
- RLS: Users can only access their own recordings
