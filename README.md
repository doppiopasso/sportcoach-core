# sportcoach-core

Motore di coaching **deterministic-first** multi-sport (corsa · ciclismo · triathlon · nuoto).
L'LLM interpreta e propone; il codice calcola, valida, simula e persiste.

[![CI](https://github.com/doppiopasso/sportcoach-core/actions/workflows/ci.yml/badge.svg)](...)
[![License: MIT](LICENSE)](LICENSE)

## Quickstart
```bash
pip install -r requirements.txt
python -m sportcoach validate --sport corsa --file esempio.json
```
## Architettura
- `athlete/` · `load/` · `periodization/` (ATR) · `validator/` · `simulator/` · `mcp_server/`
- `sports/{corsa,ciclismo,triathlon,nuoto}/` — adapter per sport (zone, pacing, schemi)
## Filosofia
Numeri mai inventati; parametri con stato epistemico; target verificati da feasibility gate;
dry-run di default. Vedi CODE GOVERNANCE.md.
## Licenze
MIT (software). I dataset terzi seguono le loro licenze (NOTICE inclusi). [Link prodotto → Gumroad]
