
# 🕹️ MCINV – Retro Price Calculator

## Descrizione

**MCINV** è una Progressive Web App (PWA) retro-futurista ispirata al Commodore 64.  
Rielaborazione completa della mia **storica calcolatrice di margini e sconti**, scritta in BASIC nel 1983, ora trasformata in un'app moderna e installabile.

Minimal. Precisa. Estetica 8-bit.

---

## Funzionalità

1. **Calcolo Prezzo Netto:**
   - Inserisci un **prezzo lordo**
   - Applica uno **sconto (%)**
   - Aggiungi un **margine (%)**
   - Calcola automaticamente il **prezzo netto finale**

2. **Calcolo Inverso (con margine):**
   - Inserisci un **prezzo netto desiderato**
   - L'app calcola lo **sconto necessario** per raggiungerlo partendo dal prezzo lordo

3. **Calcolo Inverso Diretto (senza margine):**
   - Inserisci il netto atteso
   - Ottieni lo **sconto diretto (%)** da applicare

---

## Modalità d'Uso

- Compila i campi richiesti
- Clicca su **RUN**
- Il risultato viene mostrato subito in stile `>>>` terminale C64

---

## Stile Retro

- Font monospace, sfondo blu C64 (`#0400A0`)
- Colori pixelati: verde brillante su sfondo blu
- Nessuna interfaccia moderna, nessun tema dark: solo essenziale

---

## Codice originale (Commodore 64 – BASIC, 1983)

```basic
10 PRINT "CALCOLATRICE IN C64 BASIC"
20 INPUT "PREZZO LORDO";P
30 INPUT "SCONTO (%)";S
40 INPUT "MARGINE (%)";M
50 S1 = P * (1 - S / 100)
60 NETTO = S1 / (1 - M / 100)
70 PRINT ">>> NETTO: ";NETTO
80 INPUT "PREZZO NETTO DESIDERATO";D
90 DS = (1 - ((D * (1 - M / 100)) / P)) * 100
100 PRINT ">>> SCONTO NECESSARIO: ";DS;"%"

🧠 Bastavano 10 righe. Nessuna dipendenza. Solo logica.

⸻

Tecnologie Usate
	•	HTML + CSS + JS
	•	Compatibile con tutti i browser moderni
	•	Funzionamento offline via service-worker.js
	•	Installabile su iPhone, Android e desktop (PWA)

⸻

Dove provarla

🔗 Versione live:
👉 www.alessandropezzali.it/MCINV/

📁 Codice sorgente:
👉 github.com/pezzaliapp/MCINV

⸻

Autore

Realizzata da
Alessandro Pezzali
📦 pezzaliAPP.com | ☕ patreon.com/pezzaliAPP

⸻

Licenza

MIT – Libera per uso personale e professionale.
Distribuibile, retro-compatibile, nostalgica.
