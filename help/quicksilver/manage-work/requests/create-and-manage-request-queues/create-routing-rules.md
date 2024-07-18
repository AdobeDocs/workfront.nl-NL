---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Verpletterende regels maken
description: Het verpletteren van Regels controleert wat Adobe Workfront met kwesties doet wanneer zij aan een Rij van het Verzoek worden voorgelegd. Zie Een aanvraagwachtrij maken voor meer informatie over het maken van aanvraagwachtrijen.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Verpletterende regels maken

<!-- Audited: 12/2023 -->

Verpletterend regelcontrole wat Adobe Workfront met kwesties doet wanneer zij aan een verzoekrij worden voorgelegd. Voor meer informatie over het creëren van de Rijen van het Verzoek, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

Het verpletteren van regels verzendt kwesties naar specifieke gebruikers of baanrollen het best uitgerust om de voorgelegde kwestie of het verzoek op te lossen. Het verpletteren van regels wordt gewoonlijk geassocieerd met rijonderwerpen, die worden gebruikt om te controleren welke verpletterende regel op de kwestie of het verzoek zal worden toegepast.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<!--drafted - replace the table at P&P:

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
   <td> <p>Current license: Standard </p> 
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
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
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
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
    <p>Nieuw: Standaard</p>
    <p>of</p>
    <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot projecten bewerken</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p> Rechten voor het project beheren</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creeer een Verpletterende Regel

1. Ga naar het project waarin u de verpletterende regels voor uw verzoeken wilt toevoegen.
1. Klik **Verpletterend Regels** in het linkerpaneel. U zou kunnen moeten klikken **Meer** tonen, dan **Verpletterend Regels**.
1. Klik **Nieuw Verpletterend Regel** om de nieuwe regel toe te voegen.
1. Ga de volgende informatie voor de Verpletterende Regel in:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Naam </strong> </td> 
      <td>De naam van de verpletterende regel. U kunt de verpletterende regel zien als u toegang hebt om deze informatie over het project te zien.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beschrijving </strong> </td> 
      <td>Voeg een beschrijving voor de verpletterende regel toe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Standaard Toegewezen* </strong> </td> 
      <td>Voeg een actieve gebruiker of een actieve baanrol toe aan wie de nieuwe kwesties zouden moeten worden toegewezen. Er kan slechts één standaardontvanger worden toegewezen in dit veld. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> StandaardTeam* </strong> </td> 
      <td>Voeg een actief team toe aan wie de nieuwe kwestie zou moeten worden toegewezen. U kunt slechts één standaardteam op dit gebied hebben.

   <p><b>OPMERKING</b></p>

   Nadat de kwestie wordt voorgelegd, kunt u zijn taken uitgeven en andere gebruikers, rollen, of teams toewijzen. Voor informatie, zie <a href="../../../manage-work/issues/manage-issues/assign-issues.md"> kwesties </a> toewijzen.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Route aan Project </strong> </td> 
      <td>Dit is het project waar de kwestie wordt toegevoegd.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*If een gebruiker, baanrol, of een team worden gedeactiveerd nadat zij met een verpletterende regel worden geassocieerd, blijven de verzoeken aan hen worden verpletterd. U moet periodiek een inventaris van alle verpletterende regels nemen en gedeactiveerde taken vervangen met actieve degenen.

   Wanneer u een kwestie aan een project leidt, ontvangen de gebruikers met toestemmingen op de kwestie de toestemmingen die op dat project worden geplaatst. Voor informatie over het plaatsen van toestemmingen op projecten, zie [ een project in Adobe Workfront ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md) delen.

   ![ Nieuwe Verpletterende doos van de Regel ](assets/new-routing-rule-box.png)

1. Klik **sparen**.

   Dit proces bepaalt slechts de Verpletterende Regel. Om ervoor te zorgen dat de kwestie wordt verpletterd wanneer het aan de verzoekrij wordt voorgelegd, moet u de verpletterende regel op de **lusje van de Details van de Rij** StandaardRoute **selecteren.**

   Voor informatie over het toevoegen van een StandaardRoute aan een verzoekrij, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

   Als u veelvoudige verpletterende regels met de verzoekrij wilt associëren, moet u veelvoudige rijonderwerpen tot stand brengen en elk associëren met een afzonderlijke verpletterende regel. Voor meer informatie over het creëren van een rijonderwerp, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.
