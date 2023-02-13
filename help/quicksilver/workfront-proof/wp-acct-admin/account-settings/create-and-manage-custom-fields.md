---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Aangepaste velden maken en beheren in [!DNL Workfront Proof]
description: Een Select- of Premium-bestand [!DNL Workfront] U moet een abonnement nemen om deze functie te kunnen gebruiken. Raadpleeg de plannen van Workfront voor meer informatie over de verschillende beschikbare plannen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '918'
ht-degree: 0%

---

# Aangepaste velden maken en beheren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Een Select- of Premium-bestand [!DNL Workfront] U moet een abonnement nemen om deze functie te kunnen gebruiken. Voor meer informatie over de verschillende beschikbare plannen raadpleegt u [Workfront-plannen](https://www.workfront.com/plans).

Met aangepaste velden kunt u aanvullende gegevens vastleggen wanneer u een nieuwe proefdruk, een nieuwe gebruiker of een nieuwe gast maakt.

Gebruikers die bijvoorbeeld een nieuwe proefdruk maken, willen mogelijk een extra sectie toevoegen waarmee ze een taaknummer, afdelingscode of leverancierverwijzing kunnen vastleggen.

>[!NOTE]
>
>* Als u dit type gegevens via Aangepaste velden op de pagina Nieuwe proefdruk vastlegt, kunt u ook de lengte van de proefdruknaam verminderen, aangezien deze gegevens niet in de naam hoeven te worden opgenomen. Zie &quot;Proefdrukken maken in [!DNL Workfront Proof].&quot;
>
>Als een veld Aangepast eenmaal is gebruikt voor een proefdruk, gebruiker of contactpersoon, kunt u het veld niet verwijderen of het veldtype bewerken. U kunt de afbeelding echter verbergen (via de [!UICONTROL Custom field Settings] pagina), zodat deze niet wordt gebruikt voor nieuwe items.
>
>Als u een sectie van het gebied van de Douane verborgen maakt, zullen alle gebieden binnen de sectie ook worden verborgen zelfs als de individuele gebieden als zichtbaar worden geplaatst.

In dit artikel wordt uitgelegd hoe u het volgende kunt doen:

## Aangepaste velden maken

Eerst moet u de sectie Aangepast veld instellen waaraan u aangepaste velden wilt toevoegen.

1. Klikken **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]** en open vervolgens de **[!UICONTROL Custom fields]** tab.

1. Klikken **[!UICONTROL Add custom field section]** in de relevante module (Proef, Gebruikers, of Contacten).
1. Typ a **Naam** voor de sectie van het douaneveld, dan klik **[!UICONTROL Save]**.

   Nu kunt u aangepaste velden instellen in de sectie:

1. Klik op de knop **[!UICONTROL Custom fields settings]** om de pagina te vernieuwen.
1. Klik op de naam van de nieuwe sectie met aangepaste velden om het dialoogvenster **[!UICONTROL Custom field]sectie** pagina voor de nieuwe sectie.
1. Klik op de knop **[!UICONTROL New custom field]** in de rechterbovenhoek.
1. In de **[!UICONTROL New custom field]** Geef de details voor het aangepaste veld op op de pagina die wordt weergegeven:

   | **Verplicht** | Workfront vereist dat gebruikers het veld invullen. |
   |---|---|
   | **Doorzoekbaar** | Hiermee kunnen gebruikers items zoeken in het veld Aangepast. |
   | **Verborgen** | Hiermee verbergt u het aangepaste veld op het tabblad [!UICONTROL New proof], Nieuwe gast, en [!UICONTROL New user] pagina&#39;s |

   {style=&quot;table-layout:auto&quot;}

1. Klik op **[!UICONTROL Save]**.
1. In de **Aangepast veld** pagina die wordt weergegeven, klikt u op de knop **[!UICONTROL Custom fields settings]** om de pagina te vernieuwen.

1. Wijzig desgewenst de instellingen voor het veld:

   * De sectie van het douanegebied van de huid of unhide door te klikken **[!UICONTROL More]** (drie punten) rechts van de naam van de aangepaste veldsectie en klikt u vervolgens op **[!UICONTROL Hide section]** of **[!UICONTROL Unhide section]**.

   * Verberg of maak de verbergen van het aangepaste veld ongedaan door op de knop **[!UICONTROL More]** (drie punten) rechts van de naam van de aangepaste veldsectie en klikt u vervolgens op **[!UICONTROL Hide custom field]** of **[!UICONTROL Unhide custom field]**.

   * Wijzig de volgorde van de velden met de pijlen omhoog en omlaag die rechts van de naam worden weergegeven (als u meerdere velden hebt toegevoegd aan een sectie).

1. Open de **[!UICONTROL Visibility rules]** tab.\
   Met zichtbaarheidsregels kunt u bepalen welke aanvullende velden worden weergegeven op basis van de voltooiing van het oorspronkelijke veld Aangepast. Als het afhankelijke veld bijvoorbeeld A is en het veld voor besturing X is, betekent dit dat veld A alleen zichtbaar is als veld X is ingevuld.

   U kunt besturingselementwaarden gebruiken om de waarden in het besturingsveld te bepalen. Als u deze waarde selecteert, wordt het afhankelijke veld zichtbaar. Stel bijvoorbeeld dat het afhankelijke veld A is en dat het besturingsveld X is en dat u de besturingselementwaarden in X alleen instelt op opties 1 en 2. Dit betekent dat veld A alleen zichtbaar is als veld X optie 1 of 2 is geselecteerd. Dit betekent dat als veld X-opties 3 of 4 is geselecteerd, veld A niet wordt weergegeven. Open de **[!UICONTROL Visibility rules]** tab.

   Een zichtbaarheidsregel toevoegen:

   1. Klikken **[!UICONTROL New visibility rule]** voor de module waar u de regel wilt toevoegen.
   1. Selecteer de gewenste instellingen voor de regel en klik op **[!UICONTROL Save]**.

1. Open de **[!UICONTROL Dependency rules]** tab.

   Met de regels voor afhankelijkheid kunt u bepalen welke opties beschikbaar zijn in het afhankelijke veld wanneer bepaalde opties zijn geselecteerd in het beheerveld. Als het afhankelijke veld bijvoorbeeld &quot;B&quot; is en het besturingsveld &quot;Y&quot;, kunt u het als volgt instellen:

   Als optie 1 in veld Y wordt gekozen, worden alleen opties 1 en 2 in veld B weergegeven.

   Als optie 2 in veld Y wordt gekozen, worden alleen opties 3 en 4 in veld B weergegeven.

   Om een gebiedsdeelregel toe te voegen:

   1. Klikken **[!UICONTROL New dependency rule]** voor de module wilt u de regel toevoegen.
   1. Selecteer de instellingen die u voor de afhankelijkheid wilt gebruiken en klik op **[!UICONTROL Save]**.

## Aangepaste velden beheren

U kunt de details van de sectie Aangepast of afzonderlijke aangepaste velden weergeven en bewerken.

1. Klikken **[!UICONTROL Settings]** >**[!UICONTROL Account Settings]** en open vervolgens de **[!UICONTROL Custom fields]** tab.

1. Klik op de naam van de sectie van het aangepaste veld of het afzonderlijke aangepaste veld.
1. (Voorwaardelijk) Als u een sectie van het douanegebied beheert, breng om het even welke volgende veranderingen in **[!UICONTROL Custom field section]** pagina:

   * Bewerk de naam van de sectie.
   * Verplaats het naar een andere module.
   * De sectie verbergen/tonen.

1. (Voorwaardelijk) Als u een aangepast veld beheert, wijzigt u een van de volgende opties in het dialoogvenster **[!UICONTROL Custom field]** pagina:

   * Het veld naar een andere sectie verplaatsen.
   * Bewerk de naam van het veld.
   * InvoerHelp-tekst (er verschijnt een vraagtekenpictogram naast de veldsectie en de tekst verschijnt als u de muisaanwijzer op de tekst plaatst).
   * Schakel de **[!UICONTROL Mandatory]** instellen op het veld.
   * Schakel de **[!UICONTROL Searchable]** instellen op het veld.
   * Verberg/maak het veld zichtbaar.
   * Bewerk het veldtype.
   * Een standaardwaarde voor het veld instellen/bewerken.
   * Stel zichtbaarheids- en afhankelijkheidsregels in (zoals hierboven beschreven in de stappen 11 en 12).
