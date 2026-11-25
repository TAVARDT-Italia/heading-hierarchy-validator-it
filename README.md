# Validatore di Tag di Intestazione H1-H6 e Gerarchia Semantica

[![Validatore Tag Intestazione](https://img.shields.io/badge/TAVARDT-Heading%20Hierarchy-5b3cf5.svg)](https://tools.tavardt.com/it/validatore-tag-intestazione/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Audit dei tag di intestazione HTML5 (H1-H6), unicita di H1, rilevamento dei salti di livello e verifica della struttura semantica.

***

## Vettori di Rischio e Impatto Operativo nella Gerarchia dei Titoli

L assenza o la duplicazione dei tag H1 indebolisce la rilevanza tematica rilevata dai motori di ricerca in Italia. Una titolazione confusa ostacola gli screen reader e riduce l accessibilita complessiva del sito.

Saltare livelli logici nella successione delle intestazioni contravviene alle linee guida internazionali W3C WCAG. I titoli vuoti creano riferimenti fantasma che penalizzano il punteggio di qualita tecnica del documento.

***

## Funzionalita Centrali di Audit Tecnico

* **Verifica del Tag H1 Principale**: Accerta la presenza e l unicita del titolo primario, deducendo 40 punti se assente e 15 per tag H1 multipli.
* **Rilevamento dei Salti di Livello**: Traccia la sequenza dei titoli individuando salti strutturali impropri con penalita fino a 30 punti.
* **Identificazione di Intestazioni Vuote**: Rileva tag di titolo privi di testo significativo, applicando fino a 20 punti di detrazione.
* **Rappresentazione Strutturale Completa**: Costruisce la mappa gerarchica da H1 ad H6 calcolando la ripartizione degli elementi.
* **Punteggio di Conformita Semantica**: Assegna una valutazione tecnica da 0 a 100 categorizzata in SATISFACTORY, ADVISORY o UNSATISFACTORY.
* **Garanzia di Accessibilita per Screen Reader**: Verifica che i riferimenti testuali soddisfino i criteri di accessibilita e fruibilita assistita.
* **Esportazione Dati in Formato JSON**: Supporta la generazione di dati strutturati per l inserimento in pipeline di integrazione continua.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore senza dipendenze esterne aggiuntive.

```bash
git clone https://github.com/TAVARDT-Italia/heading-hierarchy-validator-it.git
cd heading-hierarchy-validator-it
python heading_hierarchy_validator.py https://azienda.it
```

Per generare l output in formato strutturato JSON per pipeline di integrazione continua:

```bash
python heading_hierarchy_validator.py https://azienda.it -j
```

***

## Domande Frequenti (FAQ Tecnico)

### 1. Come incidono l assenza o la presenza di piu tag H1 sul posizionamento nei motori?
I motori di ricerca considerano il tag H1 il punto di riferimento semantico primario per determinare il tema centrale della pagina. L assenza di H1 crea incertezza tematica, mentre piu tag H1 frammentano la concentrazione delle parole chiave fondamentali.

### 2. Per quale motivo saltare livelli di intestazione viola le linee guida sull accessibilita?
Le tecnologie assistive analizzano i tag di intestazione per creare un sommario vocale di orientamento per gli utenti non vedenti. Omettere livelli intermedi crea salti ingiustificati che ostacolano la comprensione e violano gli standard W3C WCAG.

### 3. Quali problemi generano le intestazioni vuote all interno del codice HTML?
I tag di intestazione privi di testo inseriscono riferimenti vuoti che confondono gli screen reader e degradano la valutazione tecnica del sito. I motori di ricerca interpretano questi elementi come difetti di sviluppo, riducendo il punteggio di qualita della pagina.

### 4. In che misura una titolazione ordinata agevola le risposte fornite dai motori basati su IA?
I sistemi di intelligenza artificiale esaminano le pagine in blocchi logici per estrarre informazioni puntuali ed elaborare risposte. Un percorso ordinato da H1 ad H6 permette agli algoritmi di isolare e citare con esattezza le sezioni di rilievo.

### 5. Qual e la sequenza tecnica corretta per suddividere i contenuti di un portale articolato?
Ogni pagina deve contenere un solo H1 descrittivo, seguito da intestazioni H2 che delineano i moduli principali. Le suddivisioni interne devono proseguire ordinatamente con H3 ed H4 senza salti, preservando la continuita logica del documento.

***

## Consulenza in Architettura Semantica e Accessibilita

Per grandi architetture digitali che richiedono la piena conformita a W3C WCAG e standard Google, consultate il team di **TAVARDT**.

***

## Collegamenti Utili

* **Portale Istituzionale:** https://ag.tavardt.com/it/
* **Suite di Diagnostica:** https://tools.tavardt.com/it/
* **Contatto Tecnico:** https://ag.tavardt.com/it/contatto/

***

### Licenza
Distribuito sotto Licenza MIT. Consultare il file LICENSE per i dettagli completi.

***

© 2026 TAVARDT. Tutti i diritti riservati.
