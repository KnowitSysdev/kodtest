# Knowit kodtest

## Uppgift
Bygg ett API som hämtar miljödata om en given typ av växthusgas från olika inrikes transporter, under en given period, 
från SCBs publika API:er och returnerar årlig utveckling av utsläpp för varje enskild fordonstyp under den givna perioden. 

**SCB API dokumentation:** https://www.scb.se/vara-tjanster/oppna-data/api-for-statistikdatabasen/

Har du tid över ser vi gärna att du börjar på extrauppgifterna i den givna ordningen.

### Krav 
* REST API
* API:t skall kunna ta emot följande in-data
  * Startår
  * Slutår
  * Utsläppstyp
  * En eller flera fordonstyper
* Förväntat resultat
  * Årlig utveckling för utsläppsvolym per fordonstyp
* Unit tester

#### Tips och Hjälpmedel
* CAGR formel för uträkning av årlig utveckling: https://en.wikipedia.org/wiki/Compound_annual_growth_rate
* Följ SCBs självdokumenterade API istället för att läsa PDF:en på sidan. Startpunkt: http://api.scb.se/OV0104/v1/doris/sv/ssd/ 
* För hjälp att genera api anrop kan följande sida användas http://www.statistikdatabasen.scb.se/pxweb/sv/ssd/START__MI__MI0107/MI0107InTransp/

### Extrauppgifter
1. Möjlighet att fråga efter både inrikes och utrikes transporter
2. Kompletta integrationstester
3. Körbar i Docker
