# Skill: Meta Autonomous Ad Agent

## Core Philosophy
"From Data to Live Ads in one evening."
Cel: Zastąpienie ręcznej pracy w Ads Managerze autonomicznym agentem, który operuje na API, analizuje dane i wdraża kreacje w trybie `PAUSED` (Human-in-the-Loop).

## Workflow (The Kamil Loop)
1. **Audit & Intelligence (API Pull):**
   - Pobranie danych z Meta Ads API (ROAS per kreacja, CTR, CPA).
   - Analiza "zabójców budżetu" i "winnerów".
   - Output: Tabela z rekomendacjami (Co wyłączyć, co skalować).
2. **Creative Generation (The Mix):**
   - **Real Assets:** Pobranie zdjęć produktu z WooCommerce/Medusa.js lub folderu `assets/`.
   - **Social Proof:** Scraping opinii z TrustMate/Google Reviews.
   - **Generative AI:** Użycie NanoBanana/Kie.ai do połączenia realnych zdjęć z wygenerowanym tłem/tekstami (img2img).
3. **Copywriting & Angles:**
   - Generowanie 5 wariantów tekstów dopasowanych do najlepszych kątów (hooks).
4. **Deployment (Meta Graph API):**
   - Tworzenie reklam statycznych i karuzel w formatach 1:1, 9:16, 16:9.
   - Wrzucanie wszystkiego jako `PAUSED`.
   - Raport finalny dla człowieka do akceptacji.

## Tech Stack & Integrations
- **Meta Graph API:** Do odczytu wyników i wgrywania kreacji.
- **NanoBanana / Kie.ai API:** Do najtańszej i najszybszej generacji grafik.
- **WooCommerce/Medusa API:** Źródło prawdziwych zdjęć produktów.
- **GitHub (Assets):** Repozytorium na "bazę wiedzy" (logi z audytów, szablony kreacji).

## Rules
- **Safety First:** Nigdy nie aktywuj reklam automatycznie. Zawsze status `PAUSED`.
- **Data-Driven:** Każda decyzja o stworzeniu nowej kreacji musi wynikać z danych (np. "ta grafika miała wysoki CTR, zrób jej variantes").
- **Asset Pipeline:** Unikaj "stockowych" looków. Bazuj na realnych fotkach z realizacji/produktu.
