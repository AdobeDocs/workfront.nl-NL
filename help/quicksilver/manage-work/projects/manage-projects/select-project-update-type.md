---
product-area: projects
navigation-topic: manage-projects
title: Selecteer het Type van projectupdate
description: Door een Type van Update voor een project te selecteren, kunt u controleren hoe vaak de veranderingen u aan de chronologie van het project aanbrengt op de oudertaken of het project worden bewaard.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Selecteer het Type van projectupdate

Door een Type van Update voor een project te selecteren, kunt u controleren hoe vaak de veranderingen u aan de chronologie van het project aanbrengt op de oudertaken of het project worden bewaard.

Wanneer de projectchronologie wordt bijgewerkt, wordt het opnieuw berekend gebaseerd op veranderingen die aan het project, zijn taken, of veranderingen worden aangebracht aan een ander project dat de chronologie van afhankelijk is.

De volgende wijzigingen in de taken van het project activeren bijvoorbeeld een update van de tijdlijn  van het project:

* Datums van taken bijwerken
* De voorgangersrelaties van taken wijzigen
* Verander ouder-kind verhoudingen, toevoegend of verwijderend taken naast het veranderen van de taakbeperking of het type van duur.

## Toegangsvereisten

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Het updatetype van een project bijwerken

Wanneer de taken bijwerken, werken hun oudervoorwerpen (oudertaken of het project) op de tijd bij die door het Type van Update wordt vermeld.  Om een Type van Update voor uw project te specificeren:

1. Ga naar het project waarvan Type van Update u wilt specificeren.
1. Klik het Meer menu ![ Meer pictogram ](assets/more-icon.png) naast de naam van het project, dan klik **uitgeven**.

1. Klik **&#x200B;**&#x200B;Montages van het Project **&#x200B;**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Op het **gebied van het Type van Update**, selecteer of u Workfront de chronologie van het project wilt automatisch dagelijks berekenen, wanneer er een verandering is, of als u de projectmanager het manueel wilt berekenen.

   Selecteer een van de opties in de onderstaande lijst. 

   >[!IMPORTANT]
   >
   >Als de tijdlijn van een project langer is dan 15 jaar, berekent Workfront de tijdlijn niet automatisch of bij wijziging. Het updatetype van een project langer dan 15 jaar is altijd Handmatig.

   * **Automatisch en op Verandering:** dit is het gebrek dat plaatst. De projectchronologie wordt bijgewerkt telkens als een verandering in het project of in een ander project voorkomt dat de chronologie van afhankelijk is. De projecttijdlijn wordt ook elke avond bijgewerkt. \
     Dit is de aanbevolen instelling omdat de tijdlijn van het project altijd up-to-date is.

     Wanneer u een taak of het project bijwerkt en een tijdlijnherberekening activeert, worden alle beschikbare datums onmiddellijk weergegeven, zodat u kunt doorgaan met werken. Voor projecten met meer dan 100 taken worden datums die langere berekeningen vereisen, grijs weergegeven.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     Dit geeft aan dat de herberekening nog niet is voltooid en dat de datums kunnen worden gewijzigd.

   * **Verandering slechts:** de projectchronologie wordt bijgewerkt telkens als een verandering in het project of in een ander project voorkomt dat de chronologie afhankelijk is; de geplande updates komen niet voor.\
     U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als de veranderingen zelden in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

   * **Automatisch slechts:** de projectchronologie wordt bijgewerkt elke nacht; het wordt niet onmiddellijk bijgewerkt nadat de veranderingen worden aangebracht.\
     U zou deze optie kunnen willen selecteren als u zich over systeemprestaties ongerust maakt en als vele veranderingen elke dag in het project of in andere projecten voorkomen dat de chronologie van afhankelijk is.

     >[!NOTE]
     >
     >Een project herberekent niet automatisch elke nacht als het in de status van de Planning is. Het herberekent alleen op verandering.

   * **Hand slechts:** de projectchronologie wordt bijgewerkt slechts wanneer u de optie om **Chronologie** opnieuw te berekenen, zoals die in de sectie &quot;Handmatige herberekening&quot;in de artikel [ wordt beschreven projectchronologie ](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) opnieuw berekent.\
     U kunt deze optie selecteren als u in één keer veel wijzigingen aanbrengt in het project en u wilt dat de tijdlijnherberekening plaatsvindt nadat alle wijzigingen zijn aangebracht (in plaats van na elke afzonderlijke wijziging).

1. Klik **sparen**.
