+++
toc = true
weight = 15
title = "Resources registreren"
+++

Een Provider kan een nieuw resource aanmelden op de Hub ovv het Resource Type en aanvullende meta-data (Resource Properties) zoals bijvoorbeeld `client_bsn`, `gravida`, etc.

Tegelijkertijd bevat de aanmelding een lijst van [Resource Shares](/architectuur/resources/#resource-shares): Een lijst van identifiers van accounts waarmee het Resource gedeeld moet worden. Als Identifiers kunnen verschillende Identifier Types worden meegestuurd waarmee de Hub de accounts kan vinden. Veelal is dit een accountName, accountUuid of AGB code.

Elk Hub Account kan meerdere Identifiers bevatten waardoor deze gevonden kunnen worden.
