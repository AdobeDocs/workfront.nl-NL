---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
title: Een goedkeuringsproces bewerken
description: Als u een Adobe Workfront-beheerder bent of als u beheerdersrechten hebt voor goedkeuringsprocessen, kunt u alle goedkeuringsprocessen in het systeem zien en bewerken.
author: Alina
feature: System Setup and Administration, Approvals
role: Admin
exl-id: 62aa8ac0-7e8a-4df6-b5d4-a32fa86a4597
source-git-commit: ea1ac823fc414608f5205ac5bd9f29c1209fb7dc
workflow-type: tm+mt
source-wordcount: '1950'
ht-degree: 0%

---

# Een goedkeuringsproces bewerken

Als u een Adobe Workfront-beheerder bent of als u beheerdersrechten hebt voor goedkeuringsprocessen, kunt u alle goedkeuringsprocessen in het systeem zien en bewerken.

Als u een groepsbeheerder bent, kunt u de goedkeuringsprocessen zien en uitgeven verbonden aan de groep of de groepen u leiden.

Voor informatie over het creëren van goedkeuringsprocessen, zie [ een goedkeuringsproces voor het werkpunten ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.

>[!NOTE]
>
>* Wanneer u een algemeen goedkeuringsproces uitgeeft dat reeds in gebruik is, beïnvloeden uw veranderingen alle voorwerpen door het systeem die reeds met het worden geassocieerd.
>* Als u een nieuwe fiatteur aan het huidige stadium op een goedkeuringsproces toevoegt dat reeds op een voorwerp is begonnen, moet het proces voor dat voorwerp terugstellen en de fiatteurs opnieuw beginnen.
>
>  Als u echter de volgende wijzigingen aanbrengt in een goedkeuringsproces dat al op een object is gestart, wordt dat proces zonder onderbreking voortgezet:
>
>* Een werkgebied toevoegen na het huidige werkgebied
>* Een extra fiatteur toevoegen voor het huidige werkgebied

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot Goedkeuringsprocessen als u geen systeembeheerder bent</p> <p><b> NOTA </b>: Als u nog geen toegang hebt, vraag uw beheerder van Workfront als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

+++

## Een bestaand goedkeuringsproces bewerken

{{step-1-to-setup}}

1. (Voorwaardelijk) als u een systeem-vlakke goedkeuringsproces uitgeeft, klik **Processen** > **goedkeurt** in het linkerpaneel.

   of

   Als u een goedkeuringsproces op groepsniveau bewerkt, doet u het volgende:

   1. In het linkerpaneel, klik **Groepen** ![](assets/groups-icon.png).
   1. Klik op de naam van de groep waarvoor u de goedkeuringsprocessen voor groepen wilt weergeven of beheren.
   1. In het linkerpaneel, klik **goedkeurt**. U zou kunnen moeten klikken **tonen meer** eerst.

1. Klik de **Goedkeuringen van het Project**, **Taak goedkeurt**, of **Kwestie goedkeurt** lusje, afhankelijk van het type van goedkeuringsproces u wilt uitgeven.

1. Selecteer het goedkeuringsproces u wilt uitgeven, dan klik **uitgeven** bij de bovenkant van de lijst. Het vak Goedkeuringsproces bewerken wordt weergegeven.

   ![](assets/edit-approval-process-global-area-new.png)

1. Geef de volgende informatie op in het vak dat wordt weergegeven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam goedkeuringsproces</td> 
      <td>Typ een beschrijvende naam voor het goedkeuringsproces. De gebruikers zien deze naam wanneer het toepassen van het goedkeuringsproces op een voorwerp, zoals die in <a href="../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md" class="MCXref xref"> wordt beschreven associëren een nieuw of bestaand goedkeuringsproces met het werk </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ een beschrijving van het goedkeuringsproces. Dit toont in de <b> goedkeurt </b> sectie in het <b> gebied van de Opstelling </b> naast de naam van het goedkeuringsproces.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Is actief</td> 
      <td> <p>Houd deze optie ingeschakeld als u wilt dat andere gebruikers het goedkeuringsproces kunnen koppelen aan projecten, taken en problemen die zij maken. </p> <p>Deze optie is standaard ingeschakeld.</p> <p>Tip: een goedkeuringsproces inactief markeren is handig wanneer uw organisatie het niet langer hoeft te gebruiken, maar u historische informatie over het gebruik ervan wilt behouden.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Dit goedkeuringsproces kan worden gebruikt door </td> 
      <td> <p>Als u het goedkeuringsproces beschikbaar voor projecten, taken, kwesties, en malplaatjes wilt die tot slechts tot een bepaalde groep behoren, begin de naam van de groep te typen, dan selecteer de naam wanneer het verschijnt:</p> 
       <ul> 
        <li>Als u een systeembeheerder bent of administratieve toegang tot goedkeuringsprocessen hebt, kunt u om het even welke groep in het systeem zien wanneer u zijn naam typt. <b> Alle groepen </b> wordt geselecteerd door gebrek. </li> 
        <li>Als u een groepsbeheerder zonder administratieve toegang tot goedkeuringsprocessen bent, kunt u het goedkeuringsproces aan om het even welke groep toewijzen u beheert wanneer u zijn naam typt. De <b> Alle Groepen </b> optie is niet beschikbaar.</li> 
       </ul> <p>Deze optie is niet beschikbaar voor goedkeuringsprocedures voor eenmalig gebruik.</p> <p><b> WAARSCHUWING </b>: Wanneer u veranderingen in het groep-specifieke goedkeuringsproces aanbrengt, zouden de bestaande goedkeuringsprocessen die reeds met het werkpunten zijn geassocieerd kunnen veranderen. Voor informatie over deze veranderingen, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref"> hoe de groep en de veranderingen van het goedkeuringsproces toegewezen goedkeuringsprocessen </a> beïnvloeden.</p> <p>Voor informatie over het een lijst maken van en het beheren van de goedkeuringsprocessen van uw groep van de pagina van uw groep, zie <a href="../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md" class="MCXref xref"> groep-vlakke goedkeuringsprocessen </a>. </p> <p>Voor informatie over administratieve toegang tot goedkeuringsprocessen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref"> gebruikers administratieve toegang van de Verlening tot bepaalde gebieden </a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Vorm een weg voor het goedkeuringsproces gebruikend de volgende opties.

   In een pad geeft u op wat er moet gebeuren tijdens het goedkeuringsproces. U maakt fasen in een pad om aan te geven wie de goedkeuring moet uitvoeren en in welke volgorde.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Goedkeuringsproces starten wanneer de status is ingesteld op</p> </td> 
      <td> <p>Selecteer de status die het goedkeuringsproces voor werkitems activeert. Wanneer iemand een tijdelijk onderdeel aan deze status bijwerkt, wordt het goedkeuringsproces gestart. </p> <p>Dezelfde status kan niet worden geselecteerd voor meerdere goedkeuringsprocespaden.</p> <p>De beschikbare statussen zijn gebaseerd op wat onder de optie <b> wordt geselecteerd Deze goedkeuring kan door </b> worden gebruikt (verklaard in de lijst hierboven):</p> 
      <ul> 
      <li> Als <b> Alle groepen </b> wordt geselecteerd, slechts zijn de systeem-brede gesloten statussen beschikbaar. <!--Remove "locked" when story about using an unlocked status in approval processes goes to preview-->
      </li> 
      <li> <p>Als een specifieke groep is geselecteerd, zijn alleen de statussen beschikbaar voor die groep</p> </li> 
      </ul> <p>Voor informatie over hoe het goedkeuringsproces met statussen werkt, zie de sectie <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref"> hoe de goedkeuringsprocessen zich op statussen </a> in het het procesoverzicht van het artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref"> goedkeuringsproces </a> baseren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werkgebiednaam</td> 
      <td>(Optioneel) Typ een naam die de eerste fase van het pad beschrijft. Als u geen werkgebiednaam specificeert, is de standaardnaam <b> Stadium 1 </b>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fiatteurs</td> 
      <td> <p>Typ de naam van de gebruiker, het team of de taakrol die u wilt toewijzen als fiatteur voor dit werkgebied en klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst. U kunt alleen actieve gebruikers, taakrollen en teams toevoegen. </p>

   <p><b> TIP </b>:</p>

   <p>Wanneer u een gebruiker toevoegt als fiatar, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres om onderscheid te maken tussen gebruikers met identieke namen. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze toevoegt.</p>
      <p>De instelling Contactinfo weergeven moet zijn ingeschakeld op uw toegangsniveau zodat gebruikers de e-mails van gebruikers kunnen bekijken. Voor informatie, zie <a href="../../add-users/configure-and-grant-access/grant-access-other-users.md"> Toegang van de Verlening tot gebruikers </a></p>.

   <p><b> NOTA </b>:

   Als u een gebruiker, team of rol als fiatteur toevoegt, geeft u deze niet automatisch machtigingen voor het object dat aan die goedkeuring is gekoppeld. Ze ontvangen machtigingen voor het object wanneer de goedkeuringsstap wordt geactiveerd. Anders moeten de objecten met hen worden gedeeld voordat ze een goedkeuringsbesluit kunnen nemen. </p>
   <p>U kunt een persoon ook als fiatteur aanwijzen door de rol van het individu op te geven. U kunt bijvoorbeeld een projecteigenaar, projectsponsor, eigenaar van Portfolio, programmaeigenaar of beheerder toewijzen als fiatteur. Deze opties worden automatisch weergegeven wanneer u begint te typen.</p> 
      <p><b> BELANGRIJK </b>:  
      <ul> 
      <li> Wanneer u een goedkeuring toewijst aan de projectsponsor en niemand als sponsor van een project is aangewezen, wordt de goedkeuring opnieuw toegewezen aan de eigenaar van het project. Als niemand als eigenaar van het project wordt aangewezen, wordt de goedkeuring toegewezen aan de beheerder van Workfront. </li> 
      <li> Wanneer u een goedkeuring aan een rol toewijst en de optie <b> Approver die niet op het projectteam </b> moet zijn wordt vereist gehandicapt, maar geen rollen in het projectteam passen de rol op de goedkeuring aan, wordt de goedkeuring opnieuw toegewezen aan de Eigenaar van het Project. Voor informatie over goedkeuringsmontages, zie <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md" class="MCXref xref"> globale goedkeuringsmontages </a> vormen.
      </li> 
      <li>Wanneer u een goedkeuring toewijst aan de Eigenaar van het Project en niemand als eigenaar van een project wordt aangewezen, wordt de goedkeuring opnieuw toegewezen aan de belangrijkste beheerder van Workfront zoals die in de sectie van de Info van de Klant in het gebied van de Opstelling wordt vermeld. Voor informatie, zie <a href="../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md" class="MCXref xref"> basisinformatie voor uw systeem </a> vormen.</li> 
      <p><img src="assets/approval-create-add-users-nwe-350x304.png"></p> 
      <li><p>Wanneer u baanrollen als fiatteurs toewijst, kunnen alle gebruikers verbonden aan die baanrol die ook op het projectteam is een besluit over de goedkeuring nemen. </p> 
      <p>Wanneer u een team als fiatteur toewijst, kan om het even welke gebruiker in dat team een besluit over de goedkeuring nemen. </p> 
      <p>Voor meer informatie over het projectteam, zie <a href="../../../manage-work/projects/planning-a-project/project-team-overview.md" class="MCXref xref"> Overzicht van het Team van het Project </a>. Voor meer informatie over het goedkeuren van het werk, zie <a href="../../../review-and-approve-work/manage-approvals/approving-work.md" class="MCXref xref"> het goedkeuren van het werk </a>.</p>
      </li>
      </ul>  
      </td> 
   </tr> 
     <tr> 
      <td role="rowheader">Slechts één besluit is vereist</td> 
      <td>(Wordt alleen weergegeven als u meerdere fiatteurs aan het werkgebied toevoegt) Selecteer deze optie als een van de fiatteurs in het werkgebied het werkitem tijdens dit werkgebied kan goedkeuren of afwijzen. Hierdoor kan het werkitem het werkgebied verlaten.  
      <p>Als deze optie niet is geselecteerd, moeten alle geïdentificeerde fiatteurs het werkgebied (in willekeurige volgorde) goedkeuren of afwijzen voordat het item het werkgebied verlaat. Als een van de fiatteurs het werkgebied afwijst, wordt het proces onderbroken en begint het opnieuw, zodat de vereiste wijzigingen kunnen worden aangebracht. Daarna kunnen de fiatteurs het werkgebied opnieuw goedkeuren of afwijzen.</p> 
      <p>Wanneer een team als fiatteur wordt aangewezen, kan om het even welk lid van het team een stadium verlenen of verwerpen.</p> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">Werkgebied toevoegen</p> </td> 
      <td>(Optioneel) Voeg nog een werkgebied aan het pad toe met de opties die in de drie bovenstaande rijen worden beschreven. U kunt zo veel fasen aan het pad toevoegen als u nodig hebt.</td> 
     </tr>
     <tr> 
      <td role="rowheader"> Kiezen wat er gebeurt wanneer de goedkeuring wordt geweigerd</td> 
      <td> <p>Selecteer de actie die u wilt uitvoeren als het werkitem in een van de fasen van het pad wordt afgewezen:</p> 
      <ul> <li><strong> creeer een Kwestie </strong>: (Beschikbaar slechts voor project en taakgoedkeuringsprocessen) Een kwestie wordt gecreeerd in het project of de taak waar het goedkeuringsproces loopt. De standaard toegewezen bron op de taak, of de eigenaar van het project wordt toegewezen aan de kwestie. Door gebrek, is de naam van de gecreeerde kwestie <strong> Afgewezen Goedkeuring (Project of Naam van de Taak) </strong>. Dit is een afwijzingsprobleem dat onder de taak of het project is aangegaan, afhankelijk van het goedkeuringsproces waarbij de afkeuring heeft plaatsgevonden.</li> 
      <li> <p><strong> plaats Status aan </strong>: Kies één van het volgende:</p> 
      <ul> <li><strong> Vorige Status </strong>: Het verworpen project, de taak, of de kwestie keert aan de status voorafgaand aan de status terug die het goedkeuringsproces activeert.</li> 
      <li> <p><strong> om het even welke andere status in de lijst </strong>: De verworpen objecten bewegingen aan de status u, zoals op Greep kiest. U kunt een van de standaardstatussen kiezen of een aangepaste status die u aan uw Workfront-systeem hebt toegevoegd.</p> <p>Als u een status selecteert die aan een goedkeuringsproces is gekoppeld als de afwijzingsstatus voor een goedkeuringspad, wordt het geweigerde object naar de geselecteerde status verplaatst en wordt deze gemarkeerd als "In afwachting van goedkeuring".</p>
      <p>Als u bijvoorbeeld In de wachtstand selecteert voor de afwijzingsstatus en de status In de wachtstand is gekoppeld aan een goedkeuringsproces, wordt het geweigerde object in de status "In de wachtstand gezet voor goedkeuring" geplaatst, waarvoor goedkeuring is vereist.</p>    <p>Voor een systeembreed goedkeuringsproces zijn alleen statussen voor het hele systeem beschikbaar.</p> <p>Voor een groepsspecifiek goedkeuringsproces zijn alle groepsstatussen beschikbaar. Dit omvat om het even welke douanestatus die de groepsbeheerder specifiek voor de groep, evenals om het even welke status voor het hele systeem creeerde. </p> <p>Voor informatie over hoe het goedkeuringsproces met statussen werkt, zie de sectie <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md#how2" class="MCXref xref"> hoe de goedkeuringsprocessen zich op statussen </a> in het het procesoverzicht van het artikel <a href="../../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md" class="MCXref xref"> goedkeuringsproces </a> baseren.</p> </li>
      </ul> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) klik **toevoegen weg** om een andere weg aan het goedkeuringsproces toe te voegen, verwijzend naar de lijst van opties in de vorige stap.

   Het nieuwe pad moet aan een andere status zijn gekoppeld. Het pad wordt geactiveerd wanneer het item wordt bijgewerkt om deze status weer te geven. U kunt voor dezelfde status geen twee paden hebben.

1. Klik **sparen**.
1. (Optioneel) Voer een van de volgende handelingen uit:

   * Associeer het goedkeuringsproces met specifieke projecten, taken, of kwesties door uw systeem, zoals die in [ wordt beschreven associeer een nieuw of bestaand goedkeuringsproces met het werk ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Buiten Workfront, breng gebruikers op de hoogte dat het goedkeuringsproces voor hen beschikbaar is om met hun projecten, taken, of kwesties te associëren, zoals die in [ worden beschreven associeer een nieuw of bestaand goedkeuringsproces met het werk ](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
   * Maak een ander goedkeuringsproces dat wordt geactiveerd als dit goedkeuringsproces wordt geweigerd en het onderdeel een andere status krijgt. Op deze manier kunt u goedkeuringsprocessen aan elkaar koppelen.
