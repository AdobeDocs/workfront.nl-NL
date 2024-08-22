---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Verwijderde items herstellen
description: Als u een Workfront-beheerder bent, kunt u projecten, taken, problemen, documenten en sjablonen in Adobe Workfront herstellen als deze in de afgelopen 30 dagen zijn verwijderd. Na 30 dagen worden deze items permanent verwijderd en kunnen ze niet meer worden hersteld.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 0%

---

# Verwijderde items herstellen

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Als u een Workfront-beheerder bent, kunt u projecten, taken, problemen, documenten en sjablonen in Adobe Workfront herstellen als deze in de afgelopen 30 dagen zijn verwijderd. Na 30 dagen worden deze items permanent verwijderd en kunnen ze niet meer worden hersteld.

Wanneer u een object herstelt, worden ook alle onderliggende objecten en velden ervan hersteld. Als u bijvoorbeeld een project herstelt, worden alle taken, problemen, documenten, uren, notities, toewijzingen en aangepaste gegevens in het project ook hersteld.

Een groepsbeheerder kan deze objecten ook herstellen voor een groep die hij of zij beheert.

>[!IMPORTANT]
>
>* Als u een rapport, dashboard, gebruiker, groep, team, of herhaling schrapt, kan het niet worden hersteld.
>* Wanneer in een groep een document rechtstreeks door een andere persoon dan de groepsbeheerder wordt geüpload naar het gebied Documenten van een object, kan alleen een Workfront-beheerder het document herstellen.
>
>* Als u een taak of een uitgave verplaatst en u ervoor kiest om de documenten die aan de taak of de uitgave zijn gekoppeld, niet te verplaatsen, worden de documenten verwijderd en gedurende 30 dagen in de prullenbak geplaatst. Een beheerder kan ze herstellen en ze worden weer aan de verplaatste taak of uitgave toegevoegd. Als de taak of de kwestie sinds het werd bewogen zijn geschrapt, worden de documenten hersteld in het gebied van Documenten van de gebruikerspagina van de beheerder die hen herstelt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

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
   <td><p>Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p></td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan of vergunningstype u hebt, contacteer uw beheerder van Workfront.

+++

## Informatie die wordt hersteld wanneer u een project, een taak, of een kwestie herstelt

Wanneer u een project, een taak, of een kwestie herstelt, wordt de volgende bijbehorende informatie teruggekregen samen met het:

* Opmerkingen en antwoorden op het gebied Updates
* Goedkeuringen
* Toewijzingen
* Aangepaste Forms
* Wachtrij instellen
* Bedrijfs gevallen, met inbegrip van scorecards, doelstellingen en risico&#39;s
* Projectteams
* Datums
* Problemen
* Taken
* Subtaken
* Statussen
* Financiële informatie:

   * Factureringsgegevens
   * Factureringsgraad
   * Uitgaven

* Tijdlijngegevens:

   * Predecessors
   * Taakbeperkingen
   * Het type Duur

* Basislijnen

  De basislijnen van de taak worden teruggekregen wanneer u hun ouderproject of taak, maar niet wanneer u individueel geschrapte taken herstelt.

* Uren (en uur-id&#39;s)

  Of het verwijderde item urenlang wordt hersteld, is afhankelijk van de instellingen die u hebt gekozen bij het configureren van voorkeuren voor tijdbladen en uren. Voor meer informatie, zie [ beïnvloeden beïnvloedt op uren wanneer een voorwerp wordt geschrapt en ](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md) hersteld.

* De URL van het item

  Wanneer de URL van het item wordt hersteld, blijft deze gelijk. Als mensen browserbladwijzers voor het item hebben gemaakt, blijven deze geldig.

* Toegang en machtigingen

  Gebruikers die toegang tot het item hadden voordat het werd verwijderd, krijgen opnieuw toegang nadat het is hersteld.

* Documenten (met inbegrip van proefdocumenten)

  Houd rekening met het volgende wanneer u documenten en documentversies herstelt:

   * Documenten die afzonderlijk zijn verwijderd, kunnen afzonderlijk worden hersteld.

     Documenten die samen met het bovenliggende project, de bovenliggende taak of het bovenliggende probleem zijn verwijderd, worden hersteld wanneer u de bovenliggende toepassing herstelt, maar u kunt deze niet afzonderlijk herstellen.

   * Alle versies van een document of documentproefdruk worden hersteld wanneer het document wordt hersteld.\
     Individuele versies van een document of documentbewijs die afzonderlijk zijn verwijderd, kunnen niet worden hersteld.

## Informatie die niet wordt hersteld wanneer u een project, een taak, of een kwestie herstelt

Wanneer u een project, een taak, of een kwestie herstelt, wordt de volgende bijbehorende informatie niet teruggekregen samen met het:

* Likes
* Aantekeningen
* E-mailadres in een aanvraagwachtrij opnemen
* Favorieten

  Een project, een taak, of een kwestie die u aan het menu van Favorieten alvorens het te schrappen toevoegde verschijnen niet op het menu van Favorieten nadat u het herstelt.

* Objecten omzetten

  Een het oplossen van voorwerp is een omgezet kwestie die met de optie **wordt gevormd houdt de originele kwestie en bindt zijn resolutie aan dit** &lt; **project** of **taak)**>. Als u het ouderproject of de taak schrapt, wordt de kwestie niet meer geïdentificeerd als het oplossen van voorwerp omdat er geen verbinding meer is die het met het project of de taak verbindt. Als u het bovenliggende element herstelt, wordt de koppeling niet hersteld.

  Voor meer informatie over hoe een beheerder van Workfront of groepsbeheerder kwesties vormt om het oplossen van voorwerp aan te passen wanneer omgezet, zie [ taak voor het hele systeem vormen en de voorkeur van de kwestie ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) en [ taak vormen en geven voorkeur voor een groep ](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md) uit.

  Voor meer informatie over het omzetten van kwesties, zie [ Overzicht van het omzetten van kwesties in Adobe Workfront ](../../../manage-work/issues/convert-issues/convert-issues.md).

## Items herstellen

{{step-1-to-setup}}

1. Klik **KringloopBak** > **onlangs Geschrapt**.
1. Klik de **Projecten**, **Taken**, **Kwesties**, **Malplaatjes**, of **Documenten** tabel, afhankelijk van het type van punt u wilt herstellen.

   De punten worden gesorteerd door de **kolom van de Datum van de Schrapping** door gebrek.

1. Selecteer maximaal 10 items die u wilt herstellen.

   Als u een onderliggende taak verwijdert, wordt deze weergegeven in de lijst.

   Als u een bovenliggende taak verwijdert, wordt alleen de bovenliggende taak in de lijst weergegeven. Maar alle onderliggende taken worden hersteld wanneer u een bovenliggende taak herstelt.

1. Klik **herstellen** om de geselecteerde punten aan hun originele plaats te herstellen.
1. (Facultatief) om het herstelde punt snel te bekijken, volg de stappen in [ Mening herstelde punt ](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Voor meer informatie over wat gebeurt nadat u een punt terugzet, zie de sectie [ wat gebeurt nadat u punten ](#what-happens-after-you-restore-items) in dit artikel terugzet.

## Wat gebeurt er nadat u items hebt teruggezet {#what-happens-after-you-restore-items}

* Wanneer u taken en subtaken herstelt, worden deze weergegeven in de volgorde waarin ze zich bevonden voordat ze werden verwijderd.

  Als de volgorde van andere taken echter verandert terwijl de taak wordt verwijderd, wordt de taak mogelijk onder aan de lijst met taken of subtaken hersteld.

* Nadat u een item hebt hersteld:

   * Er wordt een bericht weergegeven om u te laten weten of u succes hebt geboekt.

     U ontvangt ook een e-mailbericht. Als u meerdere items hebt hersteld, worden deze in de e-mail vermeld.

   * Een opmerking wordt weergegeven in het gedeelte Updates van het project, de taak of de uitgave en in dat van het bovenliggende object.

     Dit gebeurt niet wanneer u een document of een sjabloon herstelt.

## Herstelde proefdrukken

Wanneer iemand een document herstelt dat een bewijs heeft, zou de pagina van de Activiteiten van het Bewijs voor de proef de naam van de eerste actieve beheerder van Workfront kunnen tonen die voor de instantie van uw organisatie (in orde van profiel ID) wordt vermeld in plaats van daadwerkelijke persoon die de proef herstelde.
