---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: AI-medewerkers configureren
description: Als beheerder van Adobe Workfront, kunt u AI Medewerkers vormen en hen toewijzen aan projecten en taken.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25d5fef46bc8f02e92d778685c2ad6e93439f9ff
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# AI-medewerkers configureren

{{highlighted-preview-article-level}}

AI-medewerkers zijn een manier om AI-agents in uw projecten en taken op te nemen. U kunt een AI Medewerker vormen, dan het toewijzen zoals u een gebruiker zou.

U kunt bijvoorbeeld een AI Collaborator van het type revisor configureren met merkenrichtlijnen en die medewerker toewijzen om een document te reviseren.

Beschikbare typen AI-medewerkers zijn:

* Recensent: Creeer een medewerker gebruikend merken <!-- or Adobe Brand Intelligence-->, dan wijs de medewerker als recensent op activa toe.

  Voor meer informatie, zie [ begonnen worden met de Recensent van de Inhoud van Workfront ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >Reviewer is momenteel het enige beschikbare type AI-deelnemer. In de toekomst zijn er meer mogelijkheden voor AI Collaborator beschikbaar.


## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Standaard, Prime of Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
  </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten



* Uw organisatie moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.

  Voor meer informatie, zie [ Ondertekenen de Gen AI van Adobe overeenkomst ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in de artikelAI Medewerker in Workfront.
* U moet een merk hebben geconfigureerd in Workfront voordat u het kunt gebruiken voor een AI Collaborator van het type Reviewer.

  Voor instructies, zie [ merken voor de Recensent van de Inhoud ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md) creëren en leiden.

## Een nieuwe, van het type AI-deelnemer afkomstige revisor maken

{{step-1-to-setup}}

1. In de linkernavigatie, klik **AI Medewerkers**.
1. Klik **Nieuwe Medewerker** in de hoger-juiste hoek van het scherm.
1. Klik **Recensent**, dan klik **verdergaan**.

   >[!NOTE]
   >
   >Momenteel is alleen het type Revisor beschikbaar. In de toekomst zijn er meer AI-Collaboratortypen beschikbaar.

1. Voer in het veld Naam deelnemer een naam in voor de deelnemer. Dit is de naam die wordt weergegeven in de lijst met beschikbare toewijzingen voor een taak.
   <!--1. Select whether the collaborator will use a brand or Adobe Brand Intelligence for its reviews.-->
   <!--1. (Conditional) If the AI Collaborator will use Adobe Brand Intelligence, select the tenant that it will use.-->
1. <!--(Conditional) If the AI Collaborator will use a Brand,-->Selecteer het merk en de merkrichtlijn die het zal gebruiken.
1. Klik **sparen**.

## AI-medewerkers beheren

U kunt bestaande AI-medewerkers bewerken, kopiëren en verwijderen.

{{step-1-to-setup}}

1. In de linkernavigatie, klik **AI Medewerkers**.
1. (Voorwaardelijk) om een Medewerker uit te geven, klik de naam van de Medewerker u wilt uitgeven, om het even welke veranderingen in het Edit venster van de Medewerker aanbrengen, en **klikken sparen**.
1. (Voorwaardelijk) om een Medewerker te kopiëren, klik het pictogram van het Exemplaar ![ pictogram van het Exemplaar ](assets/copy-ai-collaborator.png) in de rij van de AI Medewerker u wilt kopiëren, de naam van het exemplaar klikken, om het even welke veranderingen in het Edit venster van de Medewerker aanbrengen, en **klikken sparen**.
1. (Voorwaardelijk) om een Medewerker te schrappen, klik het pictogram van de Schrapping ![ pictogram van de Schrapping ](assets/delete-collaborator-icon.png) in de rij van de AI Medewerker u wilt schrappen, dan **Schrapping** klikken.
