# coronavirus-stats
Gather statistics from Coronavirus (COVID-19) from Italy and Spain. My objective is to have an idea of when will happen the "peak".

This data must be analyzed taking a step back as they don't represent the reality:
- positive: not everyone is tested and people which have the symtoms are not tested neither. The day that we will have massing testing that number will increase, but it won't mean that the situation is worse.
- ICU: number of people in ICU is difficult to analyze as a stagnancy can mean that there a no new patient or that the hospital is full
- Hospitalization: number of people hospitalized : this is maybe the more accurate indicator although hospitals can be full
It will be great to have the number of suspicious cases (has all the symptoms but cannot be tested as the shortage of test).


Data are also available in a more viewable way in [Google Spreadsheet](https://docs.google.com/spreadsheets/d/1RCuQGKy3fer6LVD8rTL1k2gODxnVnkmWNEu09oWrvNw/edit) with also the data of Italy/Lombardia and Spain/Madrid gathered.

# Italy
Everyday around around 18.30 the Health Ministry publish a [pdf](http://www.salute.gov.it/imgs/C_17_pagineAree_5351_38_file.pdf) with last data on their [website](http://www.salute.gov.it/portale/nuovocoronavirus/archivioNotizieNuovoCoronavirus.jsp). Alternative source of data https://github.com/pcm-dpc/COVID-19

Columns of CSV:  
- Date: date of report
- Region :
- Hospitalized
- ICU
- Positive at home
- Currently positive
- Cured	
- Dead
- Postive total : cumulated
- Tested
- Source

# Spain

Graphs:
- <iframe width="600" height="371" seamless frameborder="0" scrolling="no" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRsgc5fWov1VQEagBZuJFilLC0scEF6U4VfVofBIhB4C3mD6fe8mnXTOVM6BUpcoARGkcXxObJjDW_V/pubchart?oid=682356145&amp;format=interactive"></iframe>
- ![ES-MAD.UCI](https://docs.google.com/spreadsheets/d/e/2PACX-1vRsgc5fWov1VQEagBZuJFilLC0scEF6U4VfVofBIhB4C3mD6fe8mnXTOVM6BUpcoARGkcXxObJjDW_V/pubchart?oid=682356145&format=image)

Everyday around 11:30 a pdf the Health Ministry publish a [pdf](https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov-China/documentos/Actualizacion_57_COVID-19.pdf) with last data on that [page](https://www.mscbs.gob.es/profesionales/saludPublica/ccayes/alertasActual/nCov-China/situacionActual.htm).
Please take into account that not everyone which has the symptom will be tested, thus the real number of positive people will be higher. 
Thoses reports also contains data from other countries and Spanish data grouped by age.


Columns of CSV:  
- Date: Date of the report
- Region: Country or [Autonomous community](https://en.wikipedia.org/wiki/Autonomous_communities_of_Spain) - eg "Spain" or "Madrid" (Community of Madrid != City of Madrid)
- Positive total: total number of cases (cumulated)
- IA : Cases/100.000 inhabitants
- Hospitalized
- ICU
- Dead
- Cured
- New positive
- Source : link to the PDF


# France 
Data are available in that [page](https://www.santepubliquefrance.fr/maladies-et-traumatismes/maladies-et-infections-respiratoires/infection-a-coronavirus/articles/infection-au-nouveau-coronavirus-sars-cov-2-covid-19-france-et-monde) or from the [open data website](https://www.data.gouv.fr/fr/datasets/donnees-des-ugences-hospitalieres-et-de-sos-medecins-relatives-a-lepidemie-de-covid-19/). Map tool : https://veille-coronavirus.fr/

The 03/23/2020, the government indicates that the number of deaths can be 3 times higher given that the data only take into account people dead in hospitals (not in retirement home).

# Extracting data
IT & ES data has been extracted from the pdfs using [PDF to Excel converter](https://www.ilovepdf.com/pdf_to_excel) (but sometime because of "." or "," the number are wrongly converted).
