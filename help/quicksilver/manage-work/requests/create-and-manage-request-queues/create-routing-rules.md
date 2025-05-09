---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Verpletterende regels maken
description: Het verpletteren van Regels controleert wat Adobe Workfront met kwesties doet wanneer zij aan een Rij van het Verzoek worden voorgelegd.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Verpletterende regels maken

<!-- Audited: 12/2023 -->

Verpletterend regelcontrole wat Adobe Workfront met kwesties doet wanneer zij aan een verzoekrij worden voorgelegd. Voor meer informatie over het creëren van de Rijen van het Verzoek, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

Het verpletteren van regels verzendt kwesties naar specifieke gebruikers of baanrollen het best uitgerust om de voorgelegde kwestie of het verzoek op te lossen. Het verpletteren van regels wordt gewoonlijk geassocieerd met rijonderwerpen, die worden gebruikt om te controleren welke verpletterende regel op de kwestie of het verzoek zal worden toegepast.

Zodra gecreeerd, kunt u niet het verpletteren van regels van één project aan een ander bewegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-plan</p></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Nieuwe licentie: standaard </p> 
   of
   <p>Huidige licentie: abonnement </p> </td> 
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

*For meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creeer een Verpletterende Regel

1. Ga naar het project waarin u het verpletteren van regels voor uw verzoeken wilt toevoegen.
1. Klik **Verpletterend Regels** in het linkerpaneel.
1. Klik **Nieuw Verpletterend Regel** om de nieuwe regel toe te voegen. Het **Nieuwe Verpletterende doos van de Regel** opent.

   ![ Nieuwe Verpletterende doos van de Regel ](assets/new-routing-rule-box.png)
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

1. Klik **sparen**.

   Dit proces bepaalt slechts de Verpletterende Regel. Om ervoor te zorgen dat de kwestie wordt verpletterd wanneer het aan de verzoekrij wordt voorgelegd, moet u de verpletterende regel op de **lusje van de Details van de Rij** StandaardRoute **selecteren.**

   Voor informatie over het toevoegen van een StandaardRoute aan een verzoekrij, zie [ een Rij van het Verzoek ](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md) creëren.

   Als u veelvoudige verpletterende regels met de verzoekrij wilt associëren, moet u veelvoudige rijonderwerpen tot stand brengen en elk associëren met een afzonderlijke verpletterende regel. Voor meer informatie over het creëren van een rijonderwerp, zie [ de Onderwerpen van de Rij ](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) creëren.
