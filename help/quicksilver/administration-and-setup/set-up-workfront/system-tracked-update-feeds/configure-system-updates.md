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
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Systeemupdates configureren

[!DNL Adobe Workfront] genereert automatische systeemupdates in het [!UICONTROL Updates] -gebied van een object om de volgende gebeurtenissen op te nemen:

* Wijzigingen aanbrengen in een objectveld
* Handelingen die gebruikers uitvoeren op een object

Deze systeemupdates bevatten het volgende type informatie:

* De aangebrachte wijziging
* De naam van de gebruiker die de wijziging heeft aangebracht
* Het tijdstip en de datum van de wijziging

Voor meer informatie over systeemupdates, zie [ systeem-geleide updates ](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] beheerder kunt u configureren welke objectvelden en handelingen [!DNL Workfront] bijhoudt om systeemupdates op te nemen.

U kunt bijvoorbeeld in [!DNL Workfront] alle wijzigingen bijhouden die gebruikers in de namen van problemen in het hele systeem doorvoeren. Elke wijziging in de naam van een uitgave wordt vervolgens weergegeven als een systeemupdate in het [!UICONTROL Updates] -gebied van de uitgave.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bepalen welke velden [!DNL Workfront] bijhoudt voor een objecttype

U kunt bepalen welke informatie [!DNL Workfront] bijhoudt wanneer gebruikers informatie wijzigen die aan een bepaald objecttype is gekoppeld in de gehele [!DNL Workfront] -interface. U doet dit door de velden toe te voegen of te verwijderen die u in [!DNL Workfront] wilt bijhouden voor dat objecttype.

>[!NOTE]
>
>* [!DNL Workfront] kan geen updates bijhouden en opnemen over berekende aangepaste velden.
>* U kunt de systeemupdate aanpassen voor projecten, taken, problemen, portfolio&#39;s, programma&#39;s en gebruikers. U kunt de systeemupdate voor sjablonen, documenten of tijdbladen niet aanpassen, maar in [!DNL Workfront] worden de systeemupdates voor deze objecten wel vastgelegd.
>



* [Voeg gebieden toe u  [!DNL Workfront]  wilt volgen](#add-fields-you-want-workfront-to-track)
* [Velden verwijderen die u niet wilt bijhouden](#remove-fields-that-you-don-t-want-tracked)

### Velden toevoegen die u wilt bijhouden in [!DNL Workfront] {#add-fields-you-want-workfront-to-track}

U kunt velden toevoegen die u in [!DNL Workfront] voor een bepaald type object wilt bijhouden via de [!DNL Workfront] -interface. Wanneer gebruikers gegevens in dat veld wijzigen, slaat [!DNL Workfront] informatie over de wijziging op als een systeemupdate in het [!UICONTROL Updates] -gebied voor het object.

>[!NOTE]
>
>U kunt maximaal 300 ingebouwde en aangepaste velden bijhouden in de updatefeed. Als u het maximumaantal velden bijhoudt en aanvullende velden wilt bijhouden die niet op het subtabblad [!UICONTROL All Fields] worden weergegeven, moet u eerst enkele bijgehouden velden verwijderen om nieuwe velden bij te houden. Voor meer informatie over het verwijderen van gebieden uit de updategebieden, zie [ gebieden verwijderen die u niet gevolgd ](#remove-fields-that-you-don-t-want-tracked) wilt.

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik in het linkerdeelvenster op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** .

1. &#x200B; op **[!UICONTROL Add Fields]** en klik vervolgens op het object dat u wilt bijhouden.

1. In het vak &#x200B; **[!UICONTROL Update Feeds]** dat wordt weergegeven, typt u een ingebouwd (standaard) veld of een aangepast veld voor het object. Klik vervolgens om het veld te selecteren wanneer het in de lijst wordt weergegeven.

   Als [!DNL Workfront] het veld al volgt, kunt u het niet een tweede keer uit de lijst toevoegen.

1. Nadat u alle velden hebt toegevoegd die u in [!DNL Workfront] wilt bijhouden, klikt u op **[!UICONTROL Add Fields]** .

   De ingebouwde velden die u hebt toegevoegd, worden weergegeven onder de subtab **[!UICONTROL Built-in Fields]** .

   De aangepaste velden die u hebt toegevoegd, worden weergegeven onder de subtab **[!UICONTROL Custom Fields]** .

   Op het subtabblad **[!UICONTROL All Fields]** worden zowel de ingebouwde als de aangepaste velden weergegeven die worden bijgehouden.

### Velden verwijderen die u niet wilt bijhouden {#remove-fields-that-you-don-t-want-tracked}

U kunt velden verwijderen die het systeem niet voor een bepaald type object hoeft bij te houden in de gehele interface van [!DNL Workfront] .

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** .

1. Selecteer op het tabblad **[!UICONTROL Tracked Fields]** de subtab **[!UICONTROL All Fields]** .

   Dit toont zowel de ingebouwde als de douanevelden die momenteel worden gevolgd.

1. Selecteer het veld dat u wilt stoppen met bijhouden en klik op **[!UICONTROL Remove]** .

1. Klik in het vak **[!UICONTROL Remove Field]** dat wordt weergegeven op **[!UICONTROL Yes, Remove It]** om te bevestigen.

Alle updates over de eerder bijgehouden velden blijven behouden in het [!UICONTROL Updates] -gebied waar ze zijn opgenomen.

## Bepalen welke handelingen [!DNL Workfront] bijhoudt voor een objecttype

U kunt [!DNL Workfront] de volgende acties laten volgen die gebruikers op objecten kunnen uitvoeren door de [!DNL Workfront] -interface.

U kunt bijvoorbeeld [!DNL Workfront] elke keer dat een gebruiker een toewijzing wijzigt in een taak of uitgave, een update laten opnemen. De wijziging wordt dan weergegeven als een systeemupdate in het [!UICONTROL Updates] -gebied voor de taak of uitgave.

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
   <td>Projecten, Taken, Kwesties, Portfolio's, Programma's</td> 
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
   <td>Projecten, taken, problemen, documenten, Portfolio's, programma's</td> 
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

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .

1. Klik op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]** .

1. Klik op de tab **[!UICONTROL Actions]** .

1. Selecteer een handeling om deze in te schakelen of hef de selectie van een handeling op om deze uit te schakelen.
1. Klik op **[!UICONTROL Save]**.

Wanneer u een handeling uitschakelt, blijven eerder opgenomen updates over die handeling behouden in het [!UICONTROL Updates] -gebied waar deze is opgenomen.
