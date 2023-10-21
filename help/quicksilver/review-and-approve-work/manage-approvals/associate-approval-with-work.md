---
product-area: projects
navigation-topic: approvals
title: Een nieuw of bestaand goedkeuringsproces koppelen aan werk
description: In dit artikel wordt beschreven hoe u goedkeuringsprocessen aan werkitems kunt koppelen. Zie de volgende artikelen voor informatie over het koppelen van goedkeuringen aan proefdrukken of documenten.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: e375408e6ccc25ff8d5c1e4f6c4fc7da2208db46
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# Een nieuw of bestaand goedkeuringsproces koppelen aan werk

In dit artikel wordt beschreven hoe u goedkeuringsprocessen aan werkitems kunt koppelen. Zie de volgende artikelen voor informatie over het koppelen van goedkeuringen aan proefdrukken of documenten:

* [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Documentgoedkeuring aanvragen](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

U kunt een globaal goedkeuringsproces of een goedkeuringsproces voor eenmalig gebruik koppelen aan een tijdelijk onderdeel in Adobe Workfront. De volgende scenario&#39;s bestaan:

* Koppel een bestaand globaal goedkeuringsproces aan een project, een taak, een kwestie, een malplaatje, of een malplaatjetaak. Alle groepen in het systeem beschikken over enkele algemene goedkeuringsprocessen. Globale goedkeuringsprocessen op groepsniveau zijn alleen beschikbaar voor bepaalde groepen.
* Creeer een enig-gebruik goedkeuringsproces en associeer het met een bestaand project, een taak, een kwestie, een malplaatje, of een malplaatjetaak.

>[!NOTE]
>
>In dit artikel wordt de term &quot;wereldwijd goedkeuringsproces&quot; gebruikt om een onderscheid te maken tussen &quot;goedkeuringsproces voor eenmalig gebruik&quot;. Een algemeen goedkeuringsproces kan herhaaldelijk worden gebruikt.
>
>De term &quot;mondiaal goedkeuringsproces op groepsniveau&quot; verwijst naar een goedkeuringsproces dat herhaaldelijk kan worden gebruikt voor artikelen en statussen die alleen aan een specifieke groep zijn gekoppeld.

Zie voor meer algemene informatie over goedkeuringsprocessen [Overzicht van goedkeuringsproces](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Voor informatie over het maken van een algemeen goedkeuringsproces raadpleegt u [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Geef toegang of hoger tot Projecten, Taken, Kwesties, of Malplaatjes uit</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project, de taak, de uitgave of het sjabloon beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij het koppelen van goedkeuringsprocessen aan werkitems

Naast de hieronder beschreven overwegingen, adviseren wij dat u de algemene overwegingen over goedkeuringsprocessen in Workfront herziet. Zie voor meer informatie [Overzicht van goedkeuringsproces](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* U moet het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak tot stand brengen alvorens het goedkeuringsproces met hen kan worden geassocieerd.
* Wanneer u een goedkeuringsproces aan een punt voor een status vastmaakt die is overgegaan en waarin het punt momenteel is, zal het goedkeuringsproces niet teweeggebracht worden en geen berichten worden verzonden naar de fiatteurs.

  **Voorbeeld:** Als een taak de status Voltooid heeft en u een goedkeuringsproces koppelt aan de status Voltooid, wordt de goedkeuring niet geactiveerd.

* Wanneer u een goedkeuringsproces aan de eerste status van een punt vastmaakt (door een malplaatje voor taken en projecten te gebruiken, gebruikend de montages van de Opstelling van de Rij voor kwesties, of het bepalen van de Montages van de Taak van een project voor nieuwe taken), worden de goedkeuringsprocessen overgeslagen als de voorgelegde goedkeuring wordt teruggeroepen. In dit geval ontvangen de fiatteurs geen meldingen.

  Voor meer informatie over het terugroepen van goedkeuringen, zie [Goedkeuringen weergeven](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >De eerste status voor een taak of kwestie is Nieuw. De eerste status van een project is de status die door de Workfront-beheerder is geselecteerd in de projectvoorkeuren in uw systeem. Zie voor meer informatie [Projectvoorkeuren voor het hele systeem configureren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* De koppeling van goedkeuringsprocessen aan een object wordt niet opgenomen in het gedeelte Updates voor het object.
* U kunt geen goedkeuringsproces met een oudertaak associëren.
* Als u een gebruiker, team of rol als fiatteur toevoegt, geeft u deze niet automatisch machtigingen voor het object dat aan die goedkeuring is gekoppeld. Ze ontvangen machtigingen voor het object wanneer de goedkeuringsstap wordt geactiveerd. Anders moeten de objecten met hen worden gedeeld voordat ze een goedkeuringsbesluit kunnen nemen.

De volgende secties beschrijven de verschillende methodes om een goedkeuringsproces aan een project, een taak, of een kwestie te associëren.

## Een algemeen goedkeuringsproces koppelen aan een tijdelijk onderdeel {#associate-a-global-approval-process-with-a-work-item}

U kunt een globaal goedkeuringsproces met een het werkpunt (project, taak, kwestie, malplaatje, malplaatjetaak) associëren.

Het algemene goedkeuringsproces moet beschikbaar zijn voor de groep die bij het werkitem hoort of voor alle groepen in het systeem.

>[!NOTE]
>
U kunt processen van de projectgoedkeuring aan een malplaatje, en de processen van de taakgoedkeuring aan een malplaatjetaak vastmaken. Nadat u dit doet, wanneer iemand het malplaatje gebruikt om een project tot stand te brengen, wordt het goedkeuringsproces een project of taakgoedkeuringsproces respectievelijk. Een goedkeuringsproces voor eenmalig gebruik dat aan een sjabloon of sjabloontaak is gekoppeld, blijft een goedkeuringsproces voor projecten en taken voor eenmalig gebruik.

Voor informatie over hoe de beheerders van Workfront een globaal goedkeuringsproces voor alle groepen in het systeem kunnen vormen, en hoe de groepsbeheerders goedkeuringen voor een groep kunnen tot stand brengen, zie [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
U kunt een globaal goedkeuringsproces ook wijzigen om aan uw specifieke behoeften te voldoen. Zie de sectie voor meer informatie [Een algemeen goedkeuringsproces wijzigen voor gebruik op een specifiek object](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel.

Om een bestaand globaal goedkeuringsproces met een project, een taak, een kwestie, een malplaatje, of een malplaatjetaak te associëren:

1. Ga naar het het werkpunt waar u een goedkeuringsproces wilt associëren.
1. Klikken **Goedkeuringen** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** en klik vervolgens op **Goedkeuringen**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Het geselecteerde goedkeuringsproces wordt weergegeven.

1. Breid uit **Bestaande gebruiken** en selecteert u een bestaand goedkeuringsproces.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Het geselecteerde goedkeuringsproces wordt weergegeven.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Klikken **Opslaan**.
1. (Optioneel) Klik op Goedkeuringsprocedure bewerken als u de bestaande goedkeuring die u aan het onderdeel hebt gekoppeld, wilt wijzigen. Hierdoor verandert het wereldwijde goedkeuringsproces in een goedkeuringsproces voor eenmalig gebruik. Zie de sectie voor meer informatie [Een algemeen goedkeuringsproces wijzigen voor gebruik op een specifiek object](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel.

## Een algemeen goedkeuringsproces wijzigen voor gebruik op een specifiek object {#modify-a-global-approval-process-for-use-on-a-specific-object}

Uw Workfront-beheerder of groepsbeheerder maakt algemene goedkeuringsprocessen die u kunt gebruiken, zoals beschreven in [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Het wijzigen van een algemeen goedkeuringsproces dat aan een punt wordt verbonden is identiek aan het wijzigen van een goedkeuringsproces voor eenmalig gebruik.

U kunt een globaal goedkeuringsproces wijzigen om het even welke specifieke behoeften van het project, de taak, of de kwestie aan te passen die u met het associeert.

>[!IMPORTANT]
>
Wanneer u een globaal goedkeuringsproces wijzigt, wordt het een goedkeuringsproces voor eenmalig gebruik dat slechts op het voorwerp kan worden gebruikt waar u het wijzigde. Het algemene goedkeuringsproces blijft ongewijzigd.
>
Houd rekening met de volgende beperkingen bij het wijzigen van een algemeen goedkeuringsproces:
>
* Het goedkeuringsproces wordt gewijzigd slechts voor het project, de taak, of de kwestie u het goedkeuringsproces met associeert.
* Eventuele toekomstige wijzigingen die een beheerder aanbrengt in het oorspronkelijke algemene goedkeuringsproces, weerspiegelen niet het algemene goedkeuringsproces dat u hebt gewijzigd.
>

Als u een goedkeuringsproces wilt wijzigen dat al aan een onderdeel is gekoppeld:

1. Voeg een globaal goedkeuringsproces aan het project, de taak, of de kwestie toe.

   Zie de sectie voor instructies [Een algemeen goedkeuringsproces koppelen aan een tijdelijk onderdeel](#associate-a-global-approval-process-with-a-work-item) in dit artikel.

   >[!IMPORTANT]
   >
   Zorg ervoor dat u klikt **Opslaan** bij het toevoegen van de goedkeuring.

1. Klik op de knop **Bewerken** pictogram ![](assets/edit-icon.png) in de rechterbovenhoek van de goedkeuringspagina. Met deze actie verandert u het goedkeuringsproces op mondiaal of groepsniveau in een goedkeuringsproces voor eenmalig gebruik.
1. Breng eventuele wijzigingen aan in het bestaande goedkeuringsproces. Zie de sectie voor meer informatie [Koppel een goedkeuringsproces voor één gebruik aan een project, taak, uitgave, sjabloon of sjabloontaak](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in dit artikel.
1. Klikken **Opslaan** en klik vervolgens op **Opslaan** nogmaals ter bevestiging dat u het algemene goedkeuringsproces wilt omzetten in een goedkeuringsproces voor eenmalig gebruik dat alleen op dit object beschikbaar is.

## Koppel een goedkeuringsproces voor één gebruik aan een project, taak, uitgave, sjabloon of sjabloontaak {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

U kunt een goedkeuringsproces voor eenmalig gebruik voor gebruik slechts op een specifiek project, een taak, of een kwestie tot stand brengen.

U kunt ook een goedkeuringsproces voor eenmalig gebruik koppelen aan een sjabloon of sjabloontaak, zodat het beschikbaar is voor projecten en taken die met de sjabloon zijn gemaakt.

>[!NOTE]
>
U kunt een goedkeuringsproces voor één gebruik met om het even welk systeem-niveau of groep-niveau status voor een project, een taak, kwestie, een malplaatje, of malplaatjetaak associëren. Voor informatie over Workfront-statussen raadpleegt u [Een status maken of bewerken](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Als u op deze manier een goedkeuringsproces maakt, kunt u een aangepast goedkeuringsproces maken dat aan uw behoeften voldoet. Het goedkeuringsproces kan in de toekomst echter niet aan andere werkitems worden gekoppeld.

U kunt ook een globaal goedkeuringsproces voor een specifiek item wijzigen en dat wordt ook een goedkeuringsproces voor eenmalig gebruik. Zie de sectie [Een algemeen goedkeuringsproces wijzigen voor gebruik op een specifiek object](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel.

Een goedkeuringsproces voor eenmalig gebruik maken:

1. Ga naar het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak waar u een goedkeuringsproces wilt associëren.
1. Klikken **Goedkeuringen** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** > **Goedkeuringen**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klikken **Eenmalig gebruiken maken**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Voer de stappen uit die beginnen met stap 6 in de sectie &quot;Een algemeen goedkeuringsproces op systeemniveau of groepsniveau voor werkitems maken&quot; in het artikel [Een goedkeuringsproces voor werkitems maken](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   Nadat u het goedkeuringsproces voor eenmalig gebruik hebt bevestigd, wordt het weergegeven als &quot;`<Custom>`&quot; in het veld Goedkeuringsproces in het vak Bewerken van sjablonen en sjabloontaken. Zie de volgende artikelen voor informatie over het bewerken van sjablonen of sjabloontaken:
   >
   * [Projectsjablonen bewerken](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [Een sjabloontaak bewerken](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Een goedkeuringsproces uit een tijdelijk onderdeel verwijderen

U kunt een globaal of groep-vlakke goedkeuringsproces verwijderen of u kunt een enig-gebruiksgoedkeuringsproces van een project, een taak, of een kwestie schrappen eerder verbonden aan het.

De volgende scenario&#39;s bestaan: 

* Het verwijderen van het algemene goedkeuringsproces of het goedkeuringsproces op groepsniveau betekent niet dat de goedkeuring wordt verwijderd. De goedkeuring blijft beschikbaar voor toekomstig gebruik.
* Als u een goedkeuringsproces voor één gebruiker verwijdert, wordt dit verwijderd uit Workfront en kan het proces niet worden hersteld.

Om een goedkeuringsproces uit een het werkpunt te verwijderen of te schrappen:

1. Ga naar het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak waar u een goedkeuringsproces wilt verwijderen dat u eerder toevoegde.
1. Klikken **Goedkeuringen** in het linkerdeelvenster.

   Mogelijk moet u op **Meer weergeven** > **Goedkeuringen**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klik op een van de volgende pictogrammen in de rechterbovenhoek van de sectie Goedkeuringen, afhankelijk van het type goedkeuring dat aan het item is gekoppeld:

   * **Verwijderen** pictogram ![](assets/remove-icon---x-in-circle.png) voor algemene of collectieve goedkeuringen.
   * **Verwijderen** pictogram ![](assets/delete.png) voor eenmalig gebruik.

1. Klikken **Verwijderen** of **Verwijderen** ter bevestiging.

   Het goedkeuringsproces wordt verwijderd uit het het werkpunt.

## Een goedkeuringsproces automatisch koppelen aan werkitems

Met de volgende workflows kunt u een goedkeuringsproces automatisch koppelen aan werkitems:

* Voor projecten en taken, kunt u een goedkeuringsproces associëren gebruikend een malplaatje. U kunt een bestaand goedkeuringsproces aan het lusje van de Goedkeuringen van het Malplaatje of het lusje van de Goedkeuringen van de Taak van het Malplaatje vastmaken. Zie voor informatie over het koppelen van een bestaande goedkeuring aan een tijdelijk onderdeel [Een algemeen goedkeuringsproces koppelen aan een tijdelijk onderdeel](#associate-a-global-approval-process-with-a-work-item) in dit artikel.
* Voor nieuwe taken op een bestaand project, kunt u een globaal goedkeuringsproces of een groep-vlakke globaal goedkeuringsproces op het gebied van de Montages van de Taak van het Edit vakje van het Project associëren. Zie de sectie Taakinstellingen in het artikel voor meer informatie [Projecten bewerken](../../manage-work/projects/manage-projects/edit-projects.md).
* Voor kwesties, kunt u een goedkeuring met elke nieuwe kwestie associëren die aan een project wordt toegevoegd door een bestaand goedkeuringsproces met een verzoekrij te associëren. Voor informatie over het vormen van verzoekrijen, zie [Een aanvraagwachtrij maken](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
