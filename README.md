# Infortuni nello sport – dataviz Radar QN

Tavola anatomica (davanti e dietro) con le parti del corpo più colpite dagli infortuni nel tennis professionistico e negli sport di squadra. Un'unica pagina con i pulsanti per cambiare sport; si apre sullo sport indicato nell'URL (`#tennis`, `#squadra`).

Indice con anteprime e codice per il CMS: https://cosimofire.github.io/infortuni-sport/

| Dataviz | URL |
|---|---|
| Parti del corpo, apre sul tennis | https://cosimofire.github.io/infortuni-sport/parti-corpo/#tennis |
| Parti del corpo, apre sugli sport di squadra | https://cosimofire.github.io/infortuni-sport/parti-corpo/#squadra |

## Dati (`data/infortuni.csv`)

Separatore `;`, virgola decimale. Una riga per area del corpo e sport: quota sul totale degli infortuni (%), eventuale intervallo (`quota_min_pct`, `quota_max_pct`), `approssimato` = `si` per i valori indicati come circa. Le righe senza quota (testa nel tennis, gomito negli sport di squadra) non vanno sulla figura e sono citate nelle note.

- Tennis: tennisti professionisti ATP, 2012-2016. Le aree mostrate coprono il 78,4% degli infortuni.
- Sport di squadra: rassegna di revisioni su basket, calcio, pallavolo, hockey su ghiaccio, rugby e pallamano. Ogni valore viene da uno sport o da un gruppo di studi diverso: le quote non si sommano e non sono confrontabili una per una con il tennis.

Fonte: Zupančič & Marušič (2024), Exercise and Quality of Life 16(1): 5-18, doi 10.31382/eqol.240601; Christianingsih et al. (2024). Elaborazione Radar – QN.

## Figure (`img/`)

WebP con sfondo trasparente, rigenerabili dagli originali con `script/prepara_immagini.py` (nella cartella del progetto, fuori dalla repo). Le coordinate delle zone in `parti-corpo/index.html` (oggetto `GEO`) dipendono da quei ritagli.
