---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Aangepaste velden maken en beheren in  [!DNL Workfront Proof]
description: Een Uitgezochte of Premium  [!DNL Workfront]  Plan wordt vereist om deze eigenschap te gebruiken. Raadpleeg de plannen van Workfront voor meer informatie over de verschillende beschikbare plannen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Aangepaste velden maken en beheren in [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

U hebt een abonnement op Selecteren of Premium [!DNL Workfront] nodig om deze functie te kunnen gebruiken. Voor meer informatie over de diverse beschikbare plannen, zie [ Abonnementen van Workfront ](https://www.workfront.com/plans).

Met aangepaste velden kunt u aanvullende gegevens vastleggen wanneer u een nieuwe proefdruk, een nieuwe gebruiker of een nieuwe gast maakt. Gebruikers die bijvoorbeeld een nieuwe proefdruk maken, willen mogelijk een extra sectie toevoegen waarmee ze een taaknummer, afdelingscode of leverancierverwijzing kunnen vastleggen.

>[!NOTE]
>
>* Als u dit type gegevens via aangepaste velden op de pagina Nieuwe proefdruk vastlegt, kunt u ook de lengte van de proefdruknaam verminderen, aangezien deze gegevens niet in de naam hoeven te worden opgenomen.
>
>* Als een aangepast veld eenmaal is gebruikt voor een proefdruk, gebruiker of contactpersoon, kunt u het niet verwijderen of het veldtype bewerken. U kunt het bestand echter verbergen via de pagina Instellingen aangepast veld, zodat het niet wordt gebruikt voor nieuwe items.
>
>* Als u een aangepaste veldsectie verbergt, worden ook alle velden in de sectie verborgen, zelfs als de afzonderlijke velden zijn ingesteld als zichtbaar.

## Aangepaste velden maken

{{step1-to-proofing}}

1. In de hoger-juiste hoek van de pagina, klik **montages van de Rekening**.

1. Op de **pagina van de montages van de Rekening** selecteren de **gebieden van de Douane** tabel.

1. Klik **[!UICONTROL Add custom field section]** op de rechterkant van de module (**Bewijs**, **Gebruikers**, of **Contacten**) u het douanegebied aan wilt toevoegen. Het **lusje van de Details van de Sectie** opent.

1. Typ a **Naam** voor de sectie van het douanegebied, dan klik **[!UICONTROL Save]**.

1. Klik op het tabblad **[!UICONTROL Custom fields settings]** om de pagina te vernieuwen. De nieuwe sectie van het douanegebied toont onder zijn toegewezen module.

   ![ de montages tabel van de Douane gebieden ](assets/custom-field-settings-tab.png)

1. Klik de naam van uw nieuwe sectie van het douanegebied om de **sectie van de gebieden van de Douane** tabel te openen.

1. Klik rechtsboven op de pagina op de knop **[!UICONTROL New custom field]** . De **Nieuwe pagina van het douanegebied** verschijnt.

1. Specificeer de **details van het Gebied**:

   * **Naam**: Ga de naam van het douanegebied in.
   * **Hulp**: Ga hulptekst in die in tooltip zal tonen.
   * **Verplicht**: Controle dit vakje om de gebruiker te vereisen om het gebied te voltooien.
   * **Doorzoekbaar** (Voorwaardelijk): Controleer deze doos om het douanegebied doorzoekbaar te maken.
   * **Verborgen**: Controle dit vakje om het douanegebied op de **Nieuwe proef**, **Nieuwe gast**, en **Nieuwe gebruiker** pagina&#39;s te verbergen.

1. Specificeer het **type van Gebied** en details:

   * **Type**: Selecteer het type van douanegebied.
   * **de punten van de Lijst**: (Voorwaardelijk) voeg de lijstpunten toe die op het douaneveld zullen verschijnen.
   * **Standaardwaarde**: Selecteer de standaardwaarde voor dit douanegebied. Deze optie is afhankelijk van het geselecteerde aangepaste veldtype.

1. Klik op **[!UICONTROL Save]**.

1. Wijzig desgewenst de instellingen voor het veld:

   * Verberg of unhide de sectie van het douanegebied door **Meer** ![ ](assets/more-button-small.png) menu aan het recht van de naam van de de douaneveld sectiesectie te klikken **[!UICONTROL Hide section]** of **[!UICONTROL Unhide section]**.
   * Verberg of unhide het douaneveld door **Meer** ![ ](assets/more-button-small.png) menu aan het recht van de naam van de douaneveld sectiesectie te klikken, dan klikkend **[!UICONTROL Hide custom field]** of **[!UICONTROL Unhide custom field]**.
   * Wijzig de volgorde van de velden met de pijlen omhoog en omlaag die rechts van de naam worden weergegeven (als u meerdere velden hebt toegevoegd aan een sectie).

1. Klik op de tab **[!UICONTROL Visibility rules]** .

   Met zichtbaarheidsregels kunt u bepalen welke aanvullende velden worden weergegeven op basis van de voltooiing van het oorspronkelijke aangepaste veld. Als het afhankelijke veld bijvoorbeeld A is en het veld voor besturing X is, betekent dit dat veld A alleen zichtbaar is als veld X is ingevuld.

   U kunt besturingselementwaarden gebruiken om de waarden in het besturingsveld te bepalen. Als u deze waarde selecteert, wordt het afhankelijke veld zichtbaar. Stel bijvoorbeeld dat het afhankelijke veld A is en dat het besturingsveld X is en dat u de besturingselementwaarden in X alleen instelt op opties 1 en 2. Dit betekent dat veld A alleen zichtbaar is als veld X optie 1 of 2 is geselecteerd. Als veld X-opties 3 of 4 is geselecteerd, wordt veld A niet weergegeven.

   >[!NOTE]
   >
   >Alleen aangepaste veldtypen Lijst en Radio kunnen worden gebruikt voor het besturingsveld in een zichtbaarheidsregel, terwijl het afhankelijke veld elk veldtype kan zijn.

   Een zichtbaarheidsregel toevoegen:

   1. Klik op **[!UICONTROL New visibility rule]** voor de module waaraan u de regel wilt toevoegen.

   1. Selecteer de instellingen die u voor de regel wilt gebruiken en klik op **[!UICONTROL Save]** .

1. Open de tab **[!UICONTROL Dependency rules]** .

   Met de regels voor afhankelijkheid kunt u bepalen welke opties beschikbaar zijn in het afhankelijke veld wanneer bepaalde opties zijn geselecteerd in het beheerveld. Als het afhankelijke veld bijvoorbeeld &quot;B&quot; is en het besturingsveld &quot;Y&quot;, kunt u het als volgt instellen:

   * Als optie 1 in veld Y wordt gekozen, worden alleen opties 1 en 2 in veld B weergegeven.

   * Als optie 2 in veld Y wordt gekozen, worden alleen opties 3 en 4 in veld B weergegeven.

   >[!NOTE]
   >
   >Alleen aangepaste veldtypen Lijst en Radio kunnen worden gebruikt voor afhankelijke en beheerste velden in een afhankelijkheidsregel.

   Om een gebiedsdeelregel toe te voegen:

   1. Klik op **[!UICONTROL New dependency rule]** voor de module waaraan u de regel wilt toevoegen.

   1. Selecteer de gewenste instellingen voor de afhankelijkheid en klik op **[!UICONTROL Save]** .

## Aangepaste velden beheren

U kunt de details van de sectie Aangepast of afzonderlijke aangepaste velden weergeven en bewerken.

{{step1-to-proofing}}

1. In de hoger-juiste hoek van de pagina, klik **montages van de Rekening**.

1. Op de **pagina van de montages van de Rekening** selecteren de **gebieden van de Douane** tabel.

1. Klik op de naam van de sectie van het aangepaste veld of het afzonderlijke aangepaste veld.

1. (Voorwaardelijk) Als u een sectie van het douanegebied beheert, breng om het even welke volgende veranderingen in de **[!UICONTROL Custom field section]** pagina aan:

   * Bewerk de naam van de sectie.
   * Verplaats het naar een andere module.
   * De sectie verbergen/tonen.

1. (Voorwaardelijk) Als u een aangepast veld beheert, brengt u een van de volgende wijzigingen aan op de pagina **[!UICONTROL Custom field]** :

   * Het veld naar een andere sectie verplaatsen.
   * Bewerk de naam van het veld.
   * Help-tekst bewerken.
   * De instelling **[!UICONTROL Mandatory]** in-/uitschakelen in het veld.
   * (Voorwaardelijk) Schakel de instelling **[!UICONTROL Searchable]** in of uit op het veld.
   * Verberg/maak het veld zichtbaar.
   * Bewerk het veldtype.
   * Een standaardwaarde voor het veld instellen/bewerken.
   * Stel zichtbaarheids- en afhankelijkheidsregels in.
