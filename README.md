# Validatore di Tag di Intestazione H1-H6 e Gerarchia Semantica

[![Validatore Tag Intestazione](https://img.shields.io/badge/TAVARDT-Heading%20Hierarchy-5b3cf5.svg)](https://tools.tavardt.com/it/validatore-tag-intestazione/)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)

Diagnosi dell architettura dei titoli HTML5, linearita della titolazione ed ergonomia per screen reader.

Sviluppato e gestito dalla divisione di architettura semantica web di **TAVARDT**.

***

## Funzionalita del Validatore di Intestazioni H1-H6

* **Univocita del Titolo H1**: Verifica della presenza di un solo tag `<h1>` cardine della pagina.
* **Rilevamento Salti di Livello**: Identificazione di interruzioni nell ordine gerarchico (es. passaggio diretto da `<h2>` a `<h4>`).
* **Controllo Intestazioni Vuote**: Individuazione di tag di titolo privi di testo descrittivo.
* **Mappatura dell Albero Semantico**: Visualizzazione gerarchica ad albero dell ossatura del documento HTML5.
* **Indice di Coerenza Semantica**: Punteggio tecnico da 0 a 100 conforme alle direttive AgID e W3C.

***

## Installazione ed Esecuzione

Richiede Python 3.8 o superiore senza dipendenze terze.

```bash
git clone https://github.com/TAVARDT-Italia/heading-hierarchy-validator-it.git
cd heading-hierarchy-validator-it
python heading_hierarchy_validator.py https://azienda.it
```

Emissione in formato strutturato JSON:

```bash
python heading_hierarchy_validator.py https://azienda.it -json
```

***

## Strumento Web Ufficiale

Esegui un controllo approfondito direttamente online:

* **Validatore di Tag di Intestazione Ufficiale**
* **[Portale Istituzionale TAVARDT](https://ag.tavardt.com/it/)**

***

## Consulenza e Supporto Tecnico

Per ottimizzare la struttura dei contenuti secondo Linee Guida AgID sull Accessibilita e Standard W3C, contatta **TAVARDT**.

***

© 2026 TAVARDT. Tutti i diritti riservati.
