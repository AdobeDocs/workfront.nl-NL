---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uitgiftestatus bijwerken
description: U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 0%

---

# Uitgiftestatus bijwerken

<!--Audited: 01/2024-->

U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot problemen bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

*Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Contributor or higher</p>
   Or
   <p>Current: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Uitgiftestatus

Hier volgen de standaardstatussen voor uitgaven in Workfront:

* Nieuw
* In uitvoering
* Nog geen feedback
* In de wachtstand
* Geen oplossing
* Opnieuw geopend
* Gesloten
* Opgelost

Uw Adobe Workfront-beheerder kan aangepaste statussen toevoegen voor problemen voor uw organisatie. Ze kunnen statussen ook beschikbaar maken, afhankelijk van het type uitgave.

Raadpleeg de volgende artikelen voor meer informatie over aangepaste statussen en uitgavetypen:

* [&#x200B; creeer of geef een status &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uit
* [Problemen maken](../../../manage-work/issues/manage-issues/create-issues.md)

U kunt de status van uitgaven handmatig bijwerken of u kunt Workfront toestaan deze automatisch bij te werken wanneer bepaalde handelingen plaatsvinden.

## Probleemstatus handmatig bijwerken

U kunt de status van de uitgave bijwerken in de volgende gebieden van Workfront:

* De uitgiftekoptekst op de taakpagina.
* Het uitgiftevak Bewerken wanneer u een uitgave bewerkt.
* De sectie Details op de uitgavepagina.
* In een uitgiftenlijst of rapport, wanneer het gebied van de Status in de mening zichtbaar is.
* In het paneel Samenvatting van de kwestie.

U kunt als volgt de status van de uitgave in de uitgaveheader handmatig bijwerken:

1. Ga naar een kwestie waarvoor u de status wilt bijwerken.
1. Klik het **gebied van de Status** in de uitgiftekopbal en selecteer een nieuwe status.
1. Om een visuele aanwijzing van kwestie voltooiing te verstrekken, sleep of dubbelklik de bel onder **Volledige Percentage** in de kopbal van de kwestie tweemaal

   of

   Klik binnen de bel in de kopbal van de kwestie om een percentage in te gaan.

   ![&#x200B; voltooide het taakpercentage van de Update in kopbal &#x200B;](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven:

   * Om een nota over de update toe te voegen, ga naar de **sectie van Updates** en klik **Nieuwe commentaar**, dan typ een nota.

     ![&#x200B; het berichtvakje van de updatestroom van de Uitgave &#x200B;](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Om bepaalde gebruikers over de update op de hoogte te brengen, typ hun namen op het **mensen van de Markering of team** gebied dat verschijnt wanneer u een commentaar typt. Voor meer informatie, zie [&#x200B; Tags anderen op updates &#x200B;](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Om de Vastlegdatum van de kwestie bij te werken, klik **Details van de Uitgave**, dan geef **het gebied van de Datum** toe. Voor informatie, zie [&#x200B; kwesties &#x200B;](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md) uitgeven.


   >[!IMPORTANT]
   >
   >  Alleen uitgevers kunnen de datum vastleggen bijwerken.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![Issue status expanded in header](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![Update task percent in header](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Probleemstatus automatisch bijwerken

Workfront werkt de bestaande status van een uitgave automatisch bij naar een andere status wanneer de in de onderstaande tabel vermelde handelingen plaatsvinden.

>[!NOTE]
>
>De statussen in de volgende tabel zijn standaardsysteemstatussen. Uw Workfront-beheerder of een groepsbeheerder kan de naam van de statussen in uw exemplaar van Workfront wijzigen. Voor informatie over het creëren van en het leiden van statussen in Workfront, zie [&#x200B; een status &#x200B;](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) creëren of uitgeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Handeling</b></td> 
   <td><b>Oorspronkelijke status</b></td> 
   <td><b>Nieuwe status</b></td> 
  </tr> 
  <tr> 
   <td>Het uitgiftepercentage bijwerken tot 100%</td> 
   <td>Nieuw of Bezig</td> 
   <td>Gesloten</td> 
  </tr> 
  <tr> 
   <td>Het percentage van de uitgave dat is voltooid, bijwerken van 100% naar een lager getal</td> 
   <td>Gesloten </td> 
   <td>In uitvoering</td> 
  </tr> 
  <tr> 
   <td>De status bijwerken van een oplossend object dat is gekoppeld aan het probleem</td> 
   <td>Verschillende statussen</td> 
   <td> <p>Verschillende statussen</p> <p>Voor informatie over het oplossen van voorwerpen en hoe zij de status van kwesties beïnvloeden, zie de sectie "Synchronize de Status van het Oplosbare Voorwerp met dat van het Oplossende Voorwerp"in het artikel <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref"> Overzicht van het Oplossen van en Oplosbare Voorwerpen </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span> klik de knoop van de Uitgave van het Begin om het werken aan een kwestie goed te keuren die aan u wordt toegewezen </span> </td> 
   <td><span> Nieuw </span> </td> 
   <td> <p>Om het even welke status verbonden aan de knoop van de Uitgave van het Begin in uw montages van het Team van het Huis. </p> <p>Voor informatie over het vervangen van het Werk op het knoop met een knoop van de Uitgave van het Begin, zie <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref"> het Werk op het knoop met een knoop van het Begin vervangen </a></span> <span>.</span> </p> <p>Tip: Het klikken <span data-mc-conditions="QuicksilverOrClassic.Quicksilver"> ongedaan maakt knoop </span> na het klikken van de Uitgave van het Begin keert de status aan Nieuw terug. </p> </td> 
  </tr> 
 </tbody> 
</table>
