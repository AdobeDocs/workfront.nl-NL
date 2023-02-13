---
product-area: projects
navigation-topic: update-work-in-a-project
title: Uitgiftestatus bijwerken
description: U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.
author: Alina
feature: Work Management
exl-id: 6e09dfcf-dceb-4f33-9592-0769283369c7
source-git-commit: 6bb6b834c5af8ad48179fc0d60b184d083b360e4
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Uitgiftestatus bijwerken

U kunt de status van een uitgave bijwerken om anderen te informeren over waar het probleem zich voordoet en hoe het verder gaat.

## Toegangsvereisten

<!--drafted for P&P;

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

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
   <td> <p>Aanvraag of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot problemen bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor het probleem beheren</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

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

Wanneer u een uitgiftestatus bijwerkt, kunt u ook een uitleg over de nieuwe status toevoegen en andere uitgiftegegevens wijzigen, zoals de datum waarop u bent vastgelegd.

1. Ga naar een kwestie waaraan u wordt toegewezen waaraan u de status wilt bijwerken.
1. Klik op de knop **Status** in de uitgiftheader en selecteer een nieuwe status.

   ![](assets/nwe-issue-status-expanded-in-header-350x370.png)

1. Als u een visuele indicatie van het voltooien van de uitgave wilt weergeven, sleept u of dubbelklikt u op de bel onder **Percentage voltooid** in de koptekst van de uitgave.

   of

   Klik binnen de bel in de kopbal van de kwestie om een percentage in te gaan.

   ![](assets/nwe-updatetaskpercentinheader-350x54.png)

1. (Optioneel) Voer een van de volgende handelingen uit om aanvullende informatie over de update op te geven en klik vervolgens op **Bijwerken** of als de uitgave een status heeft die gelijk is aan Voltooien, klikt u op **Gereed:**

   * Als u een notitie over de update wilt toevoegen, gaat u naar de **Updates** en klik op **Een nieuwe update starten** Typ uw notitie.

      ![](assets/nwe-issue-update-stream-message-box-350x125.png)

   * Als u bepaalde gebruikers op de hoogte wilt stellen van de update, typt u hun namen in het dialoogvenster **Waarschuwen** wordt weergegeven wanneer u een notitie over de update typt. Zie voor meer informatie [Andere tags toepassen op updates](../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
   * Klik op **Voorwaarde** Selecteer vervolgens de voorwaarde die de huidige voorwaarde van de uitgave het beste weerspiegelt. Selecteer een van de volgende opties:

      * Vloeiend gaan
      * Sommige problemen
      * Belangrijkste wegversperringen
   * Als u de datum van afgifte vastleggen wilt bijwerken, vouwt u het dialoogvenster **Vastlegdatum** en selecteer een nieuwe datum.


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
   <td>Handeling</td> 
   <td>Oorspronkelijke status</td> 
   <td>Nieuwe status</td> 
  </tr> 
  <tr> 
   <td>Het percentage van de uitgave dat is voltooid bijwerken naar 100%</td> 
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
   <td> <p>Om het even welke status verbonden aan de knoop van de Uitgave van het Begin in uw montages van het Team van het Huis. </p> <p>Voor informatie over het vervangen van de knop Werk aan het door een knop Uitgave starten, raadpleegt u <span href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md"><a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">De knop Aan de werkbalk vervangen door de knop Start</a></span><span>.</span> </p> <p>Tip: Klikken <span data-mc-conditions="QuicksilverOrClassic.Quicksilver">de knop Ongedaan maken</span> nadat u op Uitgave starten hebt geklikt, wordt de status teruggezet naar Nieuw. </p> </td> 
  </tr> 
 </tbody> 
</table>
