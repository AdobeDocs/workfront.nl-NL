---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Systeemupdates configureren
description: Workfront genereert automatische systeemupdates in het [!UICONTROL Updates] -gebied van een object om de wijzigingen op te nemen die gebruikers op het object uitvoeren. Als a [!DNL Workfront]  beheerder, kunt u vormen welke objecten gebieden en acties  [!DNL Workfront]  sporen om systeemupdates te registreren.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 4fafdcea97874e791104260375617e3989af1870
workflow-type: tm+mt
source-wordcount: '887'
ht-degree: 0%

---

# Systeemupdates configureren

<!-- Audited: 6/2025 -->

<!--

<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

[!DNL Adobe Workfront] genereert automatische systeemupdates in het [!UICONTROL Updates] -gebied van een object om de volgende gebeurtenissen op te nemen:

* Wijzigingen aanbrengen in een objectveld
* Handelingen die gebruikers uitvoeren op een object

Deze systeemupdates bevatten het volgende type informatie:

* De aangebrachte wijziging
* De naam van de gebruiker die de wijziging heeft aangebracht
* Het tijdstip en de datum van de wijziging

Voor meer informatie over systeemupdates, zie [&#x200B; systeem-geleide updates &#x200B;](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] beheerder kunt u configureren welke objectvelden en handelingen [!DNL Workfront] bijhoudt om systeemupdates op te nemen.

U kunt bijvoorbeeld in [!DNL Workfront] alle wijzigingen bijhouden die gebruikers in de namen van problemen in het hele systeem doorvoeren. Elke wijziging in de naam van een uitgave wordt vervolgens weergegeven als een systeemupdate in het [!UICONTROL Updates] -gebied van de uitgave.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td><p>Nieuw: [!UICONTROL Standard]</p>
   of
   <p>Huidige: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

*For meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bepalen welke velden [!DNL Workfront] bijhoudt voor een objecttype

U kunt bepalen welke informatie [!DNL Workfront] bijhoudt wanneer gebruikers informatie wijzigen die aan een bepaald objecttype is gekoppeld in de gehele [!DNL Workfront] -interface. U doet dit door de velden toe te voegen of te verwijderen die u in [!DNL Workfront] wilt bijhouden voor dat objecttype.

>[!NOTE]
>
>* [!DNL Workfront] kan geen updates bijhouden en opnemen over berekende aangepaste velden.
>* U kunt de systeemupdate aanpassen voor projecten, taken, problemen, portfolio&#39;s, programma&#39;s en gebruikers. U kunt de systeemupdate niet aanpassen voor sjablonen, documenten of tijdbladen, maar [!DNL Workfront] registreert wel systeemupdates voor deze objecten.
>


### Velden toevoegen die u wilt bijhouden in [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

U kunt velden toevoegen die u in [!DNL Workfront] voor een bepaald type object wilt bijhouden via de [!DNL Workfront] -interface. Wanneer gebruikers gegevens in dat veld wijzigen, slaat [!DNL Workfront] informatie over de wijziging op als een systeemupdate in het [!UICONTROL Updates] -gebied voor het object.

>[!NOTE]
>
>U kunt maximaal 300 ingebouwde en aangepaste velden bijhouden in de updatefeed. Als u het maximumaantal velden bijhoudt en aanvullende velden wilt bijhouden die niet op het subtabblad [!UICONTROL All Fields] worden weergegeven, moet u eerst enkele bijgehouden velden verwijderen om nieuwe velden bij te houden. Voor meer informatie over het verwijderen van gebieden uit de updategebieden, zie [&#x200B; gebieden verwijderen u niet gevolgd &#x200B;](#remove-fields-you-don-t-want-tracked) wilt.

{{step-1-to-setup}}

1. Klik in het deelvenster aan de linkerkant op **[!UICONTROL Interface]** en vervolgens op **[!UICONTROL Update Feeds]** .
1. (Facultatief) op de **Getraceerde gebieden** tabel, klik één van de volgende subtabs, afhankelijk van welke types van gebieden u in de updatevervoer wilt volgen:

   * **Ingebouwde gebieden**: Toont een lijst van ingebouwde gebieden.
   * **de gebieden van de Douane**: Toont een lijst van douanevelden. U moet aangepaste velden maken voordat deze beschikbaar zijn in de lijst.
   * **Alle gebieden**: Toont een lijst van zowel ingebouwde als douanegebieden.

1. Klik op **[!UICONTROL Add fields]** en selecteer in het keuzemenu het object dat u wilt bijhouden.

   Het handmatig selecteren van velden is niet beschikbaar voor alle objecten met het gebied Updates.

   Selecteer een van de velden voor de volgende objecten:

   * Project
   * Taak
   * Probleem
   * Portfolio
   * Programma
   * Gebruiker

   **voegt gebieden** doos toe opent, voor elk geselecteerd voorwerp.
1. In **voeg gebieden** doos toe, begin of een ingebouwd (standaard) gebied of een douanegebied voor het voorwerp te typen, dan het te selecteren wanneer het in de lijst verschijnt.

   >[!NOTE]
   >
   >Als [!DNL Workfront] het veld al bijhoudt, kunt u het niet nogmaals toevoegen vanuit de lijst.

1. Nadat u alle velden hebt toegevoegd die u in [!DNL Workfront] wilt bijhouden, klikt u op **[!UICONTROL Add]** .
De ingebouwde velden die u hebt toegevoegd, worden weergegeven onder de subtab **[!UICONTROL Built-in fields]** en de aangepaste velden onder de subtab **[!UICONTROL Custom fields]** .
In de subtab **[!UICONTROL All fields]** worden zowel de ingebouwde als de aangepaste velden weergegeven die [!DNL Workfront] bijhoudt.

### Velden verwijderen die u niet wilt bijhouden {#remove-fields-you-don-t-want-tracked}

U kunt velden verwijderen die het systeem niet voor een bepaald type object hoeft bij te houden in de gehele interface van [!DNL Workfront] .

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Interface]** en vervolgens op **[!UICONTROL Update Feeds]** .

1. Selecteer op het tabblad **[!UICONTROL Tracked Fields]** de subtab **[!UICONTROL All fields]** . Zowel de ingebouwde als de aangepaste velden die momenteel worden bijgehouden, worden weergegeven.

1. Selecteer het gebied u het volgen wilt ophouden, dan klik het **[!UICONTROL Remove]** pictogram ![&#x200B; verwijderen pictogram &#x200B;](assets/remove-icon.png).

1. Klik in het vak **[!UICONTROL Remove Field]** dat wordt weergegeven op **[!UICONTROL Yes, Remove It]** om te bevestigen.

   Alle updates over de eerder bijgehouden velden blijven behouden in het [!UICONTROL Updates] -gebied waar ze zijn opgenomen.

## Bepalen welke handelingen [!DNL Workfront] bijhoudt voor een objecttype

U kunt [!DNL Workfront] handelingen bijhouden die gebruikers uitvoeren op objecten in de [!DNL Workfront] -interface.

U kunt bijvoorbeeld [!DNL Workfront] elke keer dat een gebruiker een toewijzing wijzigt in een taak of uitgave, een update laten opnemen.

De wijziging wordt dan weergegeven als een systeemupdate in het [!UICONTROL Updates] -gebied voor de taak of uitgave.

In de volgende tabel worden de acties beschreven die u kunt bijhouden op objecten in [!DNL Workfront] :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Actie </strong> </th> 
   <th><strong> Voorwerpen </strong> </th> 
   <th><strong> Standaardstatus </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Toewijzing gewijzigd</td> 
   <td>Taken, problemen</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Basislijn wordt verwijderd</td> 
   <td>Projecten</td> 
   <td> <p>Uitgeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Factureringsrecord wordt gemaakt of verwijderd</td> 
   <td>Projecten</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Document wordt gemaakt of verwijderd</td> 
   <td>Projecten, taken, problemen, portfolio's, programma's</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Kosten worden gemaakt of verwijderd</td> 
   <td>Projecten, taken</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Uur is vastgelegd of verwijderd</td> 
   <td>Projecten, taken, problemen</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Probleem is verwijderd</td> 
   <td>Projecten</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Taak wordt verwijderd</td> 
   <td>Projecten</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>De toegang van iemand is gewijzigd</td> 
   <td>Projecten, taken, problemen, documenten, portfolio's, programma's</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Commentaarobject abonneren</td> 
   <td>Projecten, taken, problemen</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
 </tbody> 
</table>

Om te vormen welke acties u [!DNL Workfront] wilt volgen:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Interface]** en vervolgens op **[!UICONTROL Update Feeds]** .

1. Klik op de tab **[!UICONTROL Actions]** .

1. Schakel het selectievakje van een handeling in of uit om deze uit te schakelen.
1. Klik op **[!UICONTROL Save]**.

   Wanneer u een handeling uitschakelt, blijven eerder opgenomen updates over die handeling behouden in het [!UICONTROL Updates] -gebied waar deze is opgenomen. [!DNL Workfront] stopt met het opnemen van nieuwe updates voor de uitgeschakelde handeling.
