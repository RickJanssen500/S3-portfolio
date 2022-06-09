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
Om mij hier verder in te verdiepen heb ik voor beide sites een account aangemaakt.   
en ben ik hier in de development omgeving naar verschillende aspecten gaan kijken die ik in de komende kopjes verer zal toelichten.

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
In het menu voor SSO en "social login koppelen" kun je veel varianten kiezen en toevoegen.   
alle bekende/groote sties staan hierin(oa Goolge, facebook, twitter, twitch, miscrosoft).   
en moacht je nou nogsteeds de door jouw gewenste login site er niet bij zien staan kun je er ook nog voor kiezen om er handmatig
een toetevoegen die niet standaard in Auth0 valt.   
Conclusie de mogelijkheden zijn bijna eideloos aangezien je zelf ook je eigen sites hieraan kan toevoegen
en het standaard pakket is zeel uitgebreid.   

## FusionAuth   
op de site zeggen ze wel dat het mogelijk is.   
Hier staan namelijk voordbeelden waar een knop met "login in met google" te zien is.   
echter kan ik in het dashboard en alle instellingen hier niks over vinden.
Wel geven ze aan Dat je FusionAuth bij een ander login systeem als sso kan zetten,
en geven ze je de credentials hier voor.
Conclusie Het is niet mogelijk om sso toe te voegen aan FusionAuth, maar je kunt FusionAuth wel ergens anders toevoegen als sso.

# Is er multi factor authentication?   
Voor de veligheid is het belangrijk dat als iemand je wachtwoord heeft ze niet zomaar bij je data kunnen.   
Om dit tegen tegaan is er MFA, waarbij de gebruiker naast zijn wachtwoord ook nog een verificatie code moet invullen.   
Deze code kan de gebruiker op verschilledne manieren krijgen bijvoordbeeld d.m.v. codegenerator app, sms, mail of een telefoongesprek.   
Deze code kan maar een keer gebruikt worden, de gebruiker zal dus elke keer dat hij wil inloggen een nieuwe code aanvragen.   
Omdat dit voor de gebruiker vervelend kan zijn om dit te doen wil je het voor de gebruiker zo makkelijk mogelijk maken door veel varianten te bieden.   
Dit zodat de gebruiker zelf kan kiezen welke variant hij hiervoor gebruikt.
## Auth0   
Auth0 bied 8 verschillende manieren van MFA.   
Hiernaast bieden ze ook de mogelijkheid om aan te geven hoevaak er MFA gevruikt word.   
Bijvoordbeeld alleen bij verdacthe inlog pogingen or bij alle inlog pogingen.

| ![image](https://user-images.githubusercontent.com/84378377/172625887-a1e8ca5f-a448-4d2f-92b2-0ce9e4b81830.png) | 
| :--: |
| _MFA functie Auth0_ | 

## FusionAuth   
In het dashboard zit een kopje met MFA, hieronder kun je de multi factor authenticatie toevoegen.   
Helaas is hier maar een optie, gebruik maken ven een authenticator app.

| ![image](https://user-images.githubusercontent.com/84378377/172623029-88aff630-61fc-4928-af5d-d38c41fcfc08.png) | 
| :--: |
| _MFA functie FusionAuth_ | 

# Rol verdelingen?   
Naast authenticatie is autorisatie ook belangrijk om de veiligheid van de app te kunnen garanderen.   
Zo wil je niet dat iedere gebruiker management taken kan uit voeren als het toevoegen en verwijderen van producten/verwerken van bestellingen.   
Deze taken moeten alleen uitgevoerd worden door een admin of een picker, maar niet door een Normale gebruiker die iets wil bestellen.   
Omdat je hier meerdere rollen hebt moet het makkelijk zijn om een gebruiker een rol te geven en evt aanvullende permissies.
Om zo te zorgen dat ze de juiste rechten hebben.
## Auth0   
Je kunt zelf verschillende rollen maken. Je kunt er hiervan zoveel maken als je zelf wilt en per rol zelf alle permissies instellen.   
Ook kun je per gebruiker permissies instellen, zo kun je een gebruiker een paar extra premissies geven naast hun rol. of juist minder rechten geven.   

## FusionAuth  

   
# Conclusie   
