+++
toc = true
weight = 35
title = "Tokens"
+++

Wanneer een account de PeriHub bevraagt dan zijn de zoekresultaten voorzien van een Token (JWT - JSON Web Token). Dit token kan de bevrager gebruiken om de bron-data bij de Provider van het Resource op te vragen.

Het Token is cryptografisch ondertekend met de private key van de Hub (middels RS512).

Door het Token door te geven aan de provider kan de provider mbv de public key van de Hub valideren dat het token daadwerkelijk is uitgegeven door de hub.

Het token bevat een beperkte geldigheidsduur waardoor de bron-data alleen vlak na bevraging kan worden opgehaald. Verder bevat het token enkele “claims” waardoor de provider kan controleren om welke data het specifiek gaat. Zo kan een token voor 1 resource niet gebruikt worden om andere resources bij dezelfde provider op te halen.

Meer informatie mbt JWT:

* [https://jwt.io](https://jwt.io)
