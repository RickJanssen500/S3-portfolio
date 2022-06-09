# hoe kan ik de usability van mijn app verhogen?
# Inhoudsopgave

- [Inleiding](#inleiding)
- [Hoe laat je artikelvoorraad het best zien?](#hoe-laat-je-artikelvoorraad-het-best-zien)
  * [hoe doen andere het?](#hoe-doen-andere-het)
    + [Coolblue](#coolblue)
    + [Bol.com](#bolcom)
    + [Etrias](#etrias)
    + [Hema](#hema)
  * [Mogelijke aanpassingen voor mijn Applicatie](#mogelijke-aanpassingen-voor-mijn-applicatie)
    + [Wat vindt het testpanel van Mogelijke opties?](#wat-vindt-het-testpanel-van-mogelijke-opties)
- [Hoe laat je winkelwageninhoud het best zien?](#hoe-laat-je-winkelwageninhoud-het-best-zien)
  * [hoe doen andere het?](#hoe-doen-andere-het-1)
    + [Coolblue](#coolblue-1)
    + [Bol.com](#bolcom-1)
    + [Etrias](#etrias-1)
    + [Hema](#hema-1)
  * [Mogelijke aanpassingen voor mijn Applicatie](#mogelijke-aanpassingen-voor-mijn-applicatie-1)
    + [Wat vindt het testpanel van Mogelijke opties?](#wat-vindt-het-testpanel-van-mogelijke-opties-1)
- [Conclusie](#conclusie)
- [bronnen](#bronnen)

# Inleiding
In een feedback gepsrek met een van mijn docenten kreeg ik als feedback punt dat mijn usability niet overal even goed is.
Dit komt doordat de gebruiker niet duidelijk geinformeerd word over waarom hij een bepaalde hadeling niet kan doen.
Of dat er een getal in beeld als misleidend kan worden gezien. Na deze feedback te hebben ontvangen ben ik in mijn project een aantal van deze fouten gezocht.
Om deze punten te verbeteren heb ik eerst gekeken naar hoe andere webshops dit gedaan hebben om de usability voor hun gebruikers te verhogen.
Ik heb hierin naar 4 verschillende webshops geken om veel verschillende indrukken te krijgen. Deze webshops zijn: Coolblue, Bol.com, Etrias en Hema.   
Ik heb voor deze webshops gekozen omdat ik hier mee naar verschillende type webshops kijk en naar de grootste.
Nadat ik dit gedaan heb heb ik in mijn eigen app hier een aantal variaties op gemaakt en aan een testpanel gevraagd wat hun het fijnst vonden.
In dit onderzoek zal ik ingaan op 2 punten van usability binnen mijn Vue frontend.

# Hoe laat je artikelvoorraad het best zien?  
Het eerste usability item dat ik ga onderzoek is de artikelvoorraad.
Op dit moment begrensd de frontend het maximaal aantal van een product dat je kunt bestellen aan de hand van de artikelvoorraad.
Maar de frontend geeft de gebruiker hier geen melding van, waardoor de gebruiker niet wist waarom hij er maar bijvoordbeeld 7 van dit item kon bestellen.

## hoe doen andere het?
Om te kijken hoe anderen webshops dit deden heb ik zoveel mogelijk van 1 product proberen te bestellen en gekeken of er een melding gegeven wordt.
Als er een melding gegeven werd heb ik gekeken wat voor melding het was en welke informatie er allemaal in deze melding staat.

### Coolblue
Bij Coolblue heb ik meerdere verschillende artikellen geprobeerd omdat ik geen melding of iets kreeg.
Zo kon ik van alle producten er 999 bestellen en beloofde Coolblue nog steeds dat ik ze de volgende dag in huis zou hebben.
Het max aantal te bestellen van 1 product staat bij Coolblue dus hardcoded vast op 999.
Conclusie: Coolblue houd geen rekening met artikel voorraden en geeft de gebruiker geen enkele begrenzing of melding als er van het product niet voldoende op voorraad is.

### Bol.com
Bij Bol.com heb ik een paar honderd TP-Link TL-SG105 proberen te bestellen, toen ik naar de bestelpagina ging gaf Bol.com mij de volgende melding.
| ![product bol](https://user-images.githubusercontent.com/84378377/171406511-a852b4a5-7724-46d8-acbf-f502294ce21c.png) |
| :--: |
| Warning van Bol.com |

In deze melding geeft Bol.com aan om welk product in je winkelwagentje gaat.
Hierin geven ze aan het gewenste aantal niet op voorraad te hebben waardoor de levertijd langer wordt. Ook geven ze hun huidige voorraad(in dit geval 45) als advies aantal om de gewoone levertijd te behouden.

### Etrias
Bij Etrias heb ik 100 tennisballen proberen te bestellen. Op het moment dat ik dit invul laat hij dit aantal staan en geeft hij een melding.
| ![product etrias](https://user-images.githubusercontent.com/84378377/171806678-ea9321a2-2e09-439e-aa58-0cf36b62351a.png) |
| :--: |
| Melding van Etrias |

In deze melding geven ze aan de gebruiker niet aan wat er niet klopt ze zeggen alleen bad request. De gebruiker weet dus niet precies wat er aan de hand is.
Op het moment dat je doorgaat naar de bestel pagina zal hij het bestelde aantal aanpassen naar de aanwezige voorraad, echter laat hij dit niet aan de gebruiker weten.
Als je dit als gebruiker niet controleert denk je dat je er meer besteld dan dat je daadwerkelijk krijgt.

### Hema  
Bij de Hema heb ik veel zwembroeken proberen te bestellen, echter lukte dit niet omdat de input begrensd is op de artikel voorraad.
Dit is de eerste site waarbij de input een hoger aantal niet toelaat de andere site's kun je alles invullen.
| ![product hema](https://user-images.githubusercontent.com/84378377/171809187-60ffd5d7-0b49-4938-8a6f-8da246b8033e.png) |
| :--: |
| Melding van Hema |

De melding geeft duidelijk aan dat ik maar 3 van dit artikel kan bestellen waardoor ik als gebruiker snap waarom ik er maar 3 kan invullen in het aantal vak.

## Mogelijke aanpassingen voor mijn Applicatie   
Na te hebben gezien hoe andere webshops dit doen heb ik voor mijn eigen site 3 alternatieven gemaakt die geinspireerd zijn op alle voordbeelden die ik gezien heb.   

| ![product zonder error](https://user-images.githubusercontent.com/84378377/172813589-e6d076eb-810d-4b71-9cf6-717b3ed410aa.png) |
| :--: |
| origineel element |   

Hierboven zie je hoe het er op mijn webshop origineel uitziet.   
Een van de variaties die ik gemaakt heb is een error in het rood zodat de gebruiker duidelijk ziet dat er iets niet klopt.   
| ![product met error](https://user-images.githubusercontent.com/84378377/172814375-1e8e1e0c-6e49-4506-be47-1d82ae4a67ac.png) |
| :--: |
| voordbeeld met error |   
   
Hier naast heb ik nog een blauwe message box gemaakt die zegt wat het maximaal te bestellen aantal is.   
| ![product met message](https://user-images.githubusercontent.com/84378377/172814826-798a2dbf-6f58-49f0-9d37-b5ae669c010b.png) |
| :--: |
| voordbeeld met message |   
   
Als laatste heb ik nog een variatie gemaakt waar de artikel voorrad onder het artikel komt te staan.   
| ![product message](https://user-images.githubusercontent.com/84378377/172814844-eaeb2616-fc2a-48a0-93aa-55f1ae01de78.png) |
| :--: |
| voordbeeld met aantal |  

### Wat vindt het testpanel van Mogelijke opties?   
Nadat ik deze voordbeelden gemaakt heb heb ik deze voorgelegd aan een test om te kijken welke mogelijkheid bij hun het beste in de smaak valt.   
Dit testpanel bestaat uit gebruikers van webshops en mensen die voor webshops werken.   
Dit om te zorgen dat het testpanel zo goed mogelijk aansluit bij de doelgroep voor de applicatie.   
Nadat ik deze voordbeelden heb voorgelegd aan het panel kwam hier de volgende conclusie uit.   
Het test panel wil een combinatie uit meerdere voordbeelden.  
Zo willen ze dat standaard de artikel voorraad in beeld is en ze een melding krijgen las ze teveel proberen te bestellen.   
De melding die vanuit hun de voorkeur kreeg was de error message in het rood.   
Dus het artikel aantal altijd in beeld en bij overschreiden de rode error weergeven.   

# Hoe laat je winkelwageninhoud het best zien?   
Het tweede usability item dat ik ga onderzoek is de winkelwageninhoud. Op dit moment laat de frontend het aantal verschillende producten zien 
en niet het totaal aantal artikelen in de winkelwagen.   
Dit zou voor de gebruiker verwarrend kunne zijn omdat ze nu niet precies weten wat er in de winkelwagen zit.   

## hoe doen andere het?   
Om te kijken hoe anderen webshops dit deden heb ik van 1 product 2 besteld en van een andere product 3.   
Toen heb ik gekeken naar het aantal dat bij het winkel wagen staat.   

### Coolblue   
Coolblue laat de het aantal artikelen in het mandje zien en niet het aatal verschillende.  

| ![artikel coolblue](https://user-images.githubusercontent.com/84378377/172831590-30f4efe7-6ec3-47d5-a8b8-45aff2de8dcf.png) |
| :--: |
| winkelwagen Coolblue |

### Bol.com   
Bol.com laat de het aantal artikelen in het mandje zien en niet het aatal verschillende.  

|![artikel bol com](https://user-images.githubusercontent.com/84378377/172832003-382565ef-06a4-4660-9bd7-7d3eb84b99df.png)  |
| :--: |
| winkelwagen Bol.com |   

### Etrias   
Etrias laat de het aantal artikelen in het mandje zien en niet het aatal verschillende.  

| ![artikel etrias](https://user-images.githubusercontent.com/84378377/172832035-8a0427a5-bcfb-4bcc-a3d5-0a60b186ec3f.png) |
| :--: |
| winkelwagen Etrias |   

### Hema   
Hema laat de het aantal artikelen in het mandje zien en niet het aatal verschillende.  

| ![artikel hema 1](https://user-images.githubusercontent.com/84378377/172832056-50375887-4e4b-4e6b-87db-4803bf3d185b.png) |
| :--: |
| winkelwagen Hema |   
   
| ![artikel hema 2](https://user-images.githubusercontent.com/84378377/172832064-6fe8a766-9433-41c6-9ba4-0fabb81e065d.png) |
| :--: |
| winkelwagen aantal Hema |    

## Mogelijke aanpassingen voor mijn Applicatie   
Alle webshops waar ik naar gekeken heb laten het aantal verschillende artikelen zien en niet het aantal verschillende.   
   
| ![artikel](https://user-images.githubusercontent.com/84378377/172834373-d3fb397d-66d8-4a12-954e-056f33ffb735.png) |
| :--: |
| origineel winkelwagen aantal |   
   
Hier boven zie je het origineel waar ik het aantal verschillende artikelen laat zien.   
Ik heb dus ook een variatie gemaakt waarin ik het totaal aantal producten lat zien ipv het aantal verschillende.   
   
| ![artikel met telsom](https://user-images.githubusercontent.com/84378377/172834380-493957a2-8a2f-4f14-b39c-8048ac698670.png) |
| :--: |
| winkelwagen aantal totaal |    
   

### Wat vindt het testpanel van Mogelijke opties?   
Toen ik deze mogelijkheden aan het test panel liet zien waren ze redelijk verward dat ik maar 1 voordbeeld alleen het aantal verschillende artikelen liet zien.   
Hierin is dus al duidelijk dat de testers voor het totaal aantal artikelen gaan. Dit word inderdaad ondersteund door de menig van het panel.
Hier moet dus de totale aantal artikeln worden laten zien voor de beste usability.

# Conclusie   
 In dit onderzoek ben ik to de conclusie gekomen dat de usability van mijn website op een aantal punten verbetert kan worden.   
 Ook niet dat er een goede oplossing is maar ook meer dat er een combinatie van meerdere oplossingen gemaakt kan worden.   
 De punten die verbetert kunnen worden zijn dan ook:   
 Het max aantal dat je van een product moet bestellen. Hiervoor wil de klant beter geinformeerd worden door de artikel voorraad altijd in beeld staat.   
 Hierbij willen ze ook een opvallende error message als dit aantal toch overschreden wordt.   
 Bij het aantal van de winkel wagen willen ze het totaal aantal artikelen zien en niet het aantal verschillende.   
 Dit zorgde namelijk voor verwarring.   
 Door dit onderzoek ben ik naast dat ik een verbeterde ui heb ook beseft dat je op meerdere manieren naar ui schets kan kijken 
 en dat de oplossing vaak in een combinatie van dit is i.p.v. 1 goede oplossing.
  
# bronnen   
 - [Coolblue](https://www.coolblue.nl/)
 - [Bol.com](https://www.bol.com/nl/nl/)
 - [Etrias](https://www.etrias.nl/)
 - [Hema](https://www.hema.nl/)
