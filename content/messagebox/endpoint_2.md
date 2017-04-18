+++
title = "[GET] /api/v1/{accountName}/{boxName}/messages/{messageId}/content"
weight = 30
+++

Dit end-point wordt gebruikt om de daadwerkelijke berichten inhoud op te halen.

De response geeft de rauwe bericht content terug, en hangt dus af van de `content_type`.
In sommige gevallen een text response, in anderen een PDF bijvoorbeeld.

Na ophalen van de content wordt bij de eerste keer automatisch de `seen_at` van dit bericht gezet
naar datum+tijd van dat moment.
