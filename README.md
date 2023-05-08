# LUDOPATIA A PADOVA

Questo progetto vuole verificare se la posizione dlle slot machine in provincia di Padova rispetta le norme della [LEGGE REGIONALE  n. 38 del 10 settembre 2019
](https://bur.regione.veneto.it/BurvServices/pubblica/DettaglioLegge.aspx?id=402726).  
Si specifica che la legge si applica alle nuove installazioni, per questo progetto invece utilizzeremo l'intero dataset di slotmachine per vedere quali sarebbero mal posizionate.

I parametri da seguire sono:

Per tutelare determinate categorie di soggetti maggiormente vulnerabili e per prevenire il disturbo da gioco d’azzardo, è vietata la collocazione di apparecchi per il gioco in locali che si trovino ad una distanza inferiore a quattrocento metri, calcolati sulla base del percorso pedonale più breve, da:

- servizi per la prima infanzia;
- istituti scolastici di ogni ordine e grado;
- centri di formazione per giovani e adulti;
- luoghi di culto;
- impianti sportivi;
- ospedali, strutture ambulatoriali, residenziali o semiresidenziali operanti in ambito sanitario o sociosanitario;
- residenze per anziani, strutture ricettive per categorie protette, luoghi di aggregazione socio-culturale, oratori e circoli da gioco per adulti;
- istituti di credito e sportelli bancomat;
- esercizi di compravendita di oggetti preziosi e di oro usati;
- stazioni ferroviarie e di autocorriere.

## DATI
- [Posizione delle slot](https://www.adm.gov.it/portale/monopoli/giochi/apparecchi_intr/elenco_soggetti_ries?pagina=3&id_pagina=2&el=2&form_elenco_soggetti_esercizi=1&prov=PD&comune=G224)
- [Compro Oro](https://infostat.bancaditalia.it/GIAVAInquiry-public/oro.html)
- [ATM Poste](https://www.poste.it/resources/editoriali/uffici_postali/altri/SportelloAmico%20_ElencoUP_02052012.xls)
- Posizione scuole, banche, ATM, [OpenStreetMap](www.openstreetmap.org) e filtro `"fclass" in ('atm','bank','hospital','kindergarten','nursing_home','playground','post_office','school','sports_centre','swimming_pool', 'theme_park','university')`

_______
