---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: De knop Gereed configureren voor problemen
description: Met de knop Gereed kunt u automatisch de status van een taak of een uitgave instellen. Adobe Workfront markeert standaard een probleem dat is opgelost wanneer een toegewezen persoon op Gereed klikt voor het betreffende werkitem.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1006'
ht-degree: 0%

---

# Configureer de [!UICONTROL Done] knop voor problemen

De [!UICONTROL Done] kan de status van een taak of een uitgave automatisch instellen. Standaard, [!DNL Adobe Workfront] markeert een uitgave als [!UICONTROL Resolved] wanneer een ontvanger klikt [!UICONTROL Done] op hun werkitem.

## Overzicht

Gebruikers met bepaalde machtigingen kunnen de [!UICONTROL Done] om bepaalde statussen in het systeem te weerspiegelen. Er zijn drie verschillende manieren waarop [!UICONTROL Done] knop werkt voor problemen in [!DNL Workfront]:

* Als de gebruiker een toegewezen [!UICONTROL Home Team], [!DNL Workfront] beheerder of een gebruiker met een [!UICONTROL Plan] licentie kan de [!UICONTROL Done] om bepaalde statussen voor teamleden te weerspiegelen. Zie [Configureer de [!UICONTROL Done] knoop voor een Team](#configure-the-uicontrol-done-button-for-a-team) in dit artikel.
* Als de gebruiker geen [!UICONTROL Home Team] toegewezen [!UICONTROL Done] knop voor problemen is gekoppeld aan een systeem dat wordt gegenereerd [!UICONTROL Resolved] status met de drielettercode [!UICONTROL RLV]. Er zijn geen configuratieopties beschikbaar in dit scenario. De [!UICONTROL Done] automatisch wordt deze status ingesteld.
* Als de [!UICONTROL Resolved] ([!UICONTROL RLV]) wordt verwijderd en de gebruiker het probleem markeert als [!UICONTROL Done] heeft geen [!UICONTROL Home Team], is de standaarduitgiftestatus gekoppeld aan wat als standaard is ingesteld voor [!UICONTROL Closed] voor de groep die aan het project wordt toegewezen, behoort de kwestie tot. De Workfront-beheerder kan een standaardinstelling voor de groep configureren voor het hele systeem. Zie [Configureer de [!UICONTROL Done] als de knop [!UICONTROL Resolved] status is verwijderd](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in dit artikel.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td>De beheerdertoegang van het systeem wordt vereist om te vormen [!UICONTROL Done] als de knop [!UICONTROL Resolved] status wordt verwijderd</td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Configureer de [!UICONTROL Done] knoop voor een Team

U kunt wijzigen welke status op het werkitem is toegepast met de opdracht [!UICONTROL Done] knop. U kunt ook meerdere statussen instellen en de gebruiker de mogelijkheid geven om te kiezen welke status geschikt is.

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Teams]**.

1. Klik op de knop **[!UICONTROL Switch team]** selecteert u vervolgens een nieuw team in het keuzemenu of zoekt u naar een team in de zoekbalk.
1. Klik op de knop **[!UICONTROL More]** en klik vervolgens op **[!UICONTROL Edit]**.
1. Zoek de **[!UICONTROL Done Button]** onderaan in het gedeelte **[!UICONTROL Team Settings]** pagina.

1. Selecteer één status of meer dan één status voor elk type werkitem.

   >[!NOTE]
   >
   >Houd rekening met het volgende wanneer u statussen selecteert voor taken of problemen:
   >
   >* Wanneer u één status selecteert voor elk type werkitem, wordt de taak- of uitgiftestatus ingesteld op die status wanneer een gebruiker klikt [!UICONTROL Done] op hun object. Als u meerdere statussen instelt voor elk type werkitem, wordt een vervolgkeuzemenu toegevoegd aan het dialoogvenster [!UICONTROL Done] en de gebruiker moet een status selecteren om de status van het werkitem te wijzigen.
   >* U kunt alleen statussen op systeemniveau koppelen aan de [!UICONTROL Done] knop. U kunt geen groepsspecifieke statussen koppelen aan de status van het werkitem.
   >* Wanneer een gebruiker die aan het item is toegewezen het item in de status plaatst die aan het [!UICONTROL Done] knop, het item wordt weergegeven als [!UICONTROL Done] voor die gebruiker, ongeacht of de status die u selecteert een [!UICONTROL Completed] of [!UICONTROL Closed] status of een werkstatus.

   >   
   >   
   >  Bijvoorbeeld, associating [!UICONTROL Done] knop met In uitvoering zorgt dat het werkitem wordt weergegeven als [!UICONTROL Done] voor de gebruiker die de status wijzigt van Nieuw in Bezig.
   >   
   >* De types van kwestie zijn aanpasbaar en zij zouden verschillende namen kunnen hebben dan hieronder vermeld in uw milieu.\
      >  Hier volgen de standaardtaken en -typen:
      >     
      >   * [!UICONTROL Tasks]
      >   * [!UICONTROL Issue]
      >   * [!UICONTROL Request]
      >   * [!UICONTROL Change Order]
      >   * [!UICONTROL Bug Report]


   Als de taak of kwestie aan veelvoudige gebruikers wordt toegewezen, ziet u &quot;[!UICONTROL Done with my part]&quot; in het keuzemenu, naast de meerdere statussen die voor uw team zijn gekozen.

1. Klik op **[!UICONTROL Save Changes]**.

## Gebruikers koppelen aan een Home Team

Als u de wijzigingen wilt aanbrengen in het dialoogvenster [!UICONTROL Done] de knoopfunctionaliteit zichtbaar aan gebruikers, kunt u het team maken waarvan montages u het Team van het Huis van de gebruikers veranderde.

Om gebruikers met een Team van het Huis te associëren:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront].

1. Klikken **[!UICONTROL Users]** en selecteert u vervolgens de gebruiker of gebruikers die u aan een Home Team wilt koppelen.
1. Klik op de knop **[!UICONTROL More]** menu, selecteert u vervolgens **[!UICONTROL Edit]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. In de **[!UICONTROL Organization]** selecteert u de **[!UICONTROL Home Team]** veld. Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.
Om het even welke teammontages, met inbegrip van de statussen verbonden aan [!UICONTROL Done] zijn nu zichtbaar voor deze gebruikers.

## Configureer de [!UICONTROL Done] als de knop [!UICONTROL Resolved] status is verwijderd

Als een gebruiker geen Team van het Huis en het systeembrede gebrek voor heeft [!UICONTROL Resolved] ([!UICONTROL RLV]) is verwijderd, a [!DNL Workfront] beheerder kan de [!UICONTROL Closed] status van de groep die het project uitvoert. [!DNL Workfront] selecteert deze status voor een gesloten probleem wanneer de gebruiker op de knop [!DNL Done] knop.

### Zoek de groep die aan het project is gekoppeld

Wanneer een gebruiker een project creeert, wordt hun Groep van het Huis automatisch toegewezen aan het project. Gebruikers met [!UICONTROL Manage] de toegang tot het project kan deze groep in [!UICONTROL Project Details] op elk gewenst moment. Om te begrijpen welke status [!DNL Workfront] gebruik voor een voltooide kwestie in dit geval, moet u begrijpen welke groep met het project wordt geassocieerd de kwestie is en wat de standaardstatus voor [!UICONTROL Closed] deze groep heeft voor problemen te maken .

U kunt als volgt de groep vinden die aan het project is gekoppeld:

1. Ga naar een project.
1. Klik links op de pagina op **[!UICONTROL Project Details]**.
1. Zoek de **[!UICONTROL Project association]** sectie, dan zoeken **[!UICONTROL Group]**.\
   Dit is de groepsnaam u moet gebruiken om de status in het gebied van de Opstelling te controleren. Zie de volgende sectie voor instructies over hoe te om de standaardstatus voor een specifieke groep bij te werken.

### De standaardstatus voor een specifieke groep bijwerken

Als [!UICONTROL Workfront] beheerder, kunt u de status voor een specifieke groep bijwerken:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klik in het linkerdeelvenster op **[!UICONTROL Project Preferences]** vervolgens **[!UICONTROL Statuses]**.

1. Klikken **[!UICONTROL Issues]** Typ vervolgens de naam van de groep in het dialoogvenster **[!UICONTROL System Statuses]** zoekvak rechts.

1. Selecteer de groep.
1. Klik op de knop **[!UICONTROL Set Default Statuses]** vervolgkeuzemenu en kies vervolgens een standaardstatus voor [!UICONTROL Closed]. [!DNL Workfront] gebruikt deze status voor een gesloten kwestie wanneer een gebruiker klikt [!UICONTROL Done] knop.

   >[!IMPORTANT]
   >
   >Deze status wordt alleen gebruikt wanneer de gebruiker geen Home Team heeft toegewezen en de [!UICONTROL RLV] status is verwijderd.

1. Klik op **[!UICONTROL Save]**.
