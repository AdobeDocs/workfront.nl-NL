---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook'
description: Als u een outlookIdentityToken fout wanneer het gebruiken van Workfront voor Vooruitzichten krijgt, moet u Microsoft 365 erfenistokens voor uw organisatie toelaten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook

>[!IMPORTANT]
>
>[&#x200B; Microsoft heeft steun voor online tokens van de erfenisUitwisseling &#x200B;](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar gemaakt, die door toe:voegen-binnen van Workfront Outlook voor authentificatie werden gebruikt. Deze verandering door Microsoft werd in fasen doorgevoerd en is voltooid op 1 oktober 2025.
>
>**omdat Microsoft deze tokens heeft onbruikbaar gemaakt, werkt Workfront voor de integratie van Microsoft Outlook niet meer.**

Als u Workfront for Outlook gebruikt, wordt mogelijk de volgende fout weergegeven:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Om deze fout op te lossen, moet u Microsoft 365 oudere tokens voor uw organisatie toelaten. Omdat dit moet gebeuren in Microsoft 365, kan Workfront deze tokens niet inschakelen voor uw organisatie.

Voor instructies bij het toelaten van Microsoft 365 erfenistokens, zie [&#x200B; Online tokens van de Verouderde Uitwisseling van de Draai &#x200B;](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in de documentatie van Microsoft.

Voor meer informatie over erfenistokens, zie [&#x200B; Kan ik Uitwisseling Online erfenistokens terug draaien?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in de documentatie van Microsoft.
