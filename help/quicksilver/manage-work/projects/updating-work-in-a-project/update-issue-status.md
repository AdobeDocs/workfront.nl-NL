---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uitgiftestatus bijwerken
description: U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Uitgiftestatus bijwerken

<!--Audited: 01/2024-->

U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuwe licentie: Medewerker of hoger</p>
   of
   <p>Huidige licentie: aanvragen of hoger</p>
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

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt. Zie voor meer informatie [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

* [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)
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
1. Klik op de knop **Status** in de uitgiftheader en selecteer een nieuwe status.
1. Als u een visuele indicatie van het voltooien van de uitgave wilt weergeven, sleept u of dubbelklikt u op de bel onder **Percentage voltooid** in de koptekst van de uitgave

   of

   Klik binnen de bel in de kopbal van de kwestie om een percentage in te gaan.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven:

   * Als u een notitie over de update wilt toevoegen, gaat u naar de **Updates** sectie en klik op **Nieuwe opmerking** Typ vervolgens een notitie.

     ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Als u bepaalde gebruikers op de hoogte wilt stellen van de update, typt u hun namen in het dialoogvenster **Tags toewijzen aan personen of teams** wordt weergegeven wanneer u een opmerking typt. Zie voor meer informatie [Andere tags toepassen op updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Als u de datum van afgifte vastleggen wilt bijwerken, klikt u op **Probleemdetails** en bewerkt u vervolgens de **Vastlegdatum** veld. Zie voor meer informatie [Problemen bewerken](/help/quicksilver/manage-work/issues/manage-issues/edit-issues.md).


   >[!IMPORTANT]
   >
   >  Alleen uitgevers kunnen de datum vastleggen bijwerken.



<!--Old instructions, in old commenting: 

When you are updating an issue status, you can also add an explanation about the new status and change other issue information such as the commit date.

1. Go to an issue that you are assigned to for which you want to update the status.
1. Click the **Status** field in the issue header and select a new status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. To provide a visual indication of issue completion, drag or double-click the bubble under **Percent Complete** in the header of the issue.

   Or

   Click inside the bubble in the header of the issue to enter a percentage.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

-->

## Probleemstatus automatisch bijwerken

Workfront werkt de bestaande status van een uitgave automatisch bij naar een andere status wanneer de in de onderstaande tabel vermelde handelingen plaatsvinden.

>[!NOTE]
>
>De statussen in de volgende tabel zijn standaardsysteemstatussen. Uw Workfront-beheerder of een groepsbeheerder kan de naam van de statussen in uw exemplaar van Workfront wijzigen. Voor informatie over het maken en beheren van statussen in Workfront raadpleegt u [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

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
   <td> <p>Verschillende statussen</p> <p>Voor informatie over het oplossen van voorwerpen en hoe zij de status van kwesties beïnvloeden, zie de sectie "Synchronize de Status van het Oplosbare Voorwerp met dat van het Oplossende Voorwerp"in het artikel <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Overzicht van Oplossende en Oplosbare objecten </a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Klik op Uitgave starten om te accepteren dat u werkt aan een probleem dat aan u is toegewezen</span> </td> 
   <td><span>Nieuw</span> </td> 
   <td> <p>Om het even welke status verbonden aan de knoop van de Uitgave van het Begin in uw montages van het Team van het Huis. </p> <p>Voor informatie over het vervangen van de knop Werk aan het door een knop Uitgave starten, raadpleegt u <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a></span><span>.</span> </p> <p>Tip: klikken <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">de knop Ongedaan maken</span> nadat u op Uitgave starten hebt geklikt, wordt de status teruggezet naar Nieuw. </p> </td> 
  </tr> 
 </tbody> 
</table>
