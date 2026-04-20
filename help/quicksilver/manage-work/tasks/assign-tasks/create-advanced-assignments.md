---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Geavanceerde toewijzingen maken
description: U kunt taken beheren of taken uitgeven gebruikend Geavanceerde Toewijzingen.
author: Lisa
feature: Work Management, Resource Management
role: User
exl-id: 09780f78-4eb8-404d-859b-d066d462776d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: daaa13d5a3ebbd249f0093181ee7834f9db43fdb
workflow-type: tm+mt
source-wordcount: '3457'
ht-degree: 0%

---

# Geavanceerde toewijzingen maken

<!-- Audited: 11/2025-->

<!--remove the bullet indicated when we get rid of the new/old experience of editing tasks-->


<!--
<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>
-->

U kunt taken beheren of taken uitgeven gebruikend Geavanceerde Toewijzingen.

U kunt de volgende toewijzingsgegevens aanpassen bij het maken van geavanceerde toewijzingen:

* Wijs gebruikers aan de taak of de kwestie toe (dit kan buiten een geavanceerde taak worden verwezenlijkt).
* Pas het aantal uren aan dat elke toegewezen persoon is toegewezen en verdeel dit aantal.
* Bepaal welke gebruiker als eigenaar of primaire ontvanger van de taak of kwestie zou moeten worden aangewezen.
* Geef op welke rol elke gebruiker vervult wanneer hij of zij aan de taak of kwestie werkt.
* Facturatie- en kosteninformatie toevoegen op toewijzingsniveau.
* Bekijk de volgende details voor elke taak: geplande uren, totale kosten en totale opbrengsten.

>[!NOTE]
>
>Wanneer gebruikers aan het werk worden toegewezen, heeft hun beschikbaarheid volgens hun programma&#39;s invloed op de geplande en verwachte datum van taken en problemen. Voor informatie over programma&#39;s, zie [ een programma ](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md) creëren.

## Gebieden in Adobe Workfront waar u geavanceerde toewijzingen kunt maken

In dit artikel wordt beschreven hoe u toegang krijgt tot Geavanceerde toewijzingen in de taak- of uitgiftekop.

Bovendien kunt u geavanceerde toewijzingen maken in de volgende gebieden van Workfront:

* In lijsten en rapporten wanneer het gebied van Toewijzingen in de mening toont.
* In de sectie Toewijzingen wanneer u een taak bewerkt. Voor meer informatie, zie [ taken ](../../../manage-work/tasks/manage-tasks/edit-tasks.md) uitgeven. <!--When we remove the old/ new experience: take this bullet out completely; in the new Edit Task experience, this is no longer possible-->
* In de taak of de uitgiftekopbal, in het gebied van Taken.
* In het werklastevenwicht. Voor meer informatie, zie [ werk manueel toewijzen gebruikend de Balancer van de Werkbelasting ](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td> <p>Facturerings en kostensnelheden toevoegen aan taaktaken en de geavanceerde zoekopdracht gebruiken: Workflow Ultimate</p> <p>Geavanceerde toewijzingen maken: elk Workfront- of workflowpakket</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td> <p>Standard</p>
   <p>Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot taken en problemen bewerken</p>  </td> 
  </tr> 
  <tr> 
   <td>Objectmachtigingen</td> 
   <td> <p>Contribute of hoger machtigingen voor de taak of uitgave</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Geavanceerde toewijzingen maken - Workflow Ultimate-pakket

Deze indeling van Geavanceerde toewijzingen is alleen van toepassing op taken. Voor kwesties, zie [ Geavanceerde Toewijzingen creëren - alle andere pakketten ](#create-advanced-assignments--all-other-packages).

>[!NOTE]
>
>De oude Ervaring Geavanceerde Toewijzingen is het gebrek. U moet de nieuwe ervaring manueel met de knoop op het hoogste recht van het Geavanceerde venster van Toewijzingen aanzetten.
>Voor informatie over de oude ervaring, zie [ Geavanceerde Toewijzingen creëren - alle andere pakketten ](#create-advanced-assignments--all-other-packages), hieronder.

1. Ga naar het project waar u een taak wilt toewijzen.
1. Klik **Taken** of **Kwesties** in het linkerpaneel, dan klik de naam van een taak in de lijst.

   >[!TIP]
   >
   >U kunt geavanceerde taken rechtstreeks in de takenlijst plaatsen. Klik binnen het **gebied van Taken** op de zelfde lijn zoals de taak, dan klik **Geavanceerd** bij de bodem van de lijst, of het **pictogram van Mensen** in de hoger-juiste hoek van de toewijzingsdoos, om het Geavanceerde venster van Toewijzingen te openen. Ga verder met stap 5 om door te gaan met het maken van geavanceerde toewijzingen.
   >![ klik Geavanceerd of het pictogram van Mensen ](assets/access-aa-from-lists.png)

1. Klik **toewijzen aan** in het **3} gebied van Taken {in de kopbal van de taak**

   of

   Klik op een van de toegewezen namen als de taak al is toegewezen.

1. Klik **Geavanceerd**.

   ![ klik Geavanceerde ](assets/assignments-from-task-header-0825.png)

   Het venster Geavanceerde toewijzingen wordt weergegeven.

   ![ Geavanceerde het venster van Taken ](assets/advanced-assignments-031826.png)

1. Controleer indien nodig de informatie over de taakduur. Deze velden zijn allemaal alleen-weergeven van Geavanceerde toewijzingen en u kunt ze in de taak bijwerken.

   Voor informatie over de taakduur, de types van duur, de eenheden van tijd, en geplande uren, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](/help/quicksilver/manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   >[!NOTE]
   >
   >Als een gegevenskolom die u wilt weergeven niet wordt weergegeven, kunt u deze toevoegen. Zie [ toevoegen en verwijderde kolommen op de Geavanceerde lijst van Toewijzingen ](#add-and-remove-columns-on-the-advanced-assignments-list), hieronder.

1. (Optioneel) Selecteer **Uren**, **FTE**, of **Percentage** voor het bekijken van de toewijzingen.

   U kunt zien hoeveel een gebruiker in geplande uren, als percentage van hun capaciteit, of in VTE (voltijdequivalent, 0-1 schaal) wordt toegewezen. De standaardinstelling is Uren.

   Voor informatie over FTE, zie [ de voorkeur van het Beheer van het Middel ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md) vormen.

1. Klik **Nieuwe rij** om een taak aan de taak toe te voegen.

1. Klik in de **Assignee** kolom om een gebruiker of een team toe te voegen. Typ de naam van de gebruiker of het team en klik vervolgens op de naam wanneer deze in de vervolgkeuzelijst wordt weergegeven.

   >[!NOTE]
   >
   >Als de naam een speciaal teken bevat, moet u het speciale teken in het zoekveld opnemen.

   Wanneer u een gebruiker toevoegt die een primaire baanrol heeft, dan wordt de **Rol van de Ontvanger** bevolkt.

   Als aan de gebruiker kenmerken zijn toegewezen aan hun profiel, worden deze in de taaktoewijzing ingevuld.

1. Om een baanrol toe te voegen wanneer u niet de gebruiker kent die aan de taak zal werken, klik in de **kolom van de Rol 0} Toegewezen {.** Typ de naam van de taakrol en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   >[!NOTE]
   >
   >Als de naam een speciaal teken bevat, moet u het speciale teken in het zoekveld opnemen.

   Als de baanrol attributen heeft die van de tariefkaart van een project worden toegewezen, worden de attributen bevolkt op de taaktoewijzing.

   Wanneer u later een gebruiker toewijst met het veld Toegewezen, volgt de basiszoekopdracht het volgende algoritme:

   * Volledige overeenkomst: de rol van de baan en alle attributen
   * Gedeeltelijke overeenkomst: taakrol en enkele kenmerken
   * Alleen taakrollen

   Voor informatie over het geavanceerde onderzoek, zie [ Gebruik het geavanceerde onderzoek ](#use-the-advanced-search) in dit artikel.

1. (Optioneel) Voeg desgewenst toewijzingen toe aan nieuwe rijen om meerdere bronnen aan de taak toe te voegen.

   >[!TIP]
   >
   >* U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen. Er zijn maximaal 200 toewijzingen per taak toegestaan.
   >
   >
   >* Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Als een gebruiker, een baanrol, of een team werden toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >   
   >   * Wijs het werkitem opnieuw toe aan actieve bronnen.
   >   * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

1. Om een toegewezen als taakeigenaar te merken, selecteer de controledoos voor de rij, en klik **Vastgestelde primaire** in de actiebar bij de bodem van het Geavanceerde venster van Toewijzingen.

   Standaard markeert Workfront de eerste gebruiker- of taakrol die u aan een taak toewijst als de Eigenaar of Primaire Toewijzing. Een team kan niet worden aangewezen als primaire eigenaar van een taak.

   Als de Primaire Eigenaar van de taak niet wordt getoond, kunt u **toevoegen is Primaire** kolom aan de lijst.

   >[!IMPORTANT]
   >
   >Afhankelijk van hoe uw Workfront-beheerder of groepsbeheerder uw projectvoorkeuren heeft ingesteld, kan Workfront het schema van de taakeigenaar gebruiken om de tijdlijn van de taak te berekenen wanneer meerdere gebruikers aan de taak zijn toegewezen. Voor informatie over veelvoudige taaktoegewezen, zie de [ Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers ](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) sectie in het artikel [ toewijzen taken ](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

1. Voor elke gebruiker in de **Assignee** kolom, specificeer de volgende informatie:

   * (Facultatief) **rol van de Baan voor het factureren**: Onderzoek naar en selecteer de baanrol voor het factureren voor deze specifieke ontvanger en taak.

     De taakrol voor facturering wordt alleen gebruikt voor deze toewijzing en wordt niet automatisch toegepast op de andere toewijzingen van de gebruiker. De primaire functie van een gebruiker is bijvoorbeeld Designer, maar in één taak fungeert hij als Senior Designer en de factureringsgraad moet dat weerspiegelen. De taakrol voor facturering is alleen van toepassing op gebruikers en kan niet worden gebruikt voor andere functies.

     Wanneer een baanrol voor het factureren op de gebruikerstaak wordt toegepast, kan het tarief verbonden aan de baanrol voor het factureren in plaats van de gebruikers of baanroltarieven in het facturerings en opbrengstberekeningen worden gebruikt.

     Een de baanrol op projectniveau voor het factureren kan ook voor een gebruiker worden geplaatst, en die waarde wordt gebruikt op alle taken van de gebruiker op dat project.

     Voor meer informatie, zie [ Opstelling een Rol van de Baan voor het Factureren ](/help/quicksilver/manage-work/projects/project-finances/set-up-job-role-for-billing.md).

   * **Toewijzing**: Wanneer het Type van Duur van een taak Eenvoudig is, specificeer het aantal uren elke gebruiker of baanrol aan de taak zou moeten worden toegewezen. De som van alle toegewezen uren voor elke gebruiker is gelijk aan het aantal op het **Geplande Uren** gebied bij de bovenkant van het Geavanceerde venster van Toewijzingen. In alle andere gevallen geeft u het percentage aan tijd (of toewijzing) op dat de toegewezen persoon moet besteden aan het oplossen van de taak.

     >[!TIP]
     >
     >Nadat u de toewijzing van taken handmatig hebt gewijzigd, kunnen de geplande uren van de taken dienovereenkomstig worden bijgewerkt. Merk op dat u geen toewijzingen voor teams kunt manueel wijzigen die aan taken worden toegewezen. Voor meer informatie, zie de sectie [ Geplande taak van de Update Uren wanneer het beheren van gebruikerstoewijzingen ](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) in het artikel [ Geplande overzicht van Uren ](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).

   * **Attributen**: Om het even welke attributen beschikbaar voor de gebruiker worden getoond op de attributengebieden. De beheerder stelt de kenmerken in en deze worden toegevoegd aan het gebruikersprofiel of gekoppeld aan een taakrol in een tariefkaart. Voor meer informatie, zie [ tariefattributen ](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md) bepalen en [ geef het profiel van een gebruiker ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uit.

     Kenmerken zijn momenteel alleen-lezen bij gebruikerstoewijzingen. Ze zijn bewerkbaar voor functies.

   * **de munteenheid van het Tarief**: De valuta voor het factureren en kostentarieven wordt in gebreke gesteld van het project, maar u kunt de munt voor deze taak veranderen.

   * (Facultatief) **het Facturerings tarief**: Het factureringstarief kan uit andere gebieden van het systeem, zoals tariefkaarten komen. Voor meer informatie, zie [ Overzicht van opbrengst en kostenhiërarchie ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). U kunt de factureringssnelheid voor deze specifieke toewijzing op dit gebied manueel met voeten treden, en het zal alle andere tarieven voor de gebruiker in opbrengstberekeningen met voeten treden.
   * (Facultatief) **Tarief van Kosten**: Het kostentarief kan uit andere gebieden van het systeem komen. Voor meer informatie, zie [ Overzicht van opbrengst en kostenhiërarchie ](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md). U kunt de kostenvoet voor deze specifieke taak op dit gebied manueel met voeten treden, en het zal alle andere tarieven voor de gebruiker in kostenberekeningen met voeten treden.
   * **is Billable**: Selecteer deze optie om de taak in financiële berekeningen te omvatten. Schakel deze optie uit om de toewijzing uit te sluiten van financiële berekeningen.

     Dit veld is standaard ingeschakeld voor alle toewijzingen wanneer de taak een type inkomsten heeft.

1. (Facultatief) om toewijzingsgegevens door datum voor een gebruiker of een rol te bekijken, selecteer de lijstrij en klik **Mening tegen data** in de actiebar bij de bodem van het Geavanceerde venster van Toewijzingen. Voor meer informatie, zie [ de taakgegevens van de Mening door data ](#view-assignment-data-by-dates) in dit artikel.
1. (Facultatief) om één of meerdere taken van de lijst te schrappen, de controledoos voor elke rij te selecteren, en **Schrapping** in de actiebar bij de bodem van het Geavanceerde venster van Toewijzingen te klikken.
1. Klik **sparen** of **sparen en sluit** wanneer u gebeëindigd het uitgeven van de Geavanceerde Toewijzingen bent.

### Kolommen toevoegen en verwijderen in de lijst Geavanceerde toewijzingen

Velden moeten bestaan voordat u ze aan de lijst kunt toevoegen.

1. Klik **+** op het hoogste recht van de lijst om de **manager van de Kolom** te openen.

   ![ Geavanceerde Manager van de Kolom van Toewijzingen ](assets/aa-column-manager.png)

1. Selecteer het **lusje van Eigenschappen** of het **KPIs** lusje om het type van gebied te kiezen u wilt toevoegen.

   Eigenschappen zoals locatie of kostenplaats bieden contextuele informatie. KPI&#39;s met tijdfasering, zoals inkomsten of kostenonderverdelingen, zijn onderverdeeld in waarden over tijdsperiodes.

1. Onderzoek naar een bestaand objecten gebied in de **Beschikbare** sectie, dan klik **+** rechts van het gebied naam het om het aan de **Geselecteerde** kolom toe te voegen.
1. Klik **-** rechts van een gebied in de **Geselecteerde** sectie om het uit de lijst te verwijderen.
1. Klik **sparen**.

   Voor meer informatie over de manager van de Kolom, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Een weergave toepassen op de lijst Geavanceerde toewijzingen

Een weergave is een gepersonaliseerde set kolomregelingen die u op de lijst kunt toepassen.

1. Klik de **drop-down Meningen** en selecteer de mening u op de lijst wilt toepassen.

   {de Weergaven van het 0} Systeem **zijn meningen die de systeembeheerder toevoegde, en zij kunnen niet worden veranderd.** **Mijn Meningen** zijn meningen die u creeerde of met u werd gedeeld.

1. Klik **Nieuwe mening** in **Meningen** dropdown om een mening tot stand te brengen.

   Wanneer u de kolommen toevoegt, verwijdert of opnieuw rangschikt, worden de wijzigingen automatisch in de weergave opgeslagen. De volgende keer dat u deze weergave toepast, blijven de kolommen behouden zoals u ze instelt.

   Voor meer informatie over meningen, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### De geavanceerde zoekopdracht gebruiken

Met de geavanceerde zoekopdracht kunt u de juiste gebruiker of taakrol zoeken die u aan de toewijzing wilt toevoegen.

1. Voer een van de volgende handelingen uit om het geavanceerde zoekvenster te openen:

   * Klik **Geavanceerd Onderzoek** bij het hoogste recht van het Geavanceerde venster van Toewijzingen.
   * Selecteer een toewijzingsrij en klik **Geavanceerd Onderzoek** in de actiebar bij de bodem van het Geavanceerde venster van Toewijzingen. Hierdoor wordt de geavanceerde zoekopdracht geopend met filters die automatisch worden toegepast op die specifieke toewijzing.

1. Selecteer het tabblad Gebruikers of Taakrollen in het geavanceerde zoekvenster.
1. Pas de filters naar wens toe:

   1. Klik **Filter** boven de lijst.
   1. In de doos van de Filter, klik **toevoegt voorwaarde**.
   1. Selecteer een veld waarop u wilt filteren.
   1. Selecteer een filtermodifier, zoals &quot;Heeft een van de opties,&quot; &quot;Heeft geen van de opties&quot;, &quot;Is ervoor&quot; of &quot;Is erna&quot;. De opties voor wijzigingstoetsen zijn afhankelijk van het type veld waarop u filtert.
   1. Selecteer de veldwaarde(n). Afhankelijk van het veldtype waarop u filtert, wordt u mogelijk gevraagd het item in een lijst te selecteren, ernaar te zoeken of een kalender te gebruiken om een datumbereik te selecteren.

   Het filter wordt automatisch toegepast op de lijst. Voor meer informatie over filters, zie [ Gebruik verbeterde lijsten ](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

1. Zoeken naar een taakrol of gebruiker.

   Bij het zoeken naar een gebruiker die een taakroltoewijzing aanpast, worden alleen volledige overeenkomsten (taakrol en alle kenmerken) weergegeven.

1. Klik **+** om kolommen aan de lijst toe te voegen. Voor meer informatie, zie [ kolommen op de Geavanceerde lijst van Toewijzingen toevoegen en verwijderen ](#add-and-remove-columns-on-the-advanced-assignments-list).
1. Selecteer één of meerdere gebruikers of baanrollen, en de klik **voegt Gebruikers** toe of **voegt Rollen** in de actiebar bij de bodem van het venster toe.

   De toewijzingen worden toegevoegd in het venster Geavanceerde toewijzingen.

### Toewijzingsgegevens op datums weergeven

De **Mening door data** venster voor Geavanceerde Taken toont de volledige datum-efficiënte geschiedenis van de taak voor een specifieke gebruiker of een rol. Zowel oude als toekomstige wijzigingen worden weergegeven.

Voorbeelden van datumeffectieve items die de toewijzingsgeschiedenis kunnen beïnvloeden zijn:

* De primaire/andere taakrollen van de gebruiker
* Functie op projectniveau voor facturering
* Facturering/kosten gebruikersprofiel
* Facturerings-/kostenpercentages voor het overschrijven van projecten (gebruiker- of taakrol)
* Creditcardtarieven op taakrol/kenmerken
* Gebruikerskenmerken
* Gebruikersschema

Merk op dat dit geen uitvoerige lijst is, en het gebied dat verandert niet noodzakelijk in de lijst van toewijzingsgegevens wordt getoond, maar het beïnvloedt het factureren en kostentarieven of de attributen voor de gebruiker of baanrol.

U kunt toewijzingsgegevens alleen op datums weergeven voor één gebruiker of rol.

1. Selecteer de lijstrij voor een gebruiker of een rol, en klik **Mening tegen data** in de actiebar bij de bodem van het Geavanceerde venster van Toewijzingen.

   Het **Mening door data** venster verschijnt. De gegevens zijn alleen-lezen.

   Elke rij in de tabel vertegenwoordigt een datum-effectieve wijziging in de toewijzing. Als er geen datum-effectieve wijzigingen zijn aangebracht, bevat de tabel één rij met de huidige gegevens. Gemarkeerde velden geven aan wat is gewijzigd en de begin- en einddatum voor elke update worden vermeld. Als bijvoorbeeld de factureringssnelheid op 21 augustus van 202 tot 205 is veranderd, wordt de frequentie gemarkeerd. De tekst tussen haakjes geeft aan waar de wijziging in de frequentie is aangebracht, zoals een project.

   ![ Mening door datumvenster ](assets/resource-changes-view-by-dates.png)

   Wanneer u de gegevens hebt gecontroleerd, klikt u op de pijl linksboven om terug te keren naar het venster Geavanceerde toewijzingen.

## Geavanceerde toewijzingen maken - alle andere pakketten

Deze indeling van Geavanceerde toewijzingen is van toepassing op zowel taken als problemen.

1. Ga naar het project waar u een taak of een kwestie wilt toewijzen.
1. Klik **Taken** of **Kwesties** in het linkerpaneel, dan klik de naam van een taak of kwestie in de lijst.

   >[!TIP]
   >
   >U kunt geavanceerde taken rechtstreeks in de taak- of uitgavelijst plaatsen. Klik binnen het **gebied van Taken** op de zelfde lijn zoals de taak of de kwestie, dan klik **Geavanceerd** bij de bodem van de lijst, of het **pictogram van Mensen** in de hoger-juiste hoek van de toewijzingsdoos, om het Geavanceerde venster van Toewijzingen te openen. Ga verder met stap 5 om door te gaan met het maken van geavanceerde toewijzingen.
   >![ klik Geavanceerd of het pictogram van Mensen ](assets/access-aa-from-lists.png)

1. Klik **toewijzen aan** in het **3} gebied van Taken {in de kopbal van de taak of de kwestie**

   of

   Klik op een van de toegewezen namen als de taak of uitgave al is toegewezen.

1. Klik **Geavanceerd**.

   ![ klik Geavanceerde ](assets/assignments-from-task-header-0825.png)

1. Op de **mensen van het Onderzoek, de rol en het teamgebied**, begin de naam van een gebruiker, een rol, of een team te typen, dan de naam te klikken wanneer het in de drop-down lijst verschijnt.

   >[!NOTE]
   >
   >Als de naam van de gebruiker een speciaal teken bevat, moet u het speciale teken in het zoekveld opnemen.

1. (Optioneel) Ga door met het toevoegen van toewijzingen in het **vak Personen, Rol en Teams** om meerdere bronnen aan de taak of kwestie toe te voegen.

   >[!TIP]
   >
   >* U kunt meerdere gebruikers, taakrollen of teams toewijzen. U kunt alleen actieve gebruikers, taakrollen en teams toewijzen.
   >
   >
   >* Wanneer u een gebruikerstoewijzing toevoegt, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen.
   >Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.
   >De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie [ toegang van de Verlening tot gebruikers ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
   >
   >
   >* Als een gebruiker, een baanrol, of een team werden toegewezen alvorens zij werden gedeactiveerd, blijven zij toegewezen aan het het werkpunt. In dit geval raden we het volgende aan:
   >   
   >   * Wijs het werkitem opnieuw toe aan actieve bronnen.
   >   * Koppel de gebruikers in een gedeactiveerd team aan een actief team en wijs het het werkpunt aan het actieve team opnieuw toe.

1. Voor elke gebruiker in de **Assignee** kolom, specificeer de volgende informatie:

   * **Eigenaar**: Beweeg over de naam van toegewezen en klik **Primair maken** op het gebied van de Eigenaar als u toegewezen als taak of uitgeverseigenaar wilt merken. Een groen selectievakje geeft aan dat de opgegeven gebruiker de primaire contactpersoon van de taak of uitgave is. Adobe Workfront markeert de eerste gebruiker of baanrol die u aan een taak of kwestie als Eigenaar of Primaire Toewijzing toewijst. Een team kan niet worden aangewezen als primaire eigenaar van een taak of uitgave.

     >[!IMPORTANT]
     >
     >Afhankelijk van hoe uw Workfront-beheerder of groepsbeheerder uw projectvoorkeuren heeft ingesteld, kan Workfront het schema van de taakeigenaar gebruiken om de tijdlijn van de taak te berekenen wanneer meerdere gebruikers aan de taak zijn toegewezen. Voor informatie over veelvoudige taaktoegewezen, zie de [ Overwegingen voor veelvoudige taken aan baanrollen, teams, en gebruikers ](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md#considerations-for-multiple-assignments-to-job-roles-teams-and-users) sectie in het artikel [ toewijzen taken ](../../../manage-work/tasks/assign-tasks/assign-tasks.md).

   * **Toewijzingen**: Wanneer het Type van Duur van een taak Eenvoudig is, specificeer het aantal uren elke gebruiker of baanrol aan de taak zou moeten worden toegewezen. De som van alle toegewezen uren voor elke gebruiker is gelijk aan het aantal op het **Geplande Uren** gebied bij de bodem van de kolom van Toewijzingen. In alle andere gevallen geeft u het percentage aan tijd (of toewijzing) op dat de toegewezen persoon moet besteden aan het oplossen van de taak of kwestie.

     >[!TIP]
     >   
     >   * Nadat u de toewijzing van taken handmatig hebt gewijzigd, kunnen de geplande uren van de taken dienovereenkomstig worden bijgewerkt. Voor meer informatie, zie de sectie [ Geplande taak van de Update Uren wanneer het beheren van gebruikerstoewijzingen ](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md#update-task-planned-hours-when-managing-user-allocations) in het artikel [ Geplande overzicht van Uren ](/help/quicksilver/manage-work/tasks/task-information/planned-hours.md).
     >   * U kunt toewijzingen niet handmatig wijzigen bij uitgaven.
     >   * U kunt toewijzingen voor teams die aan taken zijn toegewezen niet handmatig wijzigen.

   * **Rol van de Ontvanger:** selecteer de rol de gebruiker zou moeten gebruiken wanneer het vervullen van deze taak.  Standaard wordt de primaire rol van de gebruiker weergegeven. Klik in het **vakje van de Rol van 0} toewijzen {om een andere rol te selecteren.** Wanneer u eerst de taak of de kwestie aan een rol toewijst, en dan een gebruiker toevoegt die die rol als tweede taak kan vervullen, wordt de lijst van voorgestelde gebruikers gefiltreerd voor de gebruikers die de rollen kunnen vervullen die reeds aan de taak en de kwestie worden toegewezen.

     ![ Rol van de Ontvanger ](assets/advanced-assignments-select-role.png)

   * **Type van Duur**: Dit is slechts beschikbaar voor taken. Klik de naam van het Type van Duur en selecteer een Type van Duur van het drop-down menu. Voor informatie over de Types van Duur, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

   * **Duur:** u kunt dit gebied voor een taak bijwerken wanneer u beheertoestemmingen aan de taak hebt.

     Voor meer informatie, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md). Bij het bewerken van grote hoeveelheden toewijzingsgegevens wordt een vergelijkbaar dialoogvenster weergegeven waarin gebruikers, uren, toewijzing en taakeigenaar worden toegewezen.

   * **Geplande Uren**: Wanneer het Type van Duur Toewijzing of Eenvoudig wordt berekend, werk het aantal Geplande Uren bij. De toewijzingspercentages of de uren voor elke bron worden als gevolg hiervan gelijkmatig verdeeld. Workfront berekent de geplande uren wanneer het Duur-type Berekend Werk of Gedreven Inspanning is. Voor meer informatie, zie [ Overzicht van het Type van Duur en van de Duur van de Taak ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

1. Klik **sparen**.


