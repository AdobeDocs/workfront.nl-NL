---
content-type: api
navigation-topic: general-api
title: De API Explorer gebruiken
description: De API Explorer gebruiken
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# De API Explorer gebruiken

Wanneer u de Adobe Workfront Core API gebruikt, is de API Explorer een verouderd naslagprogramma waarmee de relaties tussen ondersteunde bronnen, parameters en variabelen worden gecatalogiseerd.

## Open de API Explorer:

1. Gebruik Webbrowser om aan de [&#x200B; API Ontdekkingsreiziger &#x200B;](https://developer.adobe.com/workfront/api-explorer/) te navigeren\
   ![&#x200B; ga aan API Ontdekkingsreiziger &#x200B;](assets/mceclip1-350x149.png)

1. In het hogere recht van de API Ontdekkingsreiziger, selecteer de gewensteWorkfront **API Versie**, door gebrek wordt de huidigste versie automatisch geselecteerd
1. Het **gebied van de Filter**, kan worden gebruikt om de voorwerpen te filtreren die door naam worden vermeld en zal de lijst van dienovereenkomstig getoonde voorwerpen beknotten:

   ![&#x200B; API de gebieden van de Ontdekkingsreiziger &#x200B;](assets/mceclip2-350x147.png)

   * **Gebieden**: Beschikbare gebieden binnen het gespecificeerde voorwerp.
   * **Verwijzingen**: Beschikbare verwijzingsvariabelen voor het gespecificeerde voorwerp. Een verwijzing is een alias voor een variabele. Na initialisatie kan een verwijzing worden gebruikt met de variabelenaam. Een verwijzing gebruikt geïnitialiseerd geheugen.
   * **Inzamelingen**: Beschikbare inzamelingen voor het voorwerp. Verzamelingen zijn variabelen die een een-op-een relatie tussen het object en de bron vertegenwoordigen.
   * **Onderzoek**: Beschikbare onderzoeksmiddelen voor het voorwerp. De resultaten van een onderzoek zijn gebaseerd op de vraagparameters die door het onderzoeksmiddel in het API verzoek worden gespecificeerd.
   * **Acties**: De gesteunde acties voor het voorwerp. Handelingen kunnen eenvoudige of complexe procedures zijn die worden uitgevoerd met behulp van een bron of een reeks bronnen. Een bepaalde actie kan ook gevolgen hebben voor de bijbehorende middelen.

1. Open een tabblad en klik vervolgens op Object-id om de toepasselijke variabelen weer te geven.\
   ![&#x200B; variabelen van de Mening &#x200B;](assets/approval-350x89.png)\
   Afhankelijk van het geselecteerde object kunnen de volgende variabelen worden toegepast:

   | Variabele | Definitie |
   |---|---|
   | Veldnaam | De naam van een veld dat wordt gebruikt in een bewerking binnen de Workfront API. |
   | Veldtype | Het type waarden dat in een specifiek veld in een gegevenstabel kan worden ingevoerd. Mogelijke veldtypewaarden zijn string, double, int, dateTime. |
   | Opsommingstype | Het type waarden dat kan worden gebruikt om een gegevenstype te identificeren. |
   | Mogelijke waarden | Acceptabele waarden voor het object. |
   | Kenmerktype ObjCode | Kenmerken die kunnen worden gebruikt om de objectklasse te wijzigen. |
   | URL | Het ingangspad waarmee uw toepassing kan communiceren met de Workfront API. |
   | Argumenten | De objectvariabelen die tussen de toepassing en Workfront kunnen worden doorgegeven. |
   | Resultaattype | Toegestane gegevenstypen die door een methode kunnen worden geretourneerd. |
