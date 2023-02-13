---
product-area: resource-management
navigation-topic: resource-scheduling
title: Gegevens filteren in het planningsgebied
description: Het gebruiken van een filter in het Middel dat gebied plant laat u toe om te bepalen welke het werkpunten op de het plannen chronologie worden getoond. Dit omvat welke taken en kwesties in Unassigned gebied worden getoond, evenals welke gebruikers worden getoond.
author: Alina
feature: Resource Management
exl-id: 974b2515-ed10-459d-a317-36e62c52afc7
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '2452'
ht-degree: 0%

---

# Gegevens filteren in het planningsgebied

>[!IMPORTANT]
>  
><span class="preview">De planningsfunctionaliteit die in dit artikel wordt beschreven, is vanaf de release 23.1 in januari 2023 vervangen en uit Adobe Workfront verwijderd.   </span>
>  
> <span class="preview"> Dit artikel wordt ook verwijderd kort na de release van 23.1, begin 2023. Op dit moment raden we u aan eventuele bladwijzers dienovereenkomstig bij te werken. </span>
> 
><span class="preview"> U kunt de werklastbalans nu gebruiken om werk voor uw bronnen te plannen. </span>
>  
> <span class="preview">Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie de sectie [De werklastbalans](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**.  </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

<!--
<p>(SEVERAL SECTIONS BELOW LINKED TO THE PRODUCT. SEE NOTES</p>
-->

Het gebruiken van een filter in het Middel dat gebied plant laat u toe om te bepalen welke het werkpunten op de het plannen chronologie worden getoond. Dit omvat welke taken en kwesties in Unassigned gebied worden getoond, evenals welke gebruikers worden getoond.

Voordat u begint met het filteren van inhoud zoals beschreven in deze sectie, moet u goed leren hoe het plannen van resources in Adobe Workfront werkt.\
Raadpleeg het artikel voor informatie over het plannen van bronnen in Workfront [Aan de slag met Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).\
Zie het artikel voor meer informatie over de tijdlijn voor planning [Aan de slag met Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

U kunt middelen of een individueel team plannen u een lid van of voor om het even welke projecten bent waarvoor u de Manager van het Middel bent.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>De toegang van de mening of hoger tot Projecten, Taken, en Kwesties</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toestemmingen of hoger van de mening aan projecten, taken, en kwesties</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

<!--
<p>(NOTE: sections below - LINKED TO THE ui. DO NOT RENAME/ DELETE)</p>
-->

## Een filter maken in de sectie Schema (voor teams)

De taken en de kwesties van de projecten, de gebruikers, en de rollen u in de filter bepaalt worden getoond op de het plannen chronologie op het Werken aan lusje. Gebruik de opties in de filter om te bepalen welke projecten, gebruikers, en rollen op de het plannen chronologie worden vertegenwoordigd.

>[!NOTE]
>
>U kunt geen filter opslaan in het tabblad Werken op tabblad (voor een team). Wanneer u de pagina vernieuwt of buiten de pagina navigeert, worden de standaardinstellingen hersteld.

U kunt als volgt een filter voor de tijdlijn van de planning maken op het tabblad Werken aan voor teams:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Teams**, selecteert u een team en klikt u op **Werklastverdeling** in het linkerdeelvenster selecteert u vervolgens **Planning** in het keuzemenu linksboven.
1. Klikken **Filter**.
1. Bepaal welke projecten in Unassigned gebied door de volgende informatie te specificeren worden vertegenwoordigd:

   <!--
   <p>(NOTE: Alina: there was a note that [This step is linked to from the context-sensitive help] but I could not find from where in the UI it is linked.)&nbsp;</p>
   -->

   * **Projectprioriteiten:** Selecteer de prioriteit van de projecten die u op de het plannen chronologie wilt worden vertegenwoordigd. De taken en de kwesties van projecten met de prioriteiten u selecteert worden getoond op de het plannen chronologie.\
      Alleen prioriteiten van projecten die taken of problemen bevatten die aan het team zijn toegewezen, zijn beschikbaar in dit menu.
   * **Status van project:** Selecteer de status van de projecten die u op de geplande tijdlijn wilt worden vertegenwoordigd. Taken en problemen in projecten met de status die u selecteert, worden weergegeven op de tijdlijn van de planning.\
      Alleen statussen van projecten die taken of problemen bevatten die aan het team zijn toegewezen, zijn beschikbaar om te kiezen in dit menu.
   * **Projecten:** Selecteer om het even welke projecten die u op de het plannen chronologie wilt worden vertegenwoordigd. De taken en de kwesties van de projecten u selecteert worden getoond op de het plannen chronologie.\
      Uw selecties in de vorige velden bepalen welke projecten beschikbaar zijn om te selecteren.\
      Alleen projecten die taken of problemen bevatten die aan het team zijn toegewezen, zijn beschikbaar om te kiezen in dit menu.

1. Bepaal welke gebruikers op de planningschronologie door de volgende informatie te specificeren worden getoond. Standaard worden alle teamleden weergegeven.

   <!--
   <p>(NOTE: this step is linked in the UI.)</p>
   -->

   * **Rollen:** Selecteer de rollen u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen taken die aan die rol zijn toegewezen, worden weergegeven in het gebied Niet toegewezen. Alleen gebruikers met de rollen die u selecteert en aan wie die taken kunnen worden toegewezen, worden weergegeven.\
      Gebruikers worden weergegeven op de tijdlijn voor de planning, ingedeeld op taakrol.
   * **Gebruikers:** Selecteer de individuele gebruikers u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen de gebruikers die u selecteert, worden weergegeven, ongeacht of ze een roltoewijzing hebben die overeenkomt met de roltoewijzing van taken in het gebied Niet toegewezen.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.

      <!--   
     <p>(NOTE: Alina: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])</p>   
     -->

1. (Optioneel) Raadpleeg het artikel als u verdere wijzigingen wilt aanbrengen in de tijdlijn van de planning (zoals het wijzigen van het datumbereik) en de gebruikerstoewijzingen wilt wijzigen [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

<!--
<p>(NOTE: below - LINKED TO THE UI, DO NOT RENAME/ DELETE/ CHANGE)</p>
-->

## Filters maken en wijzigen in de sectie Planning (voor meerdere projecten)

U kunt een nieuw filter maken, een eerder gemaakt filter toepassen, een eerder gemaakt filter wijzigen of een filter verwijderen. U kunt filters die u maakt, niet delen met andere gebruikers.

* [Creeer een filter in de Plannende sectie (voor projecten)](#create-a-filter-in-the-scheduling-section-for-projects)
* [Een opgeslagen filter toepassen](#apply-a-saved-filter)
* [Een opgeslagen filter wijzigen](#modify-a-saved-filter)
* [Een opgeslagen filter verwijderen](#delete-a-saved-filter)

### Creeer een filter in de Plannende sectie (voor projecten) {#create-a-filter-in-the-scheduling-section-for-projects}

<!--
<p>(NOTE: *****LINKED TO THE PRODUCT FROM THE GLOBAL SCHEDULER >> BOTH THE FIRST AND THE SECOND AREAS) </p>
-->

De taken en de kwesties van de projecten, de gebruikers, en de rollen u in de filter bepaalt worden getoond op de het plannen chronologie op het Plannende lusje. Gebruik de opties in de filter om te bepalen welke projecten, gebruikers, en rollen op de het plannen chronologie worden vertegenwoordigd.

Om een filter voor de het plannen chronologie op het Plannende lusje voor veelvoudige projecten tot stand te brengen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
1. Klikken **Filter**.\
   ![](assets/scheduling-filter-350x351.png)

1. Laat de **Opgeslagen filters** veld leeg.
1. Bepaal welke projecten in Unassigned gebied door de volgende informatie te specificeren worden vertegenwoordigd:

   <!--
   <p>(NOTE: Alina: this step is linked in the UI.) </p>
   -->

   * **Portfolio:** Selecteer om het even welke portefeuilles die programma&#39;s en projecten omvatten die u op de het plannen chronologie wilt worden vertegenwoordigd.

      Alleen programma&#39;s binnen de portfolio&#39;s die u selecteert, kunnen worden geselecteerd in het dialoogvenster **Programma** veld.

   * **Programma&#39;s:** Selecteer om het even welke programma&#39;s die projecten omvatten die u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Uw selecties in het dialoogvenster **Portfolio** bepaalt welke programma&#39;s beschikbaar zijn om te selecteren.\
      Alleen projecten binnen de geselecteerde programma&#39;s zijn beschikbaar voor selectie in de **Projecten** veld.

   * **Projectprioriteiten:** Selecteer de prioriteit van de projecten die u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen projecten met de geselecteerde prioriteiten worden weergegeven.

   * **Status van project:** Selecteer de status van de projecten die u op de geplande tijdlijn wilt worden vertegenwoordigd.\
      Alleen projecten met de status die u selecteert, worden weergegeven.

   * **Projectbedrijven:** De taken en de kwesties worden getoond op de het plannen chronologie slechts wanneer zij tot een project behoren dat een bedrijf aanpast u selecteert.

   * **Projectgroepen:** Taken en problemen worden alleen op de tijdlijn van de planning weergegeven wanneer ze bij een project horen dat overeenkomt met een groep die u selecteert.

   * **Projecten:** Selecteer om het even welke projecten die u op de het plannen chronologie wilt worden vertegenwoordigd. De taken en de kwesties van de projecten u selecteert worden getoond op de het plannen chronologie.\
      Uw selecties in de vorige velden bepalen welke projecten beschikbaar zijn om te selecteren.\
      De taken en de kwesties van de projecten u selecteert worden getoond op de het plannen chronologie. Alleen projecten die taken of problemen bevatten die aan het team zijn toegewezen, zijn beschikbaar om te kiezen in dit menu.

1. Bepaal welke gebruikers op de geplande tijdlijn worden weergegeven door de volgende informatie op te geven: (Standaard worden alleen gebruikers weergegeven die in aanmerking komen voor een taak of uitgave in het gebied Niet toegewezen. Wanneer u individuele gebruikers selecteert, worden de gebruikers getoond op de plannende chronologie ongeacht of zij verkiesbaar zijn om een taak of kwestie van het Niet toegewezen gebied worden toegewezen.) 

   <!--
   <p>(NOTE: Alina: this step had a note that it is linked in the UI but I could not find from where.) </p>
   -->

   * **Gebruikersbedrijven:** Met dit veld kunt u voorkomen dat gebruikers van andere bedrijven worden weergegeven op de tijdlijn van de planning.\
      Laat dit veld leeg als u wilt dat gebruikers van een bedrijf worden toegevoegd. Als u afzonderlijke bedrijven opgeeft, kunnen alleen gebruikers van die bedrijven aan de tijdlijn van de planning worden toegevoegd. Als u een bedrijf opgeeft, worden gebruikers van dat bedrijf niet automatisch toegevoegd aan de tijdlijn van de planning. Gebruik in plaats daarvan de onderstaande velden om specifieke gebruikers toe te voegen.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.****

   * **Gebruikersgroepen:** Alle gebruikers van een gebruikersgroep die u opgeeft, worden weergegeven op de tijdlijn van de planning.

   * **Teams:** Alle gebruikers van een team dat u opgeeft, worden weergegeven op de tijdlijn van de planning.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.

   * **Rollen:** Selecteer de rollen u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen taken die aan die rol zijn toegewezen, worden weergegeven in het gebied Niet toegewezen. Alleen gebruikers met de rollen die u selecteert en aan wie die taken kunnen worden toegewezen, worden weergegeven.\
      Gebruikers worden weergegeven op de tijdlijn voor de planning, ingedeeld op taakrol.

   * **Gebruikers:** Selecteer de individuele gebruikers u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen de gebruikers die u selecteert, worden weergegeven, ongeacht of ze een roltoewijzing hebben die overeenkomt met de roltoewijzing van taken in het gebied Niet toegewezen.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.
   <!--
   <p>NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->

1. Klikken **Nieuw filter opslaan**.\
   Uw gegevens worden weergegeven op de tijdlijn van de planning.

1. (Optioneel) Raadpleeg het artikel als u verdere wijzigingen wilt aanbrengen in de tijdlijn van de planning (zoals het wijzigen van het datumbereik) en de gebruikerstoewijzingen wilt wijzigen [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Een opgeslagen filter toepassen {#apply-a-saved-filter}

>[!NOTE]
>
>Deze optie is slechts van toepassing wanneer het plannen van middelen voor veelvoudige projecten (van het Plannende lusje); u kunt geen bewaarde filter toepassen wanneer het plannen van middelen voor een team (van het Werken aan lusje) of wanneer het plannen van middelen voor één enkel project (van het Stafbestellende lusje).

U kunt een filter toepassen dat u eerder hebt gemaakt.

Een opgeslagen filter toepassen op meerdere projecten:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
1. Klikken **Filter**.
1. In de **Opgeslagen filters** selecteert u het filter dat u wilt toepassen.\
   Uw gegevens worden weergegeven op de tijdlijn van de planning.

1. (Optioneel) Raadpleeg het artikel als u verdere wijzigingen wilt aanbrengen in de tijdlijn van de planning (zoals het wijzigen van het datumbereik) en de gebruikerstoewijzingen wilt wijzigen [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Een opgeslagen filter wijzigen {#modify-a-saved-filter}

>[!NOTE]
>
>Deze optie is slechts van toepassing wanneer het plannen van middelen voor veelvoudige projecten (van het Plannende lusje); u kunt geen opgeslagen filter wijzigen wanneer het plannen van middelen voor een team (van het Werken aan lusje) of wanneer het plannen van middelen voor één enkel project (van het Stafbestellende lusje).

U kunt een filter wijzigen dat u eerder hebt gemaakt.

Een opgeslagen filter wijzigen voor meerdere projecten:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
1. Klikken **Filter**.
1. In de **Opgeslagen filters** selecteert u in de vervolgkeuzelijst het filter dat u wilt wijzigen.
1. Geef op welke gegevens op de tijdlijn van de planning moeten worden weergegeven.
1. Klikken **Opslaan**.\
   Uw gegevens worden weergegeven op de tijdlijn van de planning.

1. (Optioneel) Raadpleeg het artikel als u verdere wijzigingen wilt aanbrengen in de tijdlijn van de planning (zoals het wijzigen van het datumbereik) en de gebruikerstoewijzingen wilt wijzigen [Niet-toegewezen taken en problemen handmatig toewijzen in de planningsgebieden](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Een opgeslagen filter verwijderen {#delete-a-saved-filter}

>[!NOTE]
Deze optie is slechts van toepassing wanneer het plannen van middelen voor veelvoudige projecten (van het Plannende lusje); u kunt geen bewaard filter schrappen wanneer het plannen van middelen voor een team (van het Werken aan lusje) of wanneer het plannen van middelen voor één enkel project (van het Stafsende lusje).

U kunt een filter verwijderen dat u eerder hebt gemaakt.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
1. Klikken **Filter**.
1. In de **Opgeslagen filters** Klik in de vervolgkeuzelijst op de (x) naast het filter dat u wilt verwijderen. 

## Filters maken en wijzigen in de sectie Planning (voor één project)

<!--
<p>(NOTE: **** LINKED FROM THE PRODUCT FROM THE PROJECT> STAFFING> SCHEDULING AREA) </p>
-->

Taken en kwesties van de gebruikers, de teams, en de rollen u in de filter bepaalt worden getoond op de plannende chronologie op het het Vouwen lusje. Gebruik de opties in de filter om te bepalen welke gebruikers, teams, en rollen op de het plannen chronologie worden vertegenwoordigd.

>[!NOTE]
U kunt geen filter opslaan op het tabblad Werkruimte (voor één project). Wanneer u de pagina vernieuwt of buiten de pagina navigeert, worden de standaardinstellingen hersteld.

Om een filter voor de het plannen chronologie op het het Vouwen lusje voor één enkele projecten tot stand te brengen:

1. Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.
1. Bepaal welke gebruikers op de geplande tijdlijn worden weergegeven door de volgende informatie op te geven: (Standaard worden alleen gebruikers weergegeven die in aanmerking komen voor een taak of uitgave in het gebied Niet toegewezen. Wanneer u individuele gebruikers selecteert, worden de gebruikers getoond op de plannende chronologie ongeacht of zij verkiesbaar zijn om een taak of kwestie van het Niet toegewezen gebied worden toegewezen.) 

   <!--
   <p><span>(NOTE: Alina: [This step is linked to from the context-sensitive help]) </span> </p>
   -->

   * **Gebruikersbedrijven:** Met dit veld kunt u voorkomen dat gebruikers van andere bedrijven worden weergegeven op de tijdlijn van de planning.\
      Laat dit veld leeg als u wilt dat gebruikers van een bedrijf worden toegevoegd. Als u afzonderlijke bedrijven opgeeft, kunnen alleen gebruikers van die bedrijven aan de tijdlijn van de planning worden toegevoegd. Als u een bedrijf opgeeft, worden gebruikers van dat bedrijf niet automatisch toegevoegd aan de tijdlijn van de planning. Gebruik in plaats daarvan de onderstaande velden om specifieke gebruikers toe te voegen.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.

   * **Gebruikersgroepen:** Alle gebruikers van een gebruikersgroep die u opgeeft, worden weergegeven op de tijdlijn van de planning.

   * **Teams:** Alle gebruikers van een team dat u opgeeft, worden weergegeven op de tijdlijn van de planning.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.

   * **Rollen:** Selecteer de rollen u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen taken die aan die rol zijn toegewezen, worden weergegeven in het gebied Niet toegewezen. Alleen gebruikers met de rollen die u selecteert en aan wie die taken kunnen worden toegewezen, worden weergegeven.\
      Gebruikers worden weergegeven op de tijdlijn voor de planning, ingedeeld op taakrol.

   * **Gebruikers:** Selecteer de individuele gebruikers u op de het plannen chronologie wilt worden vertegenwoordigd.\
      Alleen de gebruikers die u selecteert, worden weergegeven, ongeacht of ze een roltoewijzing hebben die overeenkomt met de roltoewijzing van taken in het gebied Niet toegewezen.\
      Deze optie heeft geen invloed op welke taken en problemen worden weergegeven in het gebied Niet toegewezen.
   <!--
   <p>(NOTE: [! Users with Plan, Work, or Review licenses are available. Users with Request licenses are not available. - This is what it used to say. I think now instead you select specific users, not license types.])<br></p>
   -->
