# hoe kan ik de usability van mijn app verhogen?
## Inhoudsopgave

- [Inleiding](#inleiding)
- [Hoe laat je artikelvoorraad het best zien?](#hoe-laat-je-artikelvoorraad-het-best-zien)
  * [hoe doen andere het?](#hoe-doen-andere-het)
    + [Coolblue](#coolblue)
    + [Bol.com](#bolcom)
    + [Etrias](#etrias)
    + [Hema](#hema)
  * [Mogelijke aanpassingen voor mijn Appilicatie](#mogelijke-aanpassingen-voor-mijn-appilicatie)
    + [Wat vindt het testpanel van Mogelijke opties?](#wat-vindt-het-testpanel-van-mogelijke-opties)
- [Hoe laat je winkelwageninhoud het best zien?](#hoe-laat-je-winkelwageninhoud-het-best-zien)
  * [hoe doen andere het?](#hoe-doen-andere-het-1)
    + [Coolblue](#coolblue-1)
    + [Bol.com](#bolcom-1)
    + [Etrias](#etrias-1)
    + [Hema](#hema-1)
  * [Mogelijke aanpassingen voor mijn Appilicatie](#mogelijke-aanpassingen-voor-mijn-appilicatie-1)
    + [Wat vindt het testpanel van Mogelijke opties?](#wat-vindt-het-testpanel-van-mogelijke-opties-1)
- [Conclusie](#conclusie)
- [bronnen](#bronnen)

## Inleiding
In een feedback gepsrek met een van mijn docenten kreeg ik als feedback punt dat mijn usability niet overal even goed is.
Dit komt doordat de gebruiker niet duidelijk geinformeerd word over waarom hij een bepaalde hadeling niet kan doen.
Of dat er een getal in beeld als misleidend kan worden gezien. Na deze feedback te hebben ontvangen ben ik in mijn project een aantal van deze fouten gezocht.
Om deze punten te verbeteren heb ik eerst gekeken naar hoe andere webshops dit gedaan hebben om de usability voor hun gebruikers te verhogen.
Ik heb hierin naar 4 verschillende webshops geken om veel verschillende indrukken te krijgen. Deze webshops zijn: Coolblue, Bol.com, Etrias en Hema.
Nadat ik dit gedaan heb heb ik in mijn eigen app hier een aantal variaties op gemaakt en aan een testpanel gevraagd wat hun het fijnst vonden.
In dit onderzoek zal ik ingaan op 2 punten van usability binnen mijn Vue frontend.

## Hoe laat je artikelvoorraad het best zien?  
Het eerste usability item dat ik ga onderzoek is de artikelvoorraad.
Op dit moment begrensd de frontend het maximaal aantal van een product dat je kunt bestellen aan de hand van de artikelvoorraad.
Maar de frontend geeft de gebruiker hier geen melding van, waardoor de gebruiker niet wist waarom hij er maar bijvoordbeeld 7 van dit item kon bestellen.

### hoe doen andere het?
Om te kijken hoe anderen webshops dit deden heb ik zoveel mogelijk van 1 product proberen te bestellen en gekeken of er een melding gegeven wordt.
Als er een melding gegeven werd heb ik gekeken wat voor melding het was en welke informatie er allemaal in deze melding staat.

#### Coolblue
Bij Coolblue heb ik meerdere verschillende artikellen geprobeerd omdat ik geen melding of iets kreeg.
Zo kon ik van alle producten er 999 bestellen en beloofde Coolblue nog steeds dat ik ze de volgende dag in huis zou hebben.
Het max aantal te bestellen van 1 product staat bij Coolblue dus hardcoded vast op 999.
Conclusie: Coolblue houd geen rekening met artikel voorraden en geeft de gebruiker geen enkele begrenzing of melding als er van het product niet voldoende op voorraad is.

#### Bol.com
Bij Bol.com heb ik een paar honderd TP-Link TL-SG105 proberen te bestellen, toen ik naar de bestelpagina ging gaf Bol.com mij de volgende melding.
| ![product bol](https://user-images.githubusercontent.com/84378377/171406511-a852b4a5-7724-46d8-acbf-f502294ce21c.png) |
| :--: |
| Warning van Bol.com |

In deze melding geeft Bol.com aan om welk product in je winkelwagentje gaat.
Hierin geven ze aan het gewenste aantal niet op voorraad te hebben waardoor de levertijd langer wordt. Ook geven ze hun huidige voorraad(in dit geval 45) als advies aantal om de gewoone levertijd te behouden.

#### Etrias
Bij Etrias heb ik 100 tennisballen proberen te bestellen. Op het moment dat ik dit invul laat hij dit aantal staan en geeft hij een melding.
| ![product etrias](https://user-images.githubusercontent.com/84378377/171806678-ea9321a2-2e09-439e-aa58-0cf36b62351a.png) |
| :--: |
| Melding van Etrias |

In deze melding geven ze aan de gebruiker niet aan wat er niet klopt ze zeggen alleen bad request. De gebruiker weet dus niet precies wat er aan de hand is.
Op het moment dat je doorgaat naar de bestel pagina zal hij het bestelde aantal aanpassen naar de aanwezige voorraad, echter laat hij dit niet aan de gebruiker weten.
Als je dit als gebruiker niet controleert denk je dat je er meer besteld dan dat je daadwerkelijk krijgt.

#### Hema  
Bij de Hema heb ik veel zwembroeken proberen te bestellen, echter lukte dit niet omdat de input begrensd is op de artikel voorraad.
Dit is de eerste site waarbij de input een hoger aantal niet toelaat de andere site's kun je alles invullen.
| ![product hema](https://user-images.githubusercontent.com/84378377/171809187-60ffd5d7-0b49-4938-8a6f-8da246b8033e.png) |
| :--: |
| Melding van Hema |

De melding geeft duidelijk aan dat ik maar 3 van dit artikel kan bestellen waardoor ik als gebruiker snap waarom ik er maar 3 kan invullen in het aantal vak.

### Mogelijke aanpassingen voor mijn Appilicatie

#### Wat vindt het testpanel van Mogelijke opties?
## Hoe laat je winkelwageninhoud het best zien?
### hoe doen andere het?
#### Coolblue
#### Bol.com
#### Etrias
#### Hema
### Mogelijke aanpassingen voor mijn Appilicatie
#### Wat vindt het testpanel van Mogelijke opties?
## Conclusie
## bronnen
