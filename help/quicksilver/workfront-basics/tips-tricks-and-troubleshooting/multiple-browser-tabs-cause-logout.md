---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Door meerdere browsertabbladen kan Workfront zich afmelden
description: Wanneer een gebruiker meerdere browsertabbladen heeft geopend, kan Workfront zich automatisch afmelden.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# Door meerdere browsertabbladen kan Workfront zich afmelden

>[!IMPORTANT]
>
>Dit probleem is alleen aanwezig voor organisaties die aan Adobe IMS zijn aangemeld.

## Probleem

Wanneer een gebruiker meerdere browsertabbladen heeft geopend en op een tabblad klikt dat al enige tijd inactief is, is de tabsessie verlopen. De gebruiker kan de geopende pagina niet zien en ziet in plaats daarvan het volgende bericht:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Reden

Dit gedrag is toe te schrijven aan beleid-Gebaseerde Authentificatie (PBA), een veiligheidsmaatregel die door uw organisatie wordt gevormd. Wanneer een lusje voor meer dan de tijdslimiet die in de configuratie van PBA van uw organisatie wordt geplaatst inactief is geweest, verloopt de lusjezitting.

## Oplossing

De oplossing hangt af van het feit of u actief bent geweest op een ander tabblad dat is aangemeld bij Workfront.

* Als u een actief Workfront-tabblad hebt geopend, laadt u het verlopen tabblad opnieuw. De pagina wordt weergegeven op de pagina die u had geopend voordat deze verstreek.

* Als u geen actief Workfront-tabblad hebt geopend, meldt u zich opnieuw aan bij Workfront.
