---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Systeemupdates configureren
description: Workfront genereert automatische systeemupdates in de [!UICONTROL Updates] om de wijzigingen op te nemen die gebruikers op het object uitvoeren. Als [!DNL Workfront] beheerder, kunt u vormen welke objecten gebieden en acties [!DNL Workfront] tracks voor het opnemen van systeemupdates.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Systeemupdates configureren

[!DNL Adobe Workfront] genereert automatische systeemupdates in de [!UICONTROL Updates] gebied voor het opnemen van de volgende gebeurtenissen:

* Wijzigingen aanbrengen in een objectveld
* Handelingen die gebruikers uitvoeren op een object

Deze systeemupdates omvatten de wijziging die is aangebracht, de naam van de gebruiker die de wijziging heeft aangebracht en de tijd en datum van de wijziging.

Zie voor meer informatie over systeemupdates [Door het systeem bijgehouden updates](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Als [!DNL Workfront] beheerder, kunt u vormen welke objecten gebieden en acties [!DNL Workfront] tracks voor het opnemen van systeemupdates.

U kunt bijvoorbeeld [!DNL Workfront] Volg alle wijzigingen die gebruikers aanbrengen in de namen van problemen in het hele systeem. Elke wijziging in de naam van een uitgave wordt dan weergegeven als een systeemupdate van de [!UICONTROL Updates] gebied.

## Toegangsvereisten

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Bepalen welke velden worden gebruikt [!DNL Workfront] tracks voor een objecttype

U kunt bepalen welke informatie [!DNL Workfront] tracks wanneer gebruikers de informatie die aan een bepaald objecttype is gekoppeld, in de gehele code wijzigen [!DNL Workfront] interface. U doet dit door de gewenste velden toe te voegen of te verwijderen [!DNL Workfront] om bij te houden voor dat objecttype.

>[!NOTE]
>
>* [!DNL Workfront] Kan geen updates bijhouden en opnemen over berekende aangepaste velden.
>* U kunt de systeemupdate aanpassen voor projecten, taken, problemen, portfolio&#39;s, programma&#39;s en gebruikers. U kunt de systeemupdate voor sjablonen, documenten of tijdbladen niet aanpassen, maar [!DNL Workfront] worden systeemupdates voor deze objecten vastgelegd.
>



* [Voeg gewenste velden toe [!DNL Workfront] naar track](#add-fields-you-want-workfront-to-track)
* [Velden verwijderen die u niet wilt bijhouden](#remove-fields-that-you-don-t-want-tracked)

### Voeg gewenste velden toe [!DNL Workfront] naar track {#add-fields-you-want-workfront-to-track}

U kunt gewenste velden toevoegen [!DNL Workfront] om een bepaald type object in de gehele [!DNL Workfront] interface. Wanneer gebruikers gegevens in dat veld wijzigen, [!DNL Workfront] registreert informatie over de verandering als systeemupdate in [!UICONTROL Updates] gebied voor het object.

>[!NOTE]
>
>U kunt maximaal 300 ingebouwde en aangepaste velden bijhouden in de updatefeed. Als u het maximumaantal velden bijhoudt en aanvullende velden wilt bijhouden die niet worden weergegeven in het dialoogvenster [!UICONTROL All Fields] Subtab, moet u eerst enkele bijgehouden velden verwijderen om nieuwe velden bij te houden. Zie voor meer informatie over het verwijderen van velden uit de updatevelden [Velden verwijderen die u niet wilt bijhouden](#remove-fields-that-you-don-t-want-tracked).

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. &#x200B; klikken **[!UICONTROL Add Fields]** Klik vervolgens op het object dat u wilt laten volgen.

1. In de &#x200B; **[!UICONTROL Update Feeds]** in het vak dat wordt weergegeven, typt u een ingebouwd (standaard) veld of een aangepast veld voor het object en klikt u op de gewenste waarde wanneer deze in de lijst wordt weergegeven.

   Indien [!DNL Workfront] Als u het veld al bijhoudt, kunt u het niet een tweede keer uit de lijst toevoegen.

1. Nadat u alle gewenste velden hebt toegevoegd [!DNL Workfront] om te volgen, klik **[!UICONTROL Add Fields]**.

   De ingebouwde velden die u hebt toegevoegd, worden weergegeven onder de **[!UICONTROL Built-in Fields]** subtab.

   De aangepaste velden die u hebt toegevoegd, worden weergegeven onder de **[!UICONTROL Custom Fields]** subtab.

   De **[!UICONTROL All Fields]** Op het subtabblad ziet u zowel de ingebouwde als de aangepaste velden die worden bijgehouden.

### Velden verwijderen die u niet wilt bijhouden {#remove-fields-that-you-don-t-want-tracked}

U kunt velden verwijderen die het systeem niet voor een bepaald type object hoeft bij te houden in het hele dialoogvenster [!DNL Workfront] interface.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. Op de **[!UICONTROL Tracked Fields]** selecteert u de **[!UICONTROL All Fields]** subtab.

   Dit toont zowel de ingebouwde als de douanevelden die momenteel worden gevolgd.

1. Selecteer het veld dat u wilt stoppen met bijhouden en klik op **[!UICONTROL Remove]**.

1. In de **[!UICONTROL Remove Field]** vak dat wordt weergegeven, klikt u op **[!UICONTROL Yes, Remove It]** ter bevestiging.

Alle updates over de eerder bijgehouden velden blijven behouden in het dialoogvenster [!UICONTROL Updates] het gebied waar zij zijn geregistreerd.

## Bepalen welke handelingen worden uitgevoerd [!DNL Workfront] tracks voor een objecttype

U kunt [!DNL Workfront] Volg de volgende handelingen die gebruikers op objecten kunnen uitvoeren in de gehele [!DNL Workfront] interface.

U kunt bijvoorbeeld [!DNL Workfront] registreert een update telkens als een gebruiker een taak of kwestie verandert. De wijziging wordt dan weergegeven als een systeemupdate in het dialoogvenster [!UICONTROL Updates] gebied voor de taak of kwestie.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Handeling</strong> </th> 
   <th><strong>Objecten</strong> </th> 
   <th><strong>Standaardstatus</strong> </th> 
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
   <td>Projecten, Taken, Kwesties, Portfolio, Programma's</td> 
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
   <td>Projecten, taken, problemen, documenten, Portfolio, programma's</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
  <tr> 
   <td>Commentaarobject abonneren</td> 
   <td>Projecten, taken, problemen</td> 
   <td> <p>Ingeschakeld</p> </td> 
  </tr> 
 </tbody> 
</table>

Om te vormen welke acties u wilt [!DNL Workfront] om te volgen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. Klik op de knop **[!UICONTROL Actions]** tab.

1. Selecteer een handeling om deze in te schakelen of hef de selectie van een handeling op om deze uit te schakelen.
1. Klik op **[!UICONTROL Save]**.

Wanneer u een actie onbruikbaar maakt, wordt om het even welke eerder geregistreerde update over die actie bewaard in [!UICONTROL Updates] het gebied waar het werd geregistreerd.
