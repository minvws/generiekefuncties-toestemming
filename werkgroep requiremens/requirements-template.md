# Context
Dit document bevat de (relevante) ingevulde hoofdstukken van de Volere requirements template.
Als basis is de Nederlandse versie van de [Volere Template v13](https://www.volere.org/wp-content/uploads/2018/12/template13_nl.pdf) gebruikt.

## Volere Requirements template
Meer informatie over de Volere template kan gevonden worden op de [Volere website](https://www.volere.org/templates/volere-requirements-specification-template/).

# 1. Het doel van het project
## 1a. business van de gebruiker of de achtergrond van de projectinspanning

Voordat het beroepsgeheim mag worden doorbroken moet er o.a. aan de toestemmingsvoorwaarde worden voldaan. We ontwerpen een functie die het vastleggen en gebruik van deze toestemmingen vereenvoudigd waardoor gegevensuitwisselingen ter behoeven van het primaire en secundaire proces kan worden opgeschaald.

## 1b. Doelen van het project
1. We willen dat de burger hun toestemmingsvoorkeuren eenvoudig kan beheren
2. We willen dat een gegevensverantwoordelijke eenvoudig kan vaststellen of er sprake is van een toestemming.

### Meetbaarheid:

Eenvoudig kunnen vastleggen betekent dat een groot deel van de bevolking deze voorkeuren heeft vastgelegd.
Kunnen gebruiken betekent dat een groot deel van de gegevensuitwisselingen gebruik maakt van de in de toestemmingsfunctie vastgelegde toestemmingsvoorkeuren.

## 2a. De opdrachtgever
VWS
## 2b. De klant
Nederland

## 2c. Andere belanghebbenden

1. Personen
2. Patienten
3. Zorgverleners
4. Zorgorganisaties
5. Onderzoekers
6. Verzekeraars
7. Ontwikkelaars van gegevensuitwisselingen
8. IT-leveranciers
9. Overheid / VWS
10. Koepels
11. Juridische experts
12. Domein experts
13. UX experts

# Gebruikers van het product
## 3a De praktijk gebruikers van het product

Gebruikersgroep | Rol | Prioriteit | Participatie
| --| -- | -- | -- |
Personen | Beheren van toestemmingsvoorkeuren | Hoofdgebruiker | Testen
Patienten| Beheren van toestemmingsvoorkeuren| Hoofdgebruiker| Testen
Zorgverlener|Vastleggen en gebruiken van toestemmingsvoorkeuren van patienten| Hoofdgebruiker| Input en testen
Zorgorganisaties|Informeren van de patient over het belang van het vastleggen van een toestemmingsvoorkeur. Het ontsluiten van bestaande toestemmingen. Het aansluiten op de landelijke toestemmingsfunctie. Het aansluiten op en implementeren van het afsprakenstelsel.| Nevengebruiker| Input via vertegenwoordiging
Onderzoekers| Het gebruiken van de toestemmingsvoorkeuren bij het verkrijgen van onderzoeksgegevens.| Nevengebruiker| Valideren
Ontwikkelaars van gegevensuitwisselingen| Het opnemen van de toestemmingsfunctie in de gegevensuitwisseling voor het vaststellen van de grondslag.| Nevengebruiker| Input en valideren
IT-leveranciers| Technisch aansluiten op de functie. Het lezen van de documentatie. Voldoen aan het afsprakenstelsel.| Nevengebruiker| Input| Beheerder van de functie. Het ondersteunen van de gebruikers van de functie. Het operationeel houden van de functie. Het doorontwikkelen van de functie.| Onbelangrijke gebruiker |  Geen
Implementators| Het implementeren van de functie bij zorginstellingen en onderzoeksinstellingen. Interacteren met de helpdesk van de functie.| Onbelangrijke gebruiker| Feedback tijdens gebruik

## 3b. Prioriteiten toegewezen aan gebruikers

Zie de kolom "Prioriteit" onder 3a.

## 3c. Participatie van de gebruikers
Zie kolom “Participatie” onder 3a.

# 4. Opgelegde beperkingen
## 4a. Beperkingen voor de oplossing
### 1. Gebruik van Mitz
**Beschrijving**: De functie moet worden ingevuld met het product Mitz

**Rationale**: De opdrachtgever (VWS) heeft Mitz gekozen als de landelijke voorziening voor het vastleggen van toestemmingsvoorkeuren

**Fitcriterium**: De requirements voor de kortetermijn moeten redelijkerwijze in Mitz ingebouwd kunnen worden.

## 4b. Implementatieomgeving van het huidige systeem
## 4c. Partnerapplicaties of samenwerkende applicaties
## 4d. Aankoopbare software
## 4e. Vooropgestelde werkplekomgeving
## 4f. Beperkingen op het plan

### Tijdlijn IZA
Het IZA schrijft voor data de functie eind 2026 operationeel moet zijn voor de geprioriteerde gegevensuitwisselingen.

**Impact**: Als deze datum niet wordt gehaald zullen deze uitwisselingen (waar relevant) geen gebruik kunnen maken van de toestemmingsfunctie. Dit kan als gevolg hebben dat er of een andere bron voor de uitwisselgrondslag moet worden gevonden, mat hoge kosten tot gevolg, of dat de IZA niet wordt gehaald, met politieke gevolgen voor de opdrachtgever.

## 4g. Budget Beperkingen
Het is onduidelijk wat het budget is voor het realiseren van de landelijke toestemmingsfunctie.

# 5. Naamgevingsconventies en definities

