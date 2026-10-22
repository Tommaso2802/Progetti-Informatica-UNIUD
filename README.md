Progettazione completa di una base di dati per una rete di stazioni di servizio in FVG: dallo schema E-R all'implementazione in PostgreSQL con trigger, indici e query
# Base di dati per una rete di stazioni di servizio in Friuli Venezia Giulia

Progetto del corso di Basi di Dati – Laurea in Informatica, Università di Udine.

## Descrizione
Progettazione e implementazione di una base di dati per gestire una rete di
stazioni di servizio: aziende, stazioni, serbatoi e pompe, tipi di carburante,
personale con turni settimanali e consegne di carburante.

## Fasi del progetto
1. **Analisi dei requisiti**
2. **Progettazione concettuale**: schema E-R con 13 entità e 13 associazioni,
   una generalizzazione totale e disgiunta (Dipendente → Responsabile regionale /
   Addetto), entità deboli, vincoli di integrità e regole di derivazione
3. **Progettazione logica**: tavola dei volumi, analisi delle ridondanze,
   eliminazione delle generalizzazioni, schema relazionale
4. **Progettazione fisica**: scelta e giustificazione degli indici
5. **Implementazione** in PostgreSQL: creazione delle tabelle, trigger per i
   vincoli di integrità, query di interrogazione


## Tecnologie
PostgreSQL · SQL · LaTeX

## Struttura del repository
- `relazione/` – relazione completa del progetto (PDF e sorgente LaTeX)
- `sql/` – script di creazione, popolamento, trigger e query



Analisi sperimentale in Python di QuickSort, QuickSort 3-way, MergeSort e CountingSort: tempi misurati al variare della dimensione dell'input (n) e del dominio dei valori (m), confrontati con la complessità teorica.

 # Analisi empirica degli algoritmi di ordinamento

Progetto del corso di Algoritmi e Strutture Dati e Laboratorio – Laurea in Informatica,
Università di Udine (a.a. 2024/2025).
Autori: Tommaso Persello, Komla Achile Aziadzro.

## Obiettivo
Implementare quattro algoritmi di ordinamento su array di interi e misurarne
sperimentalmente le prestazioni al variare della dimensione dell'input (n) e
dell'intervallo dei valori (m), confrontando i risultati con la complessità teorica.

## Algoritmi implementati
| Algoritmo | Tipo | Complessità | Stabile | In-place |
|---|---|---|---|---|
| QuickSort | comparativo | Θ(n log n) medio, O(n²) peggiore | no | sì |
| QuickSort 3-way | comparativo | O(n log n) medio, ottimizzato per i duplicati | no | sì |
| MergeSort | comparativo | Θ(n log n) in ogni caso | sì | no |
| CountingSort | non comparativo | Θ(n + m) | sì | no |

