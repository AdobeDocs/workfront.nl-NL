---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook'
description: Als u een outlookIdentityToken fout wanneer het gebruiken van Workfront voor Vooruitzichten krijgt, moet u Microsoft 365 erfenistokens voor uw organisatie toelaten.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Problemen oplossen: outlookIdentityToken-fout bij gebruik van Workfront for Outlook

>[!IMPORTANT]
>
>[ Microsoft is in het proces om steun voor de online tokens van de erfenisUitwisseling ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) onbruikbaar te maken, die momenteel door de toe:voegen-binnen van Workfront Vooruitzichten voor authentificatie worden gebruikt. Deze verandering door Microsoft is al begonnen met gevolgen voor de klanten en zal tot oktober 2025 in fasen blijven doorlopen.
>
>* **nadat Microsoft volledig deze tokens onbruikbaar maakt, zal Workfront voor de integratie van Microsoft Outlook niet meer functioneren.**
>
>Als onderdeel van deze wijziging heeft Microsoft besloten om de manier te wijzigen waarop tokens opnieuw worden ingeschakeld. Na **Juni 30, 2025**, zullen de beheerders niet meer tokens kunnen re-toelaten zelf-slechts de Steun van Microsoft kan uitzonderingen verlenen. **Op 1 Oktober, 2025, zullen de erfenistokens voor alle huurders worden uitgezet. Er worden geen uitzonderingen toegestaan.**


Als u Workfront for Outlook gebruikt, wordt mogelijk de volgende fout weergegeven:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Om deze fout op te lossen, moet u Microsoft 365 oudere tokens voor uw organisatie toelaten. Omdat dit moet gebeuren in Microsoft 365, kan Workfront deze tokens niet inschakelen voor uw organisatie.

Voor instructies bij het toelaten van Microsoft 365 erfenistokens, zie [ Online tokens van de Verouderde Uitwisseling van de Draai ](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in de documentatie van Microsoft.

Voor meer informatie over erfenistokens, zie [ Kan ik Uitwisseling Online erfenistokens terug draaien?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in de documentatie van Microsoft.
