---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Aangepaste velden maken en beheren in  [!DNL Workfront Proof]
description: Een Uitgezochte of Premium  [!DNL Workfront]  Plan wordt vereist om deze eigenschap te gebruiken. Raadpleeg de plannen van Workfront voor meer informatie over de verschillende beschikbare plannen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: 6e6cc1db8f89b76d9903905e6ee4cf9014727ba1
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Aangepaste velden maken en beheren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [ het Bewijzen ](../../../review-and-approve-work/proofing/proofing.md).

U hebt een abonnement op Selecteren of Premium [!DNL Workfront] nodig om deze functie te kunnen gebruiken. Voor meer informatie over de diverse beschikbare plannen, zie [ Abonnementen van Workfront ](https://www.workfront.com/plans).

Met aangepaste velden kunt u aanvullende gegevens vastleggen wanneer u een nieuwe proefdruk, een nieuwe gebruiker of een nieuwe gast maakt.

Gebruikers die bijvoorbeeld een nieuwe proefdruk maken, willen mogelijk een extra sectie toevoegen waarmee ze een taaknummer, afdelingscode of leverancierverwijzing kunnen vastleggen.

>[!NOTE]
>
>* Als u dit type gegevens via Aangepaste velden op de pagina Nieuwe proefdruk vastlegt, kunt u ook de lengte van de proefdruknaam verminderen, aangezien deze gegevens niet in de naam hoeven te worden opgenomen. Zie &quot;Proefdrukken maken in [!DNL Workfront Proof]&quot; voor informatie over de pagina Nieuwe proefdrukken.
>
>Als een veld Aangepast eenmaal is gebruikt voor een proefdruk, gebruiker of contactpersoon, kunt u het veld niet verwijderen of het veldtype bewerken. U kunt de afbeelding echter wel verbergen (via de pagina [!UICONTROL Custom field Settings] ), zodat deze niet wordt gebruikt voor nieuwe items.
>
>Als u een sectie van het gebied van de Douane verborgen maakt, zullen alle gebieden binnen de sectie ook worden verborgen zelfs als de individuele gebieden als zichtbaar worden geplaatst.

In dit artikel wordt uitgelegd hoe u het volgende kunt doen:

## Aangepaste velden maken

Eerst moet u de sectie Aangepast veld instellen waaraan u aangepaste velden wilt toevoegen.

1. Klik **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**, dan open het **[!UICONTROL Custom fields]** lusje.

1. Klik op **[!UICONTROL Add custom field section]** in de betreffende module (Proef, Gebruikers of Contactpersonen).
1. Typ a **Naam** voor de sectie van het douanegebied, dan klik **[!UICONTROL Save]**.

   Nu kunt u aangepaste velden instellen in de sectie:

1. Klik op het tabblad **[!UICONTROL Custom fields settings]** om de pagina te vernieuwen.
1. Klik op de naam van de nieuwe sectie met aangepaste velden om de pagina **[!UICONTROL Custom field]section** voor de nieuwe sectie te openen.
1. Klik op **[!UICONTROL New custom field]** in de buurt van de rechterbovenhoek.
1. Geef op de pagina **[!UICONTROL New custom field]** die wordt weergegeven de details voor het aangepaste veld op:

   | **Verplicht** | Workfront vereist dat gebruikers het veld invullen. |
   |---|---|
   | **Doorzoekbaar** | Hiermee kunnen gebruikers items zoeken in het veld Aangepast. |
   | **Verborgen** | Verbergt het aangepaste veld op de pagina&#39;s [!UICONTROL New proof] , New gast en [!UICONTROL New user] |

   {style="table-layout:auto"}

1. Klik op **[!UICONTROL Save]**.
1. Op het **gebied van de Douane** pagina die verschijnt, klik het **[!UICONTROL Custom fields settings]** lusje om de pagina te verfrissen.

1. Wijzig desgewenst de instellingen voor het veld:

   * U kunt de sectie van het aangepaste veld verbergen of de verbergen door te klikken op het menu **[!UICONTROL More]** (drie punten) rechts van de naam van de aangepaste veldsectie en vervolgens te klikken op **[!UICONTROL Hide section]** of **[!UICONTROL Unhide section]** .

   * Verberg of maak de verbergen van het aangepaste veld ongedaan door te klikken op het menu **[!UICONTROL More]** (drie punten) rechts van de naam van de aangepaste veldsectie en vervolgens te klikken op **[!UICONTROL Hide custom field]** of **[!UICONTROL Unhide custom field]** .

   * Wijzig de volgorde van de velden met de pijlen omhoog en omlaag die rechts van de naam worden weergegeven (als u meerdere velden hebt toegevoegd aan een sectie).

1. Open de tab **[!UICONTROL Visibility rules]** .\
   Met zichtbaarheidsregels kunt u bepalen welke aanvullende velden worden weergegeven op basis van de voltooiing van het oorspronkelijke veld Aangepast. Als het afhankelijke veld bijvoorbeeld A is en het veld voor besturing X is, betekent dit dat veld A alleen zichtbaar is als veld X is ingevuld.

   U kunt besturingselementwaarden gebruiken om de waarden in het besturingsveld te bepalen. Als u deze waarde selecteert, wordt het afhankelijke veld zichtbaar. Stel bijvoorbeeld dat het afhankelijke veld A is en dat het besturingsveld X is en dat u de besturingselementwaarden in X alleen instelt op opties 1 en 2. Dit betekent dat veld A alleen zichtbaar is als veld X optie 1 of 2 is geselecteerd. Dit betekent dat als veld X-opties 3 of 4 is geselecteerd, veld A niet wordt weergegeven. Open de tab **[!UICONTROL Visibility rules]** .

   >[!NOTE]
   >
   >Alleen aangepaste veldtypen Lijst en Radio kunnen worden gebruikt voor het besturingsveld in een zichtbaarheidsregel, terwijl het afhankelijke veld elk veldtype kan zijn.

   Een zichtbaarheidsregel toevoegen:

   1. Klik op **[!UICONTROL New visibility rule]** voor de module waaraan u de regel wilt toevoegen.
   1. Selecteer de instellingen die u voor de regel wilt gebruiken en klik op **[!UICONTROL Save]** .

1. Open de tab **[!UICONTROL Dependency rules]** .

   Met de regels voor afhankelijkheid kunt u bepalen welke opties beschikbaar zijn in het afhankelijke veld wanneer bepaalde opties zijn geselecteerd in het beheerveld. Als het afhankelijke veld bijvoorbeeld &quot;B&quot; is en het besturingsveld &quot;Y&quot;, kunt u het als volgt instellen:

   Als optie 1 in veld Y wordt gekozen, worden alleen opties 1 en 2 in veld B weergegeven.

   Als optie 2 in veld Y wordt gekozen, worden alleen opties 3 en 4 in veld B weergegeven.

   >[!NOTE]
   >
   >Alleen aangepaste veldtypen Lijst en Radio kunnen worden gebruikt voor afhankelijke en beheerste velden in een afhankelijkheidsregel.

   Om een gebiedsdeelregel toe te voegen:

   1. Klik op **[!UICONTROL New dependency rule]** voor de module waaraan u de regel wilt toevoegen.
   1. Selecteer de gewenste instellingen voor de afhankelijkheid en klik op **[!UICONTROL Save]** .

## Aangepaste velden beheren

U kunt de details van de sectie Aangepast of afzonderlijke aangepaste velden weergeven en bewerken.

1. Klik **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]**, dan open het **[!UICONTROL Custom fields]** lusje.

1. Klik op de naam van de sectie van het aangepaste veld of het afzonderlijke aangepaste veld.
1. (Voorwaardelijk) Als u een sectie van het douanegebied beheert, breng om het even welke volgende veranderingen in de **[!UICONTROL Custom field section]** pagina aan:

   * Bewerk de naam van de sectie.
   * Verplaats het naar een andere module.
   * De sectie verbergen/tonen.

1. (Voorwaardelijk) Als u een aangepast veld beheert, brengt u een van de volgende wijzigingen aan op de pagina **[!UICONTROL Custom field]** :

   * Het veld naar een andere sectie verplaatsen.
   * Bewerk de naam van het veld.
   * InvoerHelp-tekst (er verschijnt een vraagtekenpictogram naast de veldsectie en de tekst verschijnt als u de muisaanwijzer op de tekst plaatst).
   * De instelling **[!UICONTROL Mandatory]** in-/uitschakelen in het veld.
   * De instelling **[!UICONTROL Searchable]** in-/uitschakelen in het veld.
   * Verberg/maak het veld zichtbaar.
   * Bewerk het veldtype.
   * Een standaardwaarde voor het veld instellen/bewerken.
   * Stel zichtbaarheids- en afhankelijkheidsregels in (zoals hierboven beschreven in de stappen 11 en 12).
