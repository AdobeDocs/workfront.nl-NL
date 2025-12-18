---
title: Records delen
description: U kunt verslagen delen gebruikend de knoop van het Aandeel om samenwerking in de Planning van Adobe Workfront te verhogen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1772'
ht-degree: 0%

---


<!--update metadata with real information at release-->

# Records delen

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

U kunt de toestemmingen van mensen aan individuele verslagen in een verslagtype aanpassen.

U kunt een Adobe Workfront-planningsrecord op de volgende manieren delen:

* Een koppeling naar de record delen.

  Voor meer informatie, zie [ verslagen van het Aandeel gebruikend een verbinding ](/help/quicksilver/planning/records/share-records.md).

* Deel alle records in een werkruimte met andere gebruikers door de werkruimte en het recordtype te delen.

  Zie de volgende artikelen voor meer informatie:

   * [Een werkruimte delen](/help/quicksilver/planning/access/share-workspaces.md)

   * [Een recordtype delen](/help/quicksilver/planning/access/share-record-types.md)

* Deel een verslag gebruikend de **optie van het Aandeel**.

  Dit artikel beschrijft hoe u een verslag met anderen kunt delen gebruikend de **optie van het Aandeel**.

>[!IMPORTANT]
>
>Gebruikers met toegang tot een werkruimte krijgen automatisch minstens weergavemachtigingen voor alle records in de werkruimte.
>Als u weergaven deelt, geeft u gebruikers geen machtigingen voor records. Alleen werkruimten delen kan gebruikers machtigingen verlenen voor het opnemen van typen en records.
>
>Voor algemene informatie over het delen van voorwerpen in de Planning van Workfront, zie ook [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront- en planningspakketten</p> 
of
<p>Willekeurig workflowpakket en planningspakket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Alle</p> 
   <p><b>OPMERKING</b></p>
   <p>Alleen personen met een standaardlicentie kunnen beheermachtigingen voor records krijgen. Alle andere licenties kunnen alleen weergavemachtigingen hebben en de optie Beheren is voor deze licenties grijs.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td>  <p>Rechten voor een werkruimte, een recordtype en de record beheren</p>  
   <p><b>BELANGRIJK</b></p>
   <p>Alleen gebruikers met de machtiging Beheren in een werkruimte kunnen een record delen</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Lay-outsjabloon</p></td>
   <td> De gebruikers met een Licht of de vergunning van de Medewerker moeten een lay-outmalplaatje worden toegewezen dat Planning omvat.
   <p>De standaardgebruikers en de Beheerders van het Systeem hebben de Gebieden van de Planning die door gebrek worden toegelaten.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overwegingen bij het delen van records

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* U kunt records delen met de volgende entiteiten: personen, groepen, teams, bedrijven of functies.
* U kunt de volgende machtigingsniveaus aan een record toekennen:

   * Weergave
   * Beheren
* Wanneer u een werkruimte en een recordtype met gebruikers deelt, ontvangen zij ook de zelfde toestemmingen aan de verslagen in de werkruimte, door gebrek.
Wanneer gebruikers Contribute-machtigingen hebben voor een werkruimte of recordtype, ontvangen zij de machtiging Beheren voor de records van dat recordtype.
* Wanneer u een entiteit uit een werkruimte verwijdert, worden alle machtigingen voor delen verwijderd uit de recordtypen en alle records in de werkruimte.
* De toegang van een gebruiker tot de record wordt bepaald door de combinatie van de volgende drie instellingen:

   * Hun rechten worden overgenomen van het recordtype en de werkruimte
   * Machtigingen die afzonderlijk zijn toegevoegd in het dialoogvenster voor het delen van records
   * De volgende machtigingen:

      * **iedereen in de werkruimte kan** bekijken: Dit maakt het verslag viewable door iedereen in de werkruimte <!-- is this OK to say "workspace? should it be "record"??-->
      * **slechts kunnen de uitgenodigde mensen tot** toegang hebben: Dit wordt geselecteerd door gebrek en staat het beperken van toegang tot het verslag tot specifieke mensen toe.

     >[!NOTE]
     >
     >Als u verkiest om **iedereen in de werkruimte toestemming** aan een verslagtype of een verslag te verlenen, dan zal iedereen die in de het delen lijst van de werkruimtemachtigingen wordt vermeld de zelfde toestemmingen op het verslagtype en het verslag hebben, zelfs wanneer de geërfte toestemmingen gehandicapt zijn.


* Wanneer u een record deelt met een gebruiker, worden deze gegevens standaard toegevoegd met dezelfde machtigingen als voor het recordtype.

  Bijvoorbeeld:

   * Als zij de toestemmingen van de Mening aan het verslagtype hebben, krijgen zij de toestemmingen van de Mening aan het verslag
   * Als zij over Contribute- of beheermachtigingen voor het recordtype beschikken, krijgen zij beheermachtigingen voor de record

* Als werkruimtemanager kunt u een record delen met een gebruiker die geen machtigingen heeft voor het recordtype of de werkruimte. In dit geval, is er een waarschuwing naast de toegevoegde entiteit op de hoogte brengend dat zij geen toegang tot de werkruimte of het verslagtype hebben. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> U kunt doorgaan met het toevoegen van de gebruiker aan de record, waardoor deze ook wordt toegevoegd aan het recordtype en de werkruimte, of het delen annuleren.

* Wanneer een gebruiker beheerdersmachtigingen of Contribute heeft voor de werkruimte en het recordtype en u deze machtigingen toevoegt aan de recordmachtigingen, worden de weergavemachtigingen grijs weergegeven. Ze behouden dezelfde machtigingen voor de record als voor het recordtype en u kunt ze geen lagere machtigingen voor de record geven. <!--Lilit is checking on this, it is not working correctly-->

  Wanneer zij de toestemmingen van de Mening aan de werkruimte of het verslagtype hebben, behouden zij de toestemmingen van de Mening aan de verslagen. U kunt hen verlenen leiden toestemmingen aan het verslag door Geërfte toestemmingen onbruikbaar te maken en de Enige uitgenodigde mensen te selecteren kunnen tot het plaatsen toegang hebben. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* U kunt geërfte toestemmingen voor één enkel verslag onbruikbaar maken, in welk geval u hen toestemmingen aan individuele verslagen kunt geven, of zij kunnen toestemmingen verkrijgen als zij tot **iedereen in de werkruimte behoren** optie kan bekijken.

* Als meerdere machtigingen voor delen van toepassing zijn op dezelfde gebruiker, krijgen ze de hoogste machtigingen voor die machtigingen.

  Als een record bijvoorbeeld wordt gedeeld met een gebruiker met weergavemachtigingen en hun groep met beheertoegang, krijgen ze beheermachtigingen voor de record.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Als een formuleveld of een raadplegingsgebied van een verbonden verslag op een gebied op een verslag gebaseerd is waarover u geen toestemmingen hebt, zult u de correcte berekening zien welke factoren in het verslag u anders niet kunt toegang hebben.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Recordmachtigingen delen

Als werkruimtebeheerder kunt u machtigingen aanpassen aan afzonderlijke records.

{{step1-to-planning}}

1. Open de werkruimte waarvan u de records wilt delen.
1. Klik op het recordtype waarvan u de records wilt delen.

1. Voer een van de volgende handelingen uit:

   * Van de lijstmening, houd over de naam van een verslag, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Aandeel**.
   * Van de lijstmening, selecteer een verslag, dan klik **Aandeel** op de blauwe toolbar bij de bodem van de lijst.
   * Van om het even welke mening, klik de naam van een verslag, dan klik **Aandeel** in de hoger-juiste hoek van de de detailspagina van het verslag.

   Het **vakje van het Aandeel** opent.

   ![ Toestemmingen voor verslagen met geërfte toestemmingen op ](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Facultatief) in **die toegang** heeft, kan **iedereen in de werkruimte** optie bekijken door gebrek worden geselecteerd.  Alle gebruikers die **Mening** of hogere toestemmingen aan de werkruimte en verslagtype hebben hebben de zelfde toestemmingen aan het verslag.

1. (Facultatief) klik het aantal gebruikers onder de **Geërfte toestemmingen** optie om gebruikers, teams, groepen, bedrijven, of baanrollen te bekijken die toestemmingen van de werkruimte erven.

   >[!TIP]
   >
   >U kunt afzonderlijke entiteiten niet verwijderen uit de lijst Geërfde machtigingen.

1. (Optioneel en voorwaardelijk) Als u de record wilt delen met specifieke entiteiten en deze een andere toegang tot het recordtype wilt geven dan ze al hebben voor de werkruimte, gaat u als volgt te werk:

   1. Selecteer **onbruikbaar maken** van **Geërfte toestemmingen** drop-down menu.

   >[!TIP]
   >
   >Workspace-managers blijven beheermachtigingen hebben voor het recordtype en de record.

   1. (Optioneel) Selecteer **slechts uitgenodigde mensen kunnen** van **toegang hebben wie toegang** gebied heeft.

   1. In de **toegang van de Verlening tot dit verslagtype** gebied, voeg de gebruikers, de teams, de groepen, de bedrijven, of baanrollen toe die u een verschillend toestemmingsniveau aan wilt verlenen dan zij voor de werkruimte of het verslagtype hebben.
   1. Kies een van de volgende machtigingsniveaus:

      * Weergave
      * Beheren

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Naast teams, groepen, bedrijven, en baanrollen, kunt u slechts met gebruikers delen die aan Adobe Admin Console zijn toegevoegd. U kunt geen gebruikers met alleen Workfront toevoegen. Voor informatie, zie [ gebruikers in Adobe Admin Console ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md) leiden.
   >* Als gebruikers over Contribute- of Beheren-machtigingen voor de werkruimte en het recordtype beschikken, behouden zij de machtiging Beheren voor de record. De machtiging Weergeven is grijs. <!--this is not dimmed at this time, Lilit to check-->
   >* U kunt gebruikers niet minder machtigingen geven voor de record als ze Contribute of hoger hebben voor het recordtype.
   > Voor meer informatie, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Om gebruikers te geven die geen toestemmingen aan de werkruimtetoegang hebben om een verslag, op de **toegang van de Verlening tot dit mening** gebied te bekijken, begin de naam van een gebruiker, een groep, een team, een bedrijf, of baanrol te typen, dan het te klikken wanneer het in de lijst toont.

   De entiteit u selecteerde wordt toegevoegd aan het verslag en ook aan het verslagtype en de werkruimte met **toestemmingen van de Mening**.

   Systeembeheerders ontvangen altijd beheermachtigingen voor records die met hen worden gedeeld, en er is een indicatie dat een gebruiker een systeembeheerder is.

1. (Facultatief) klik **verbinding van het Exemplaar** om een verbinding aan het verslag aan uw klembord te kopiëren en het met anderen te delen. Met de koppeling wordt de detailpagina van de record geopend.
1. Klik **sparen**.

   De record wordt nu gedeeld met andere gebruikers.

   De gebruikers met wie u de record hebt gedeeld, ontvangen zowel een melding in de app als een e-mailmelding dat zij machtigingen hebben gekregen voor de volgende entiteiten:

   * De record
   * Het recordtype als ze nooit eerder machtigingen hadden
   * De werkruimte, als zij geen toestemmingen aan de werkruimte hadden alvorens het verslag met hen werd gedeeld.

   Voor informatie, zie [ de Planning van Adobe Workfront berichten: artikelindex ](/help/quicksilver/planning/notifications/notifications-information.md).

1. Deel de gekopieerde koppeling met anderen. Gebruikers die de koppeling ontvangen, moeten actieve gebruikers zijn en zich aanmelden bij Workfront om de pagina met recordtypen te kunnen openen en weergeven in de geselecteerde weergave. Zij moeten toestemmingen aan het verslagtype hebben om het te kunnen bekijken. Voor meer informatie, zie ook [ verslagen van het Aandeel gebruikend een verbinding ](/help/quicksilver/planning/records/share-records.md).

## Machtigingen verwijderen uit een record

U kunt gebruikersmachtigingen uit een record verwijderen. Ze behouden echter ten minste weergavemachtigingen voor de werkruimte die hun ten minste weergavemachtigingen voor het recordtype geven. U moet hun toegang uit de werkruimte verwijderen als u hen geen toestemmingen aan de verslagtypes of verslagen in de werkruimte wilt hebben.

{{step1-to-planning}}

1. Open de werkruimte waarvan de records die u niet meer wilt delen, u wilt ophouden met delen en klik vervolgens op een opnametype-kaart. Hierdoor wordt de pagina met recordtypen geopend.
1. Voer een van de volgende handelingen uit:

   * Van de lijstmening, houd over de naam van een verslag, klik **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Aandeel**.
   * Van de lijstmening, selecteer een verslag, dan klik **Aandeel** op de blauwe toolbar bij de bodem van de lijst.
   * Van om het even welke mening, klik de naam van een verslag, dan klik **Aandeel** in de hoger-juiste hoek van de de detailspagina van het verslag.

   Het **vakje van het Aandeel** opent.
1. Vind de gebruiker, de groep, het team, het bedrijf, of de baanrol die de toestemmingen u wilt verwijderen, het drop-down menu van toestemmingen rechts van hun naam uitbreiden, dan **verwijderen** klikken. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![ verwijdert toestemmingen op verslag ](assets/remove-option-on-record-sharing-drop-down.png)

1. Klik **sparen**.

   Personen hebben niet langer de aangegeven machtigingen voor de record. Ze hebben echter nog steeds machtigingen voor het recordtype en de werkruimte, tenzij u ze ook van deze machtigingen verwijdert.

   Er is geen bericht voor de gebruikers die uit de toegang tot van het verslag zijn verwijderd dat zij niet meer deze toestemmingen hebben.
