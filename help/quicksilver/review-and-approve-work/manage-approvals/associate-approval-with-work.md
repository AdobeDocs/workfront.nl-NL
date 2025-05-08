---
product-area: projects
navigation-topic: approvals
title: Een nieuw of bestaand goedkeuringsproces koppelen aan werk
description: In dit artikel wordt beschreven hoe u goedkeuringsprocessen aan werkitems kunt koppelen. Zie de volgende artikelen voor informatie over het koppelen van goedkeuringen aan proefdrukken of documenten.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 06e42fa713bc9b0c1e308feb2b84ca62dafa416c
workflow-type: tm+mt
source-wordcount: '1891'
ht-degree: 0%

---

# Een nieuw of bestaand goedkeuringsproces koppelen aan werk

In dit artikel wordt beschreven hoe u goedkeuringsprocessen aan werkitems kunt koppelen. Zie de volgende artikelen voor informatie over het koppelen van goedkeuringen aan proefdrukken of documenten:

* [ creeer een geavanceerd bewijs met een Geautomatiseerd werkschema ](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Documentgoedkeuring aanvragen](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

U kunt een globaal goedkeuringsproces of een goedkeuringsproces voor eenmalig gebruik koppelen aan een tijdelijk onderdeel in Adobe Workfront. De volgende scenario&#39;s bestaan:

* Koppel een bestaand globaal goedkeuringsproces aan een project, een taak, een kwestie, een malplaatje, of een malplaatjetaak. Alle groepen in het systeem beschikken over enkele algemene goedkeuringsprocessen. Globale goedkeuringsprocessen op groepsniveau zijn alleen beschikbaar voor bepaalde groepen.
* Creeer een enig-gebruik goedkeuringsproces en associeer het met een bestaand project, een taak, een kwestie, een malplaatje, of een malplaatjetaak.

>[!NOTE]
>
>In dit artikel wordt de term &quot;wereldwijd goedkeuringsproces&quot; gebruikt om een onderscheid te maken tussen &quot;goedkeuringsproces voor eenmalig gebruik&quot;. Een algemeen goedkeuringsproces kan herhaaldelijk worden gebruikt.
>
>De term &quot;mondiaal goedkeuringsproces op groepsniveau&quot; verwijst naar een goedkeuringsproces dat herhaaldelijk kan worden gebruikt voor artikelen en statussen die alleen aan een specifieke groep zijn gekoppeld.

Voor meer algemene informatie over goedkeuringsprocessen, zie [ overzicht van het proces van de Goedkeuring ](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Voor informatie over het creëren van een globaal goedkeuringsproces, zie [ een goedkeuringsproces voor het werkpunten ](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td> <p>Geef toegang of hoger tot Projecten, Taken, Kwesties, of Malplaatjes uit</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het project, de taak, de uitgave of het sjabloon beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

+++

## Overwegingen bij het koppelen van goedkeuringsprocessen aan werkitems

Naast de hieronder beschreven overwegingen, adviseren wij dat u de algemene overwegingen over goedkeuringsprocessen in Workfront herziet. Voor meer informatie, zie [ overzicht van het proces van de Goedkeuring ](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* U moet het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak tot stand brengen alvorens het goedkeuringsproces met hen kan worden geassocieerd.
* Wanneer u een goedkeuringsproces aan een punt voor een status vastmaakt die is overgegaan en waarin het punt momenteel is, zal het goedkeuringsproces niet teweeggebracht worden en geen berichten worden verzonden naar de fiatteurs.

  **Voorbeeld:** als een taak in de status van Voltooid is en u een goedkeuringsproces verbonden aan de Volledige status vastmaakt, teweegbrengt de goedkeuring niet.

* Wanneer u een goedkeuringsproces aan de eerste status van een punt vastmaakt (door een malplaatje voor taken en projecten te gebruiken, gebruikend de montages van de Opstelling van de Rij voor kwesties, of het bepalen van de Montages van de Taak van een project voor nieuwe taken), worden de goedkeuringsprocessen overgeslagen als de voorgelegde goedkeuring wordt teruggeroepen. In dit geval ontvangen de fiatteurs geen meldingen.

  Voor meer informatie over het roepen van goedkeuringen, zie [ goedkeuringen van de Mening ](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >De eerste status voor een taak of kwestie is Nieuw. De eerste status van een project is de status die door de Workfront-beheerder is geselecteerd in de projectvoorkeuren in uw systeem. Voor informatie, zie [ systeem-brede projectvoorkeur ](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

* De koppeling van goedkeuringsprocessen aan een object wordt niet opgenomen in het gedeelte Updates voor het object.
* U kunt geen goedkeuringsproces met een oudertaak associëren.
* Als u een gebruiker, team of rol als fiatteur toevoegt, geeft u deze niet automatisch machtigingen voor het object dat aan die goedkeuring is gekoppeld. Ze ontvangen machtigingen voor het object wanneer de goedkeuringsstap wordt geactiveerd. Anders moeten de objecten met hen worden gedeeld voordat ze een goedkeuringsbesluit kunnen nemen.

De volgende secties beschrijven de verschillende methodes om een goedkeuringsproces aan een project, een taak, of een kwestie te associëren.

## Een algemeen goedkeuringsproces koppelen aan een tijdelijk onderdeel {#associate-a-global-approval-process-with-a-work-item}

U kunt een globaal goedkeuringsproces met een het werkpunt (project, taak, kwestie, malplaatje, malplaatjetaak) associëren.

U kunt tot om het even welk globaal goedkeuringsproces toegang hebben zolang het met een groep wordt gedeeld u tot of alle groepen in het systeem behoort.

<!--The global approval process must be available to the group associated with the work item or to all groups in the system.-->

>[!NOTE]
>
>U kunt processen van de projectgoedkeuring aan een malplaatje, en de processen van de taakgoedkeuring aan een malplaatjetaak vastmaken. Nadat u dit doet, wanneer iemand het malplaatje gebruikt om een project tot stand te brengen, wordt het goedkeuringsproces een project of taakgoedkeuringsproces respectievelijk. Een goedkeuringsproces voor eenmalig gebruik dat aan een sjabloon of sjabloontaak is gekoppeld, blijft een goedkeuringsproces voor projecten en taken voor eenmalig gebruik.

Voor informatie over hoe de beheerders van Workfront een globaal goedkeuringsproces voor alle groepen in het systeem kunnen vormen, en hoe de groepsbeheerders goedkeuringen voor een groep kunnen tot stand brengen, zie [ een goedkeuringsproces voor het werkpunten ](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) creëren.

>[!NOTE]
>
>U kunt een globaal goedkeuringsproces ook wijzigen om aan uw specifieke behoeften te voldoen. Voor meer informatie, zie de sectie [ een globaal goedkeuringsproces voor gebruik op een specifiek voorwerp ](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel wijzigen.

Om een bestaand globaal goedkeuringsproces met een project, een taak, een kwestie, een malplaatje, of een malplaatjetaak te associëren:

1. Ga naar het het werkpunt waar u een goedkeuringsproces wilt associëren.
1. Klik **goedkeurt** in het linkerpaneel.

   ![ goedkeurt sectie op taak ](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![ Gebruik bestaand of creeer enige gebruiksgoedkeuringen ](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Het geselecteerde goedkeuringsproces wordt weergegeven.

1. Breid het **Gebruik bestaande** drop-down menu uit en selecteer een bestaand goedkeuringsproces.

   ![ goedkeurt menu ](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Het geselecteerde goedkeuringsproces wordt weergegeven.

   ![ Bestaande goedkeuring in bijlage aan taak ](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Klik **sparen**.
1. (Optioneel) Klik op Goedkeuringsprocedure bewerken als u de bestaande goedkeuring die u aan het onderdeel hebt gekoppeld, wilt wijzigen. Hierdoor verandert het wereldwijde goedkeuringsproces in een goedkeuringsproces voor eenmalig gebruik. Voor meer informatie, zie de sectie [ een globaal goedkeuringsproces voor gebruik op een specifiek voorwerp ](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel wijzigen.

## Een algemeen goedkeuringsproces wijzigen voor gebruik op een specifiek object {#modify-a-global-approval-process-for-use-on-a-specific-object}

Uw beheerder van Workfront of groepsbeheerder leidt tot globale goedkeuringsprocessen voor u aan gebruik, zoals die in [ wordt beschreven leidt tot een goedkeuringsproces voor het werkpunten ](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Het wijzigen van een algemeen goedkeuringsproces dat aan een punt wordt verbonden is identiek aan het wijzigen van een goedkeuringsproces voor eenmalig gebruik.

U kunt een globaal goedkeuringsproces wijzigen om het even welke specifieke behoeften van het project, de taak, of de kwestie aan te passen die u met het associeert.

>[!IMPORTANT]
>
>Wanneer u een globaal goedkeuringsproces wijzigt, wordt het een goedkeuringsproces voor eenmalig gebruik dat slechts op het voorwerp kan worden gebruikt waar u het wijzigde. Het algemene goedkeuringsproces blijft ongewijzigd.
>
>Houd rekening met de volgende beperkingen bij het wijzigen van een algemeen goedkeuringsproces:
>
>* Het goedkeuringsproces wordt gewijzigd slechts voor het project, de taak, of de kwestie u het goedkeuringsproces met associeert.
>* Eventuele toekomstige wijzigingen die een beheerder aanbrengt in het oorspronkelijke algemene goedkeuringsproces, weerspiegelen niet het algemene goedkeuringsproces dat u hebt gewijzigd.
>

Als u een goedkeuringsproces wilt wijzigen dat al aan een onderdeel is gekoppeld:

1. Voeg een globaal goedkeuringsproces aan het project, de taak, of de kwestie toe.

   Voor instructies, zie de sectie [ een globaal goedkeuringsproces met een het werkpunt ](#associate-a-global-approval-process-with-a-work-item) in dit artikel associëren.

   >[!IMPORTANT]
   >
   >Zorg ervoor dat u **sparen** wanneer het toevoegen van de goedkeuring klikt.

1. Nadat het globale goedkeuringsproces wordt toegevoegd, klik **uitgeven** pictogram ![ pictogram ](assets/edit-icon.png) in de hoger-juiste hoek van de goedkeuringspagina. Met deze actie verandert u het goedkeuringsproces op mondiaal of groepsniveau in een goedkeuringsproces voor eenmalig gebruik.
1. Breng eventuele wijzigingen aan in het bestaande goedkeuringsproces. Voor meer informatie, zie de sectie [ een enig-gebruiks goedkeuringsproces met een project, een taak, een kwestie, een malplaatje, of malplaatjetaak ](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in dit artikel associëren.
1. Klik **sparen**, dan klik **sparen** opnieuw om te bevestigen dat u het globale goedkeuringsproces in een enig-gebruiks goedkeuringsproces wilt omzetten dat slechts op dit voorwerp beschikbaar is.

## Koppel een goedkeuringsproces voor één gebruik aan een project, taak, uitgave, sjabloon of sjabloontaak {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

U kunt een goedkeuringsproces voor eenmalig gebruik voor gebruik slechts op een specifiek project, een taak, of een kwestie tot stand brengen.

U kunt ook een goedkeuringsproces voor eenmalig gebruik koppelen aan een sjabloon of sjabloontaak, zodat het beschikbaar is voor projecten en taken die met de sjabloon zijn gemaakt.

>[!NOTE]
>
>U kunt een goedkeuringsproces voor één gebruik met om het even welk systeem-niveau of groep-niveau status voor een project, een taak, kwestie, een malplaatje, of malplaatjetaak associëren. Voor informatie over de statussen van Workfront, zie [ een status ](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

Als u op deze manier een goedkeuringsproces maakt, kunt u een aangepast goedkeuringsproces maken dat aan uw behoeften voldoet. Het goedkeuringsproces kan in de toekomst echter niet aan andere werkitems worden gekoppeld.

U kunt ook een globaal goedkeuringsproces voor een specifiek item wijzigen en dat wordt ook een goedkeuringsproces voor eenmalig gebruik. Voor informatie, zie de sectie [ een globaal goedkeuringsproces voor gebruik op een specifiek voorwerp ](#modify-a-global-approval-process-for-use-on-a-specific-object) in dit artikel wijzigen.

Een goedkeuringsproces voor eenmalig gebruik maken:

1. Ga naar het project, de taak, de kwestie, het malplaatje, of de malplaatjetaak waar u een goedkeuringsproces wilt associëren.
1. Klik **goedkeurt** in het linkerpaneel.

   ![ goedkeurt sectie op taak ](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klik **creëren enig-gebruik**.

   ![ goedkeurt menu ](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Voltooi de stappen die met stap 6 in de sectie &quot;beginnen een systeem-niveau of groep-vlakke globaal goedkeuringsproces voor het werkpunten&quot;in het artikel [ creëren een goedkeuringsproces voor het werkpunten ](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >Nadat u het enig-gebruiks goedkeuringsproces vastmaakt, toont het als &quot;`<Custom>`&quot;in het gebied van het Proces van de Goedkeuring binnen het Edit vakje van malplaatjes en malplaatjetaken. Zie de volgende artikelen voor informatie over het bewerken van sjablonen of sjabloontaken:
   >
   >* [ geef projectmalplaatjes ](../../manage-work/projects/create-and-manage-templates/edit-templates.md) uit
   >* [ geef een malplaatjetaak ](../../manage-work/projects/create-and-manage-templates/edit-template-task.md) uit

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
1. Klik **goedkeurt** in het linkerpaneel.

   ![ goedkeurt sectie op taak ](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klik op een van de volgende pictogrammen in de rechterbovenhoek van de sectie Goedkeuringen, afhankelijk van het type goedkeuring dat aan het item is gekoppeld:

   * **verwijderen** pictogram ![ verwijdert pictogram ](assets/remove-icon---x-in-circle.png) voor globale of groep-vlakke goedkeuringen.
   * **het pictogram van de Schrapping** pictogram ![ schrap pictogram ](assets/delete.png) voor enig-gebruiksgoedkeuringen.

1. Klik **verwijderen** of **Schrapping** om te bevestigen.

   Het goedkeuringsproces wordt verwijderd uit het het werkpunt.

## Een goedkeuringsproces automatisch koppelen aan werkitems

Met de volgende workflows kunt u een goedkeuringsproces automatisch koppelen aan werkitems:

* Voor projecten en taken, kunt u een goedkeuringsproces associëren gebruikend een malplaatje. U kunt een bestaand goedkeuringsproces aan het lusje van de Goedkeuringen van het Malplaatje of het lusje van de Goedkeuringen van de Taak van het Malplaatje vastmaken. Voor informatie over het associëren van een bestaande goedkeuring met een het werkpunt, zie [ een globaal goedkeuringsproces met een het werkpunt ](#associate-a-global-approval-process-with-a-work-item) in dit artikel associëren.
* Voor nieuwe taken op een bestaand project, kunt u een globaal goedkeuringsproces of een groep-vlakke globaal goedkeuringsproces op het gebied van de Montages van de Taak van het Edit vakje van het Project associëren. Voor informatie, zie de sectie &quot;Montages van de Taak&quot;in artikel [ projecten ](../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.
* Voor kwesties, kunt u een goedkeuring met elke nieuwe kwestie associëren die aan een project wordt toegevoegd door een bestaand goedkeuringsproces met een verzoekrij te associëren. Voor informatie over het vormen van verzoekrijen, zie [ een Rij van het Verzoek ](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.
