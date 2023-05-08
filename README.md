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
- [Luoghi di culto](www.openstreetmap.org)
- [Stazioni ferroviarie e corriere](www.openstreetmap.org) filtro `"fclass" in('bus_station','railway_station')`
- [Dati geografici](https://idt2.regione.veneto.it/) 
- [Popolazione](http://dati.istat.it/Index.aspx?QueryId=18549)

Per una dettagliata spiegazione dei TAG di OSM riferirsi alla [documentazione](https://wiki.openstreetmap.org/wiki/Main_Page)

_______

## RISULTATI

**Mappa di inquadramento**

![mappa1](https://github.com/fgianoli/ludopatia/blob/main/img/mappa_1.jpg)

**Densità di slot/abitanti**

![Slot per abitante](https://github.com/fgianoli/ludopatia/blob/main/img/slot_hab.jpg)

**Densità di slot non a norma/abitanti**

![Slot non a norma per abitante](https://github.com/fgianoli/ludopatia/blob/main/img/slotNo_hab.jpg)


______

## Dati tabulari


| Codistat | Nomcom                        | Provincia | N_slot | Slot_No | Comune                            | M     | F      | TOT    |
|:--------:|:-----------------------------:|:---------:|:------:|:-------:|:---------------------------------:|:-----:|:------:|:------:|
| 28001    | Abano Terme                   | PD        | 21     | 22      |     Abano Terme                   | 9653  | 10578  | 20231  |
| 28002    | Agna                          | PD        | 3      | 3       |     Agna                          | 1554  | 1603   | 3157   |
| 28003    | Albignasego                   | PD        | 42     | 20      |     Albignasego                   | 13055 | 13835  | 26890  |
| 28004    | Anguillara Veneta             | PD        | 1      | 5       |     Anguillara Veneta             | 2037  | 2087   | 4124   |
| 28005    | Arqua' Petrarca               | PD        | 5      | 0       |     Arquà Petrarca                | 900   | 910    | 1810   |
| 28006    | Arre                          | PD        | 4      | 2       |     Arre                          | 1053  | 1038   | 2091   |
| 28007    | Arzergrande                   | PD        | 5      | 6       |     Arzergrande                   | 2366  | 2422   | 4788   |
| 28008    | Bagnoli Di Sopra              | PD        | 6      | 2       |     Bagnoli Di Sopra              | 1700  | 1696   | 3396   |
| 28009    | Baone                         | PD        | 9      | 1       |     Baone                         | 1545  | 1513   | 3058   |
| 28010    | Barbona                       | PD        | 3      |         |     Barbona                       | 300   | 285    | 585    |
| 28011    | Battaglia Terme               | PD        | 12     | 6       |     Battaglia Terme               | 1847  | 1919   | 3766   |
| 28012    | Boara Pisani                  | PD        | 2      | 6       |     Boara Pisani                  | 1195  | 1184   | 2379   |
| 28107    | Borgo Veneto                  | PD        | 21     | 8       |     Borgo Veneto                  | 3535  | 3481   | 7016   |
| 28013    | Borgoricco                    | PD        | 8      | 8       |     Borgoricco                    | 4509  | 4460   | 8969   |
| 28014    | Bovolenta                     | PD        | 6      | 2       |     Bovolenta                     | 1722  | 1718   | 3440   |
| 28015    | Brugine                       | PD        | 8      | 10      |     Brugine                       | 3526  | 3634   | 7160   |
| 28016    | Cadoneghe                     | PD        | 5      | 13      |     Cadoneghe                     | 7643  | 8158   | 15801  |
| 28020    | Campo San Martino             | PD        | 6      | 6       |     Campo San Martino             | 2825  | 2780   | 5605   |
| 28017    | Campodarsego                  | PD        | 15     | 15      |     Campodarsego                  | 7455  | 7617   | 15072  |
| 28018    | Campodoro                     | PD        | 4      | 1       |     Campodoro                     | 1311  | 1296   | 2607   |
| 28019    | Camposampiero                 | PD        | 20     | 6       |     Camposampiero                 | 5866  | 5951   | 11817  |
| 28021    | Candiana                      | PD        | 4      | 1       |     Candiana                      | 1127  | 1065   | 2192   |
| 28022    | Carceri                       | PD        | 3      | 1       |     Carceri                       | 731   | 739    | 1470   |
| 28023    | Carmignano Di Brenta          | PD        | 11     | 3       |     Carmignano Di Brenta          | 3723  | 3660   | 7383   |
| 28026    | Cartura                       | PD        | 8      | 5       |     Cartura                       | 2258  | 2309   | 4567   |
| 28027    | Casale Di Scodosia            | PD        | 4      | 5       |     Casale Di Scodosia            | 2331  | 2316   | 4647   |
| 28028    | Casalserugo                   | PD        | 4      | 3       |     Casalserugo                   | 2659  | 2707   | 5366   |
| 28029    | Castelbaldo                   | PD        | 4      | 1       |     Castelbaldo                   | 702   | 718    | 1420   |
| 28030    | Cervarese Santa Croce         | PD        | 10     | 3       |     Cervarese Santa Croce         | 2778  | 2825   | 5603   |
| 28031    | Cinto Euganeo                 | PD        | 14     | 2       |     Cinto Euganeo                 | 965   | 941    | 1906   |
| 28032    | Cittadella                    | PD        | 52     | 12      |     Cittadella                    | 9792  | 10231  | 20023  |
| 28033    | Codevigo                      | PD        | 6      | 7       |     Codevigo                      | 3239  | 3065   | 6304   |
| 28034    | Conselve                      | PD        | 13     | 14      |     Conselve                      | 4846  | 5111   | 9957   |
| 28035    | Correzzola                    | PD        | 6      | 8       |     Correzzola                    | 2519  | 2474   | 4993   |
| 28036    | Curtarolo                     | PD        | 8      | 7       |     Curtarolo                     | 3513  | 3609   | 7122   |
| 28106    | Due Carrare                   | PD        | 17     | 9       |     Due Carrare                   | 4517  | 4486   | 9003   |
| 28037    | Este                          | PD        | 42     | 22      |     Este                          | 7650  | 8325   | 15975  |
| 28038    | Fontaniva                     | PD        | 21     | 5       |     Fontaniva                     | 4036  | 4012   | 8048   |
| 28039    | Galliera Veneta               | PD        | 13     | 4       |     Galliera Veneta               | 3523  | 3538   | 7061   |
| 28040    | Galzignano Terme              | PD        | 14     | 2       |     Galzignano Terme              | 2114  | 2174   | 4288   |
| 28041    | Gazzo                         | PD        | 12     | 3       |     Gazzo                         | 2151  | 2139   | 4290   |
| 28042    | Grantorto                     | PD        | 7      | 2       |     Grantorto                     | 2264  | 2238   | 4502   |
| 28043    | Granze                        | PD        | 3      | 1       |     Granze                        | 931   | 986    | 1917   |
| 28044    | Legnaro                       | PD        | 2      | 3       |     Legnaro                       | 4733  | 4725   | 9458   |
| 28045    | Limena                        | PD        | 6      | 3       |     Limena                        | 4022  | 4136   | 8158   |
| 28046    | Loreggia                      | PD        | 14     | 4       |     Loreggia                      | 3912  | 3791   | 7703   |
| 28047    | Lozzo Atestino                | PD        | 10     | 7       |     Lozzo Atestino                | 1504  | 1509   | 3013   |
| 28048    | Masera' Di Padova             | PD        | 11     | 9       |     Maserà Di Padova              | 4555  | 4571   | 9126   |
| 28049    | Masi                          | PD        | 4      | 1       |     Masi                          | 877   | 920    | 1797   |
| 28050    | Massanzago                    | PD        | 10     | 5       |     Massanzago                    | 3062  | 2974   | 6036   |
| 28052    | Megliadino San Vitale         | PD        | 5      | 3       |     Megliadino San Vitale         | 903   | 893    | 1796   |
| 28053    | Merlara                       | PD        | 5      | 2       |     Merlara                       | 1230  | 1281   | 2511   |
| 28054    | Mestrino                      | PD        | 8      | 13      |     Mestrino                      | 5766  | 5962   | 11728  |
| 28055    | Monselice                     | PD        | 28     | 16      |     Monselice                     | 8359  | 8861   | 17220  |
| 28056    | Montagnana                    | PD        | 18     | 7       |     Montagnana                    | 4353  | 4584   | 8937   |
| 28057    | Montegrotto Terme             | PD        | 16     | 8       |     Montegrotto Terme             | 5483  | 5908   | 11391  |
| 28058    | Noventa Padovana              | PD        | 9      | 8       |     Noventa Padovana              | 5653  | 5815   | 11468  |
| 28059    | Ospedaletto Euganeo           | PD        | 8      | 4       |     Ospedaletto Euganeo           | 2750  | 2799   | 5549   |
| 28060    | Padova                        | PD        | 355    | 125     |     Padova                        | 98604 | 107892 | 206496 |
| 28061    | Pernumia                      | PD        | 5      | 8       |     Pernumia                      | 1891  | 1874   | 3765   |
| 28062    | Piacenza D'Adige              | PD        | 4      |         |     Piacenza D'Adige              | 609   | 620    | 1229   |
| 28063    | Piazzola Sul Brenta           | PD        | 16     | 3       |     Piazzola Sul Brenta           | 5477  | 5602   | 11079  |
| 28064    | Piombino Dese                 | PD        | 9      | 15      |     Piombino Dese                 | 4741  | 4656   | 9397   |
| 28065    | Piove Di Sacco                | PD        | 18     | 32      |     Piove Di Sacco                | 9696  | 10308  | 20004  |
| 28066    | Polverara                     | PD        | 6      | 2       |     Polverara                     | 1678  | 1722   | 3400   |
| 28067    | Ponso                         | PD        | 4      | 4       |     Ponso                         | 1213  | 1178   | 2391   |
| 28069    | Ponte San Nicolo'             | PD        | 13     | 14      |     Ponte San Nicolò              | 6365  | 6826   | 13191  |
| 28068    | Pontelongo                    | PD        | 4      | 4       |     Pontelongo                    | 1827  | 1813   | 3640   |
| 28070    | Pozzonovo                     | PD        | 3      | 2       |     Pozzonovo                     | 1685  | 1745   | 3430   |
| 28071    | Rovolon                       | PD        | 10     | 1       |     Rovolon                       | 2459  | 2454   | 4913   |
| 28072    | Rubano                        | PD        | 17     | 19      |     Rubano                        | 8166  | 8690   | 16856  |
| 28073    | Saccolongo                    | PD        | 3      | 2       |     Saccolongo                    | 2464  | 2461   | 4925   |
| 28075    | San Giorgio Delle Pertiche    | PD        | 16     | 8       |     San Giorgio Delle Pertiche    | 5043  | 5040   | 10083  |
| 28076    | San Giorgio In Bosco          | PD        | 20     | 5       |     San Giorgio In Bosco          | 3209  | 3168   | 6377   |
| 28077    | San Martino Di Lupari         | PD        | 11     | 11      |     San Martino Di Lupari         | 6579  | 6630   | 13209  |
| 28078    | San Pietro In Gu'             | PD        | 10     | 1       |     San Pietro In Gu              | 2080  | 2118   | 4198   |
| 28079    | San Pietro Viminario          | PD        | 6      | 3       |     San Pietro Viminario          | 1557  | 1494   | 3051   |
| 28080    | Santa Giustina In Colle       | PD        | 17     | 6       |     Santa Giustina In Colle       | 3580  | 3535   | 7115   |
| 28082    | Sant'Angelo Di Piove Di Sacco | PD        | 5      | 9       |     Sant'Angelo Di Piove Di Sacco | 3626  | 3698   | 7324   |
| 28083    | Sant'Elena                    | PD        | 4      | 3       |     Sant'Elena                    | 1225  | 1292   | 2517   |
| 28084    | Sant'Urbano                   | PD        | 7      | 1       |     Sant'Urbano                   | 951   | 954    | 1905   |
| 28085    | Saonara                       | PD        | 13     | 9       |     Saonara                       | 5196  | 5285   | 10481  |
| 28086    | Selvazzano Dentro             | PD        | 26     | 13      |     Selvazzano Dentro             | 11040 | 11792  | 22832  |
| 28087    | Solesino                      | PD        | 3      | 16      |     Solesino                      | 3321  | 3416   | 6737   |
| 28088    | Stanghella                    | PD        | 6      | 2       |     Stanghella                    | 2029  | 2071   | 4100   |
| 28089    | Teolo                         | PD        | 24     | 7       |     Teolo                         | 4336  | 4529   | 8865   |
| 28090    | Terrassa Padovana             | PD        | 4      | 2       |     Terrassa Padovana             | 1347  | 1328   | 2675   |
| 28091    | Tombolo                       | PD        | 6      | 9       |     Tombolo                       | 4021  | 4111   | 8132   |
| 28092    | Torreglia                     | PD        | 11     | 4       |     Torreglia                     | 2958  | 3045   | 6003   |
| 28093    | Trebaseleghe                  | PD        | 19     | 10      |     Trebaseleghe                  | 6488  | 6448   | 12936  |
| 28094    | Tribano                       | PD        | 9      | 3       |     Tribano                       | 2112  | 2083   | 4195   |
| 28095    | Urbana                        | PD        | 1      |         |     Urbana                        | 1010  | 1006   | 2016   |
| 28096    | Veggiano                      | PD        | 7      | 4       |     Veggiano                      | 2437  | 2380   | 4817   |
| 28097    | Vescovana                     | PD        | 1      | 1       |     Vescovana                     | 844   | 871    | 1715   |
| 28098    | Vighizzolo D'Este             | PD        | 4      |         |     Vighizzolo D'Este             | 456   | 408    | 864    |
| 28099    | Vigodarzere                   | PD        | 12     | 10      |     Vigodarzere                   | 6473  | 6670   | 13143  |
| 28100    | Vigonza                       | PD        | 31     | 22      |     Vigonza                       | 11300 | 11772  | 23072  |
| 28101    | Villa Del Conte               | PD        | 14     | 7       |     Villa Del Conte               | 2839  | 2753   | 5592   |
| 28102    | Villa Estense                 | PD        | 5      | 5       |     Villa Estense                 | 1053  | 1034   | 2087   |
| 28103    | Villafranca Padovana          | PD        | 14     | 5       |     Villafranca Padovana          | 5146  | 5357   | 10503  |
| 28104    | Villanova Di Camposampiero    | PD        | 6      | 3       |     Villanova Di Camposampiero    | 3084  | 3076   | 6160   |
| 28105    | Vo'                           | PD        | 12     | 6       |     Vo'                           | 1626  | 1638   | 3264   |
