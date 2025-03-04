---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook'
description: Als u een outlookIdentityToken fout wanneer het gebruiken van Workfront voor Vooruitzichten krijgt, moet u Microsoft 365 erfenistokens voor uw organisatie toelaten.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 77cc1acde87b2ada96117daa06e98ba38e64fa8a
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook

Als u Workfront for Outlook gebruikt, wordt mogelijk de volgende fout weergegeven:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Om deze fout op te lossen, moet u Microsoft 365 oudere tokens voor uw organisatie toelaten. Omdat dit moet gebeuren in Microsoft 365, kan Workfront deze tokens niet inschakelen voor uw organisatie.

Voor instructies bij het toelaten van Microsoft 365 erfenistokens, zie [ Online tokens van de Verouderde Uitwisseling van de Draai ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in de documentatie van Microsoft.

Voor meer informatie over logacy tokens, zie [ Kan ik Uitwisseling Online erfenistokens terug draaien?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in de documentatie van Microsoft.
