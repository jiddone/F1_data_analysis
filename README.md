# 🏁 F1 Data Analysis – Stagione 2024

Questo notebook effettua un'analisi dati della **stagione di Formula 1 2024** con due livelli di approfondimento.  
Prima si analizza l’intera stagione, includendo gare e sessioni di qualifiche.  
Poi si effettua un'analisi mirata e approfondita delle **qualifiche del Gran Premio di Montecarlo**.

---

## 📘 Introduzione

`f1-data-analysis.ipynb` contiene esplorazioni, trasformazioni e visualizzazioni create per rispondere a domande operative sulle prestazioni stagionali.  
L'approccio è data-driven. Le analisi cercano pattern su risultati, consistenza e impatto delle variabili temporali e di sessione.

---

## ⚙️ Caricamento e gestione dei dati

- Lettura dei dataset con `pandas`.  
- Uso di `pathlib.Path` per gestire i percorsi dei file.  
- Impostazioni di visualizzazione per ispezione completa dei dataframe.  
- Funzioni helper per mappare identificatori (es. driverId) ai nomi completi.  
- Importazione esplicita dei dati relativi a: risultati di gara, risultati qualifiche, tempi di settore se presenti, informazioni su piloti e team, metadati di sessione (es. condizioni atmosferiche, temperatura).

---

## 🧹 Preprocessing

- Normalizzazione e pulizia dei nomi di piloti e scuderie.  
- Gestione dei valori mancanti e rimozione di duplicati.  
- Allineamento e merge tra tabelle gare, qualifiche e anagrafica piloti/team.  
- Creazione di colonne derivate utili all’analisi: posizione normalizzata, gap temporali, punti per gara, medie e deviazioni dei tempi di qualifica.  
- Verifica di coerenza temporale tra sessioni (qualifiche vs gara).

---

## 🔎 Analisi stagionale: gare e qualifiche

- Statistiche riassuntive per l’intera stagione.  
  - Punti totali, podi, vittorie per pilota e per team.  
  - Distribuzione delle posizioni di arrivo.  
- Analisi comparata tra sessioni: qualifiche vs gara.  
  - Differenze tra posizione in griglia e posizione a fine gara.  
  - Frequency di sorpassi netti (posizioni guadagnate/perse tra qualifica e arrivo).  
- Metriche di consistenza.  
  - Posizione media e deviazione standard per pilota/team.  
  - Percentuale di arrivi nei punti.  
- Analisi temporale e trend.  
  - Evoluzione delle prestazioni nel corso della stagione.  
  - Eventuali cambi di rendimento correlati a circuiti o condizioni (se i dati lo permettono).

---

## 🏎️ Analisi dettagliata: Qualifiche – Gran Premio di Montecarlo

- Estrazione e isolamento della sessione di qualifiche di Montecarlo.  
- Valutazione dei tempi di qualifica.  
  - Classifica dei migliori tempi.  
  - Gap tra i piloti e analisi degli outlier.  
- Analisi settore-per-settore quando disponibili.  
  - Identificazione dei piloti più performanti per settore.  
  - Confronto tra best sector e tempo complessivo.  
- Analisi dei fattori di variabilità.  
  - Impatto di traffico, bandiere gialle o condizioni meteo sulla distribuzione dei tempi.  
- Breakdown delle strategie di tentativo in qualifica.  
  - Numero di tentativi per pilota.  
  - Success rate dei tentativi migliori.  
- Visualizzazioni specifiche per Montecarlo.  
  - Scatter plot tempi vs tentativi.  
  - Heatmap o plot settore-per-settore per evidenziare punti di guadagno/ perdita.

---

## 📊 Visualizzazioni incluse nel notebook

- Tabelle riassuntive e pivot per pilota e team.  
- Grafici a linee per trend stagionali.  
- Boxplot e violin plot per distribuzioni di tempi e posizioni.  
- Scatter plot e grafici a barre per confronti diretti.  
- Visualizzazioni dedicate per la qualifica di Montecarlo (tempi, gap, settori).  

Le figure sono accompagnate da brevi commenti interpretativi. I grafici sono progettati per essere riprodotti e adattati facilmente.

---

## 🧾 Risultati principali (sintesi)

- Sintesi delle performance stagionali per pilota e team.  
- Differenze osservate tra posizione in griglia e risultato di gara.  
- Indicatori di consistenza e vulnerabilità stagionale.  
- Insight specifici sulla qualifica di Montecarlo: pattern di gap, settori critici, variabilità dovuta a eventi di sessione.

---

## 👨‍💻 Autore

📬 Contatti
Per domande o suggerimenti:

Gianluca Ferrari
📧 Email: gianlucaferrari2000@gmail.com
