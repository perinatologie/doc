+++
toc = true
weight = 5
title = "Resources"
+++



## Resources
Op de Hub kunnen accounts (Organizations en Users) “Resources” aanmelden op de Hub. Vervolgens kunnen deze resources worden gedeeld met andere Hub Accounts.

## Resource types
Elke Resource heeft een Resource Type. Het Type geeft aan wat voor soort Resource het betreft. Aanmelders zijn vrij te bepalen welke typen ze aanmelden, maar samenwerkende partijen kunnen afspraken maken over welke typen ze ondersteunen.
Resource typen: perinatologie/dossier en hub/dossier
Het eerste Resource Type waarvoor deze afspraken zijn gemaakt via het Perinatologie.nl platform is het type “perinatologie/dossier”, wat een zwangerschaps dossier beschrijft. De opvolger hiervan is het type “hub/dossier”. Deze is met betrekking tot resource eigenschappen identiek.

Deze resources bevatten de volgende eigenschappen:

Zwangerschap gerelateerde elementen:

* **reference**: Unieke referentie voor een zwangerschap van 1 client
* **gravida**: De graviditeit van de zwangerschap
* **para**: De pariteit van de zwangerschap
* **start_at**: intake datum bij de provider
* **end_at**: eind datum indien van toepassing
* **edd**: Aterme datum


Client gerelateerde elementen:

* **client_displayname**: Volledige client naam
* **client_bsn**: Burger Service Nummer van de client.
* **client_birthdate**: Geboortedatum van de client


Automatische elementen:

* **registered_at**: Aanmeld datum op de hub
* **provider_accountname**: account naam van de provider


## Resource shares
Een aangemelde Resource kan via de Hub gedeeld worden met andere Hub Accounts.

Enkele voorbeelden:

Een verloskundige praktijk (organization account) kan een dossier (resource type peri/dossier) delen met een ziekenhuis (organization account).
Een ziekenhuis (organization account) kan een dossier (resource type peri/dossier) delen met verschillende verloskundige praktijken (organization accounts) in de regio.
Een verloskundige praktijk (organization account) kan een dossier delen met een client (user account).
Een client (user account) kan haar eigen dossier delen met een huisartsenpraktijk (organization account).
Een verloskundige praktijk (organization account) kan een dossier delen met een kraamzorg buro (organization account).
… etc

Een Resource kan gedeeld worden met een of meerdere andere accounts. Hetzelfde dossier kan dus zowel gedeeld worden met bijvoorbeeld een ziekenhuis, een kraamzorg buro als een client.

Een resource heeft altijd 1 Provider. De Provider is het account welke de resource heeft aangemeld op de hub, en is daarmee eigenaar van het dossier. Andere accounts waarmee de resource is gedeeld kunnen de data van deze resource opvragen bij de Provider mbv een “token” welke wordt uitgegeven door de Hub.

Een Provider kan Resources delen door tijdens de aanmelding een lijst van Identifiers en Identifier Types mee te geven zodat de Hub kan achterhalen om welke accounts het gaat. Geldige Identifier Types zijn bijvoorbeeld accountNames, AGB codes of accountUuids.


## Resource providers:

Organisaties die resources op de PeriHub aanmelden zijn de Provider van deze resource. Tijdens aanmelding geven Providers slechts een beperkte hoeveelheid ‘meta-data’ door aan de Hub (zie Resource Types). De PeriHub bevat niet de daadwerkelijke bron-data van een bepaalde resource, alleen de data die van toepassing is op het Resource Type.

Om de bron-data te verkrijgen bevraagt de aanvrager eerst de Hub. De Hub geeft de meta-data van de zoekresultaten terug zoals deze bekend zijn in de hub. Daarnaast bevat het zoekresultaat informatie die de bevrager kan gebruiken om direct bij de Provider van het Resource de bron-data op te vragen.

De Hub bevat op deze manier nooit de volledige informatie, en de bevrager krijgt altijd de meest actuele data terug precies zoals deze op dat moment is vastgelegd bij de Provider.
