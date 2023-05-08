# APPLICAZIONE DELLA LEGGE REGIONALE SUL GIOCO D'AZZARDO IN PROVINCIA DI PADOVA

Questo progetto vuole verificare se la posizione dlle slot machine in provincia di Padova rispetta le norme della [LEGGE REGIONALE  n. 38 del 10 settembre 2019
](https://bur.regione.veneto.it/BurvServices/pubblica/DettaglioLegge.aspx?id=402726).  
Si specifica che la legge si applica alle nuove installazioni, per questo progetto invece utilizzeremo l'intero dataset di slotmachine per vedere quali sarebbero mal posizionate.
Il lavoro prende spunto da un [progetto analogo](https://github.com/skampus/ludopatia) di Stefano Campus per la Regione Piemonte.

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

| Codistat | Nomcom                        | Provincia | N_slot | Slot_Non_Regola | M     | F      | TOT    | Area_km2 | Dens_pop |
|:--------:|:-----------------------------:|:---------:|:------:|:-------:|:-----:|:------:|:------:|:--------:|:--------:|
| 28001    | Abano Terme                   | PD        | 22     | 14      | 9653  | 10578  | 20231  | 21.53    | 939.67   |
| 28002    | Agna                          | PD        | 3      | 2       | 1554  | 1603   | 3157   | 18.87    | 167.3    |
| 28003    | Albignasego                   | PD        | 20     | 16      | 13055 | 13835  | 26890  | 20.97    | 1282.31  |
| 28004    | Anguillara Veneta             | PD        | 5      | 3       | 2037  | 2087   | 4124   | 21.55    | 191.37   |
| 28005    | Arqua' Petrarca               | PD        | 0      | 0       | 900   | 910    | 1810   | 12.53    | 144.45   |
| 28006    | Arre                          | PD        | 2      | 1       | 1053  | 1038   | 2091   | 12.47    | 167.68   |
| 28007    | Arzergrande                   | PD        | 6      | 6       | 2366  | 2422   | 4788   | 13.67    | 350.26   |
| 28008    | Bagnoli Di Sopra              | PD        | 2      | 2       | 1700  | 1696   | 3396   | 34.89    | 97.33    |
| 28009    | Baone                         | PD        | 1      | 0       | 1545  | 1513   | 3058   | 24.47    | 124.97   |
| 28010    | Barbona                       | PD        | 0      | 0       | 300   | 285    | 585    | 8.58     | 68.18    |
| 28011    | Battaglia Terme               | PD        | 6      | 6       | 1847  | 1919   | 3766   | 6.26     | 601.6    |
| 28012    | Boara Pisani                  | PD        | 6      | 2       | 1195  | 1184   | 2379   | 16.49    | 144.27   |
| 28107    | Borgo Veneto                  | PD        | 8      | 6       | 3535  | 3481   | 7016   | 39.19    | 179.03   |
| 28013    | Borgoricco                    | PD        | 8      | 7       | 4509  | 4460   | 8969   | 20.47    | 438.15   |
| 28014    | Bovolenta                     | PD        | 2      | 0       | 1722  | 1718   | 3440   | 22.72    | 151.41   |
| 28015    | Brugine                       | PD        | 10     | 5       | 3526  | 3634   | 7160   | 19.58    | 365.68   |
| 28016    | Cadoneghe                     | PD        | 13     | 8       | 7643  | 8158   | 15801  | 12.85    | 1229.65  |
| 28020    | Campo San Martino             | PD        | 6      | 4       | 2825  | 2780   | 5605   | 13.14    | 426.56   |
| 28017    | Campodarsego                  | PD        | 15     | 12      | 7455  | 7617   | 15072  | 25.61    | 588.52   |
| 28018    | Campodoro                     | PD        | 1      | 1       | 1311  | 1296   | 2607   | 11.42    | 228.28   |
| 28019    | Camposampiero                 | PD        | 6      | 4       | 5866  | 5951   | 11817  | 21.12    | 559.52   |
| 28021    | Candiana                      | PD        | 1      | 1       | 1127  | 1065   | 2192   | 22.36    | 98.03    |
| 28022    | Carceri                       | PD        | 1      | 1       | 731   | 739    | 1470   | 9.72     | 151.23   |
| 28023    | Carmignano Di Brenta          | PD        | 3      | 3       | 3723  | 3660   | 7383   | 14.75    | 500.54   |
| 28026    | Cartura                       | PD        | 5      | 5       | 2258  | 2309   | 4567   | 16.22    | 281.57   |
| 28027    | Casale Di Scodosia            | PD        | 5      | 4       | 2331  | 2316   | 4647   | 21.19    | 219.3    |
| 28028    | Casalserugo                   | PD        | 3      | 0       | 2659  | 2707   | 5366   | 15.54    | 345.3    |
| 28029    | Castelbaldo                   | PD        | 1      | 1       | 702   | 718    | 1420   | 15.14    | 93.79    |
| 28030    | Cervarese Santa Croce         | PD        | 3      | 3       | 2778  | 2825   | 5603   | 17.56    | 319.08   |
| 28031    | Cinto Euganeo                 | PD        | 2      | 0       | 965   | 941    | 1906   | 19.79    | 96.31    |
| 28032    | Cittadella                    | PD        | 12     | 11      | 9792  | 10231  | 20023  | 36.45    | 549.33   |
| 28033    | Codevigo                      | PD        | 7      | 4       | 3239  | 3065   | 6304   | 70.01    | 90.04    |
| 28034    | Conselve                      | PD        | 14     | 10      | 4846  | 5111   | 9957   | 24.29    | 409.92   |
| 28035    | Correzzola                    | PD        | 8      | 8       | 2519  | 2474   | 4993   | 42.37    | 117.84   |
| 28036    | Curtarolo                     | PD        | 7      | 3       | 3513  | 3609   | 7122   | 14.84    | 479.92   |
| 28106    | Due Carrare                   | PD        | 9      | 6       | 4517  | 4486   | 9003   | 26.59    | 338.59   |
| 28037    | Este                          | PD        | 22     | 18      | 7650  | 8325   | 15975  | 32.73    | 488.08   |
| 28038    | Fontaniva                     | PD        | 5      | 5       | 4036  | 4012   | 8048   | 20.62    | 390.3    |
| 28039    | Galliera Veneta               | PD        | 4      | 4       | 3523  | 3538   | 7061   | 9.01     | 783.68   |
| 28040    | Galzignano Terme              | PD        | 2      | 2       | 2114  | 2174   | 4288   | 18.16    | 236.12   |
| 28041    | Gazzo                         | PD        | 3      | 1       | 2151  | 2139   | 4290   | 22.69    | 189.07   |
| 28042    | Grantorto                     | PD        | 2      | 2       | 2264  | 2238   | 4502   | 14.08    | 319.74   |
| 28043    | Granze                        | PD        | 1      | 1       | 931   | 986    | 1917   | 11.48    | 166.99   |
| 28044    | Legnaro                       | PD        | 3      | 0       | 4733  | 4725   | 9458   | 14.91    | 634.34   |
| 28045    | Limena                        | PD        | 3      | 2       | 4022  | 4136   | 8158   | 15.12    | 539.55   |
| 28046    | Loreggia                      | PD        | 4      | 2       | 3912  | 3791   | 7703   | 19.22    | 400.78   |
| 28047    | Lozzo Atestino                | PD        | 7      | 6       | 1504  | 1509   | 3013   | 23.99    | 125.59   |
| 28048    | Masera' Di Padova             | PD        | 9      | 9       | 4555  | 4571   | 9126   | 17.53    | 520.59   |
| 28049    | Masi                          | PD        | 1      | 1       | 877   | 920    | 1797   | 13.33    | 134.81   |
| 28050    | Massanzago                    | PD        | 5      | 5       | 3062  | 2974   | 6036   | 13.24    | 455.89   |
| 28052    | Megliadino San Vitale         | PD        | 3      | 2       | 903   | 893    | 1796   | 15.14    | 118.63   |
| 28053    | Merlara                       | PD        | 2      | 1       | 1230  | 1281   | 2511   | 21.44    | 117.12   |
| 28054    | Mestrino                      | PD        | 13     | 9       | 5766  | 5962   | 11728  | 19.29    | 607.98   |
| 28055    | Monselice                     | PD        | 16     | 11      | 8359  | 8861   | 17220  | 50.63    | 340.11   |
| 28056    | Montagnana                    | PD        | 7      | 4       | 4353  | 4584   | 8937   | 45.03    | 198.47   |
| 28057    | Montegrotto Terme             | PD        | 8      | 7       | 5483  | 5908   | 11391  | 15.34    | 742.57   |
| 28058    | Noventa Padovana              | PD        | 8      | 2       | 5653  | 5815   | 11468  | 7.14     | 1606.16  |
| 28059    | Ospedaletto Euganeo           | PD        | 4      | 2       | 2750  | 2799   | 5549   | 21.42    | 259.06   |
| 28060    | Padova                        | PD        | 125    | 111     | 98604 | 107892 | 206496 | 93.26    | 2214.2   |
| 28061    | Pernumia                      | PD        | 8      | 8       | 1891  | 1874   | 3765   | 13.22    | 284.8    |
| 28062    | Piacenza D'Adige              | PD        | 0      | 0       | 609   | 620    | 1229   | 18.55    | 66.25    |
| 28063    | Piazzola Sul Brenta           | PD        | 3      | 3       | 5477  | 5602   | 11079  | 40.89    | 270.95   |
| 28064    | Piombino Dese                 | PD        | 15     | 12      | 4741  | 4656   | 9397   | 29.52    | 318.33   |
| 28065    | Piove Di Sacco                | PD        | 32     | 21      | 9696  | 10308  | 20004  | 35.66    | 560.96   |
| 28066    | Polverara                     | PD        | 2      | 2       | 1678  | 1722   | 3400   | 9.87     | 344.48   |
| 28067    | Ponso                         | PD        | 4      | 4       | 1213  | 1178   | 2391   | 10.97    | 217.96   |
| 28069    | Ponte San Nicolo'             | PD        | 14     | 11      | 6365  | 6826   | 13191  | 13.52    | 975.67   |
| 28068    | Pontelongo                    | PD        | 4      | 3       | 1827  | 1813   | 3640   | 10.65    | 341.78   |
| 28070    | Pozzonovo                     | PD        | 2      | 2       | 1685  | 1745   | 3430   | 24.45    | 140.29   |
| 28071    | Rovolon                       | PD        | 1      | 1       | 2459  | 2454   | 4913   | 27.53    | 178.46   |
| 28072    | Rubano                        | PD        | 19     | 15      | 8166  | 8690   | 16856  | 14.47    | 1164.89  |
| 28073    | Saccolongo                    | PD        | 2      | 1       | 2464  | 2461   | 4925   | 13.76    | 357.92   |
| 28075    | San Giorgio Delle Pertiche    | PD        | 8      | 6       | 5043  | 5040   | 10083  | 18.81    | 536.04   |
| 28076    | San Giorgio In Bosco          | PD        | 5      | 3       | 3209  | 3168   | 6377   | 28.43    | 224.31   |
| 28077    | San Martino Di Lupari         | PD        | 11     | 5       | 6579  | 6630   | 13209  | 24.27    | 544.25   |
| 28078    | San Pietro In Gu'             | PD        | 1      | 1       | 2080  | 2118   | 4198   | 17.8     | 235.84   |
| 28079    | San Pietro Viminario          | PD        | 3      | 3       | 1557  | 1494   | 3051   | 13.29    | 229.57   |
| 28080    | Santa Giustina In Colle       | PD        | 6      | 4       | 3580  | 3535   | 7115   | 17.93    | 396.82   |
| 28082    | Sant'Angelo Di Piove Di Sacco | PD        | 9      | 3       | 3626  | 3698   | 7324   | 13.99    | 523.52   |
| 28083    | Sant'Elena                    | PD        | 3      | 3       | 1225  | 1292   | 2517   | 8.92     | 282.17   |
| 28084    | Sant'Urbano                   | PD        | 1      | 1       | 951   | 954    | 1905   | 32.04    | 59.46    |
| 28085    | Saonara                       | PD        | 9      | 8       | 5196  | 5285   | 10481  | 13.49    | 776.95   |
| 28086    | Selvazzano Dentro             | PD        | 13     | 10      | 11040 | 11792  | 22832  | 19.64    | 1162.53  |
| 28087    | Solesino                      | PD        | 16     | 7       | 3321  | 3416   | 6737   | 10.24    | 657.91   |
| 28088    | Stanghella                    | PD        | 2      | 2       | 2029  | 2071   | 4100   | 19.7     | 208.12   |
| 28089    | Teolo                         | PD        | 7      | 5       | 4336  | 4529   | 8865   | 31.29    | 283.32   |
| 28090    | Terrassa Padovana             | PD        | 2      | 2       | 1347  | 1328   | 2675   | 14.7     | 181.97   |
| 28091    | Tombolo                       | PD        | 9      | 5       | 4021  | 4111   | 8132   | 11.12    | 731.29   |
| 28092    | Torreglia                     | PD        | 4      | 2       | 2958  | 3045   | 6003   | 18.6     | 322.74   |
| 28093    | Trebaseleghe                  | PD        | 10     | 8       | 6488  | 6448   | 12936  | 30.79    | 420.14   |
| 28094    | Tribano                       | PD        | 3      | 3       | 2112  | 2083   | 4195   | 19.27    | 217.7    |
| 28095    | Urbana                        | PD        | 0      | 0       | 1010  | 1006   | 2016   | 17.06    | 118.17   |
| 28096    | Veggiano                      | PD        | 4      | 2       | 2437  | 2380   | 4817   | 16.23    | 296.8    |
| 28097    | Vescovana                     | PD        | 1      | 0       | 844   | 871    | 1715   | 22.23    | 77.15    |
| 28098    | Vighizzolo D'Este             | PD        | 0      | 0       | 456   | 408    | 864    | 17.13    | 50.44    |
| 28099    | Vigodarzere                   | PD        | 10     | 7       | 6473  | 6670   | 13143  | 19.95    | 658.8    |
| 28100    | Vigonza                       | PD        | 22     | 12      | 11300 | 11772  | 23072  | 33.41    | 690.57   |
| 28101    | Villa Del Conte               | PD        | 7      | 7       | 2839  | 2753   | 5592   | 17.32    | 322.86   |
| 28102    | Villa Estense                 | PD        | 5      | 5       | 1053  | 1034   | 2087   | 15.87    | 131.51   |
| 28103    | Villafranca Padovana          | PD        | 5      | 3       | 5146  | 5357   | 10503  | 23.66    | 443.91   |
| 28104    | Villanova Di Camposampiero    | PD        | 3      | 2       | 3084  | 3076   | 6160   | 12.17    | 506.16   |
| 28105    | Vo'                           | PD        | 6      | 5       | 1626  | 1638   | 3264   | 20.38    | 160.16   |

