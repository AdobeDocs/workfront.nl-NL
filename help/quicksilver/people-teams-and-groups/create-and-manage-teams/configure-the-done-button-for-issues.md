---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: De knop Gereed voor problemen configureren
description: Met de knop Gereed kunt u automatisch de status van een taak of een uitgave instellen. Adobe Workfront markeert standaard een probleem dat is opgelost wanneer een toegewezen persoon op Gereed klikt voor het betreffende werkitem.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 0%

---

# De knop [!UICONTROL Done] configureren voor problemen

Met de knop [!UICONTROL Done] kunt u automatisch de status van een taak of een uitgave instellen. Standaard markeert [!DNL Adobe Workfront] een uitgave als [!UICONTROL Resolved] wanneer een toegewezen persoon [!UICONTROL Done] op het werkitem klikt.

>[!NOTE]
>
>De knop Gereed wordt in alle gebieden van Workfront weergegeven als Markeren.

## Overzicht

Gebruikers met bepaalde machtigingen kunnen de knop [!UICONTROL Done] zo configureren dat bepaalde statussen in het systeem worden weerspiegeld. Er zijn drie verschillende manieren waarop de knop [!UICONTROL Done] werkt voor problemen in [!DNL Workfront] :

* Als de gebruiker een toegewezen [!UICONTROL Home Team] heeft, kan een [!DNL Workfront] beheerder of een gebruiker met een [!UICONTROL Plan] licentie de [!UICONTROL Done] knop configureren om bepaalde statussen voor teamleden te weerspiegelen. Zie [ de [!UICONTROL Done] knoop voor een Team ](#configure-the-uicontrol-done-button-for-a-team) in dit artikel vormen.
* Als de gebruiker geen [!UICONTROL Home Team] heeft maar [!UICONTROL Other Teams] in zijn profiel, zoekt Workfront naar de instelling van de knop [!UICONTROL Done] in een van de teams die aan de gebruiker zijn gekoppeld. De selectie is willekeurig en de status verbonden aan om het even welke teams wordt gebruikt voor de kwestie.
* Als de gebruiker geen [!UICONTROL Home Team] toegewezen heeft, is de [!UICONTROL Done] knop voor uitgaven gekoppeld aan een door het systeem gegenereerde [!UICONTROL Resolved] status met de drielettercode [!UICONTROL RLV] . Er zijn geen configuratieopties beschikbaar in dit scenario. Deze status wordt automatisch ingesteld op de knop [!UICONTROL Done] .
* Als de status [!UICONTROL Resolved] ([!UICONTROL RLV]) wordt verwijderd en de gebruiker die de uitgave als [!UICONTROL Done] markeert geen [!UICONTROL Home Team] heeft, is de standaarduitgavestatus gekoppeld aan wat als standaard voor [!UICONTROL Closed] wordt ingesteld voor de groep die is toegewezen aan het project waartoe de uitgave behoort. De Workfront-beheerder kan een standaardinstelling voor de groep configureren voor het hele systeem. Zie [ vormen de [!UICONTROL Done] knoop wanneer de [!UICONTROL Resolved] status ](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in dit artikel is geschrapt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-pakket</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>De beheerdertoegang van het systeem wordt vereist om de Gedaan knoop te vormen wanneer de Resolved status wordt geschrapt</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De knop [!UICONTROL Done] voor een team configureren

U kunt met de knop [!UICONTROL Done] wijzigen welke status wordt toegepast op het werkitem. U kunt ook meerdere statussen instellen en de gebruiker de mogelijkheid geven om te kiezen welke status geschikt is.

{{step1-to-team}}

1. Klik op het pictogram **[!UICONTROL Switch team]** en selecteer vervolgens een nieuw team in het keuzemenu of zoek naar een team op de zoekbalk.
1. Klik op het menu **[!UICONTROL More]** en klik vervolgens op **[!UICONTROL Edit]** .
1. Zoek de sectie **[!UICONTROL Done Button]** onder aan de pagina van **[!UICONTROL Team Settings]** .

1. Selecteer één status of meer dan één status voor elk type werkitem.

   >[!NOTE]
   >
   >Houd rekening met het volgende wanneer u statussen selecteert voor taken of problemen:
   >
   >* Wanneer u één status voor elk type werkitem selecteert, wordt de taak- of uitgiftestatus ingesteld op die status wanneer een gebruiker op [!UICONTROL Done] op het item klikt. Als u meerdere statussen instelt voor elk type werkitem, wordt een vervolgkeuzemenu toegevoegd aan de knop [!UICONTROL Done] en moet de gebruiker een status kiezen om de status van het werkitem te wijzigen.
   >* U kunt alleen statussen op systeemniveau aan de knop [!UICONTROL Done] koppelen. U kunt geen groepsspecifieke statussen koppelen aan de status van het werkitem.
   >* Wanneer een gebruiker die aan het item is toegewezen het item in de status plaatst die aan de knop [!UICONTROL Done] is gekoppeld, wordt het item weergegeven als [!UICONTROL Done] voor die gebruiker, ongeacht of de status die u selecteert een [!UICONTROL Completed] - of [!UICONTROL Closed] -status of een werkstatus is.
   >   
   >   
   >  Als u bijvoorbeeld de knop [!UICONTROL Done] koppelt aan Bezig, wordt het werkitem weergegeven als [!UICONTROL Done] voor de gebruiker die de status wijzigt van Nieuw in Bezig.
   >   
   >* De types van kwestie zijn aanpasbaar en zij zouden verschillende namen kunnen hebben dan hieronder vermeld in uw milieu.\
   >  Hier volgen de standaardtaken en -typen:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   Als de taak of de kwestie aan veelvoudige gebruikers wordt toegewezen, ziet u een &quot;[!UICONTROL Done with my part]&quot;optie in het drop-down menu, naast de veelvoudige statussen die voor uw team worden gekozen.

1. Klik op **[!UICONTROL Save Changes]**.

## Gebruikers koppelen aan een Home Team

Als u de wijzigingen in de knopfunctionaliteit van [!UICONTROL Done] zichtbaar wilt maken voor gebruikers, kunt u het team maken van wie u de instellingen hebt gewijzigd in het Home Team van de gebruikers.

Om gebruikers met een Team van het Huis te associëren:

1. Klik op het **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) rechtsboven in [!DNL Adobe Workfront] .

1. Klik op **[!UICONTROL Users]** en selecteer vervolgens de gebruiker of gebruikers die u aan een Home-team wilt koppelen.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .\
   ![](assets/user-settings-nwe-350x291.png)

1. Selecteer in de sectie **[!UICONTROL Organization]** het veld **[!UICONTROL Home Team]** . Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.
Alle teaminstellingen, inclusief de statussen die zijn gekoppeld aan de knop [!UICONTROL Done] , zijn nu zichtbaar voor deze gebruikers.

## De knop [!UICONTROL Done] configureren wanneer de status [!UICONTROL Resolved] is verwijderd

Als een gebruiker geen Team van het Huis heeft en het systeem-brede gebrek voor [!UICONTROL Resolved] ([!UICONTROL RLV]) is geschrapt, kan een [!DNL Workfront] beheerder de [!UICONTROL Closed] status voor de groep vormen op aan het project. [!DNL Workfront] selecteert deze status voor een afgesloten uitgave wanneer de gebruiker op de knop [!DNL Done] klikt.

### Zoek de groep die aan het project is gekoppeld

Wanneer een gebruiker een project creeert, wordt hun Groep van het Huis automatisch toegewezen aan het project. Gebruikers met [!UICONTROL Manage] toegang tot het project kunnen deze groep op elk gewenst moment wijzigen in de sectie [!UICONTROL Project Details] . Als u wilt weten welke status [!DNL Workfront] in dit geval gebruikt voor een voltooid probleem, moet u weten welke groep is gekoppeld aan het project waarop het probleem betrekking heeft en wat de standaardstatus voor [!UICONTROL Closed] deze groep heeft voor problemen.

U kunt als volgt de groep vinden die aan het project is gekoppeld:

1. Ga naar een project.
1. Klik links op de pagina op **[!UICONTROL Project Details]** .
1. Zoek de sectie **[!UICONTROL Project association]** en zoek **[!UICONTROL Group]** .\
   Dit is de groepsnaam u moet gebruiken om de status in het gebied van de Opstelling te controleren. Zie de volgende sectie voor instructies over hoe te om de standaardstatus voor een specifieke groep bij te werken.

### De standaardstatus voor een specifieke groep bijwerken

Als [!UICONTROL Workfront] beheerder kunt u de status voor een specifieke groep bijwerken:

1. Klik op het pictogram **[!UICONTROL Main Menu]** ![](assets/main-menu-icon.png) rechtsboven in Adobe Workfront en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png) .
1. Klik in het linkerdeelvenster op **[!UICONTROL Project Preferences]** en vervolgens op **[!UICONTROL Statuses]** .

1. Klik op **[!UICONTROL Issues]** en typ vervolgens de naam van de groep in het zoekvak **[!UICONTROL System Statuses]** rechts in het scherm.

1. Selecteer de groep.
1. Klik op het vervolgkeuzemenu **[!UICONTROL Set Default Statuses]** en kies een standaardstatus voor [!UICONTROL Closed] . [!DNL Workfront] gebruikt deze status voor een afgesloten uitgave wanneer een gebruiker op de knop [!UICONTROL Done] klikt.

   >[!IMPORTANT]
   >
   >Deze status wordt alleen gebruikt wanneer de gebruiker geen Home Team heeft toegewezen en de status [!UICONTROL RLV] is verwijderd.

1. Klik op **[!UICONTROL Save]**.
