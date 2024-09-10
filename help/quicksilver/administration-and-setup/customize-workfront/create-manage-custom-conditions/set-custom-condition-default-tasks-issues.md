---
title: Een aangepaste voorwaarde instellen als de standaardinstelling voor taken en problemen
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wanneer een gebruiker op het Werk klikt of een updatecommentaar toevoegt aan een nieuwe taak zij (zonder manueel een voorwaarde voor de taak te plaatsen) zijn toegewezen, toont Adobe Workfront de standaardvoorwaarde voor taken, die in Opstelling wordt gevormd. Hetzelfde geldt voor kwesties.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Een aangepaste voorwaarde instellen als standaard voor taken en problemen

Wanneer een gebruiker op het Werk klikt of een updatecommentaar toevoegt aan een nieuwe taak zij (zonder manueel een voorwaarde voor de taak te plaatsen) zijn toegewezen, toont Adobe Workfront de standaardvoorwaarde voor taken, die in Opstelling wordt gevormd. Hetzelfde geldt voor kwesties.

Workfront gebruikt de ingebouwde voorwaarde Vloeiend als standaardvoorwaarde voor taken en, afzonderlijk, voor kwesties. Als Workfront-beheerder kunt u de standaardvoorwaarde voor beide objecttypen wijzigen in een aangepaste voorwaarde die u hebt gemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Stel een aangepaste voorwaarde in als een standaardvoorwaarde voor taken of uitgaven:

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** > **Voorwaarden**.

1. Klik de **Taken** of **Kwesties** tabel.

1. Klik **Vastgestelde StandaardVoorwaarden**.
1. Klik in het keuzemenu op de aangepaste voorwaarde die u als de standaardvoorwaarde voor taken (of uitgaven) wilt instellen.
1. Klik **sparen**.

>[!NOTE]
>
>* Een gebruiker die is toegewezen aan een taak of uitgave, of die beheermachtigingen heeft, kan de voorwaarde handmatig wijzigen. Voor meer informatie, zie [ Voorwaarde van de Update voor taken en kwesties ](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* De drie standaardvoorwaarden voor taken en problemen die met Workfront worden geleverd, zijn Vloeiend, Sommige zorgen en Belangrijke wegversperringen. U kunt deze voorwaarden niet verbergen of verwijderen, maar u kunt wel de naam en de kleur van de voorwaarden wijzigen. Of u kunt nieuwe degenen in plaats daarvan tot stand brengen om te gebruiken, zoals die in [ wordt beschreven creeer of geef een douanevoorwaarde ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) uit.
>

Voor informatie over het vormen van een douanevoorwaarde als standaardvoorwaarde voor projecten, zie [ Plaats een douanetoewijzing als gebrek voor projecten ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

Voor informatie over douanevoorwaarden, zie [ de voorwaarden van de Douane ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
