# Welke login service kan ik het best gebruiken voor mijn api?
# Inhoudsopgave   
- [Welke login service kan ik het best gebruiken voor mijn api?](#welke-login-service-kan-ik-het-best-gebruiken-voor-mijn-api)
- [Inhoudsopgave](#inhoudsopgave)
- [Introductie](#introductie)
- [Een eerste gevoel](#een-eerste-gevoel)
- [Welke vormen van inloggen zijn er?](#welke-vormen-van-inloggen-zijn-er)
  * [Auth0](#auth0)
  * [FusionAuth](#fusionauth)
- [Is er multi factor authentication?](#is-er-multi-factor-authentication)
  * [Auth0](#auth0-1)
  * [FusionAuth](#fusionauth-1)
- [Rol verdelingen?](#rol-verdelingen)
  * [Auth0](#auth0-2)
  * [FusionAuth](#fusionauth-2)
- [Hoe integreren in app?](#hoe-integreren-in-app)
  * [Auth0](#auth0-3)
  * [FusionAuth](#fusionauth-3)
- [Conclusie](#conclusie)

# Introductie  
Voor mijn security onderzoek wist ik in eerste instantie niet wat ik hier voor moest kiezen.
Toen ik moest gaan kijken naar een login systeem zag ik dat er redelijk veel varianten waren.
Hierop besloot ik mijn onderzoek te deon over welke login service ik het best kan gebruiken voor mijn appilicatie.   
Dit zijn de login services waar ik naar ga kijken:
  - [Auth0](https://auth0.com/)
  - [FusionAuth](https://fusionauth.io/)
  - [OneLogin](https://developers.onelogin.com/)
  - [Okta](https://www.okta.com)
  - [Keycloak](https://www.keycloak.org/)   
  
Dit waren de eerste 5 zoek resultaten van google, voor de rest heb ik geen specifieke reden waarom ik deze gekozen heb. 

# Een eerste gevoel
Omdat ik 5 services veel vind heb ik ervoor gekozen om dit terug te dringen tot 2.
Op deze 2 zal ik me verder verdiepen.   
Om te kijken welke 2 ik ging kiezen heb ik er voor gekozen om te kijken naar de website.   
Ik gekeken naar welke website het betrouwbaarst overkomt en welke hierin een overzichtelijke pagina gaven.   
Auth0 heeft een betrouwbare en proffesioneel uitziende website, ook staan de features overzichtelijk bij elkaar.   
FusionAuth Geeft een heel overzichtelijk gevoel met goede voorbeelden op de site.   
Bij Keycloak voelt de website oud aan en presenteren ze hun features niet maar hebben ze alleen maar documentatie.   
OneLogin Maakt niet gebruik van de volle breede van het scherm, tevens hebben hun ook alleen documentatie.   
Okta geeft een betrouwbaar gevoel echter zijn de features niet echt overzichtelijk geplaatst en erg vol op elkaar gepropt.  
Dit heeft er voor gezorgd dat ik mij verder ga verdiepen in Auth0 en FusionAuth.

# Welke vormen van inloggen zijn er?
Er zijn vele manieren waarop je kunt inloggen, zo kun je bijvoordbeeld op meerdere platforms inloggen met je google account.
Of met een Key inplaatsvan een password.   
Mijn appilicatie is een webshop, hierin wil je het inloggen zo makkelijk mogelijk maken zodat klanten makkelijk iets kunnen iets bestellen.   
De login vormen die ik hier voor zoek zijn dus dat je met zoveel mogelijk verschillende services kan inloggen.   
Ook moet het inloggen makkelijk en overzichtelijk zijn zodat de klant hier makkeilijk doorheen gaat.
Ik heb voor de door mij gekozen services geken welke mogelijk heden zij hier in bieden.  

## Auth0   
Bij Auth0
## FusionAuth   

# Is er multi factor authentication?   
Voor de veligheid is het belangrijk dat als iemand je wachtwoord heeft ze niet zomaar bij je data kunnen.   
Om dit tegen tegaan is er MFA, waarbij de gebruiker naast zijn wachtwoord ook nog een verificatie code moet invullen.   
Deze code kan de gebruiker op verschilledne manieren krijgen bijvoordbeeld d.m.v. codegenerator app, sms, mail of een telefoongesprek.   
Deze code kan maar een keer gebruikt worden, de gebruiker zal dus elke keer dat hij wil inloggen een nieuwe code aanvragen.   
Omdat dit voor de gebruiker vervelend kan zijn om dit te doen wil je het voor de gebruiker zo makkelijk mogelijk maken door veel varianten te bieden.   
Dit zodat de gebruiker zelf kan kiezen welke variant hij hiervoor gebruikt.
## Auth0   
## FusionAuth   

# Rol verdelingen?   
Naast authenticatie is autorisatie ook belangrijk om de veiligheid van de app te kunnen garanderen.   
Zo wil je niet dat iedere gebruiker management taken kan uit voeren als het toevoegen en verwijderen van producten/verwerken van bestellingen.   
Deze taken moeten alleen uitgevoerd worden door een admin of een picker, maar niet door een Normale gebruiker die iets wil bestellen.   
Omdat je hier meerdere rollen hebt moet het makkelijk zijn om een gebruiker een rol te geven en evt aanvullende permissies.
Om zo te zorgen dat ze de juiste rechten hebben.
## Auth0
## FusionAuth   

# Hoe integreren in app?   
Naast dat de service voor authenticatie en autorisatie moet zorgen moet het voor developers ook makkelijk zijn om de service te inteplementer en te onderhouden.   
Zodat het toevoegen van extra/nieuwe veligigere manieren van inloggen en rechten makkelijk kan geboeren.   
Zodat de appilicatie altijd de maximale en moedernste beveiliging geniet.  

## Auth0
## FusionAuth   

# Conclusie   
