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
source-git-commit: d20215ae2d535ba98ca27ce62aaa28fd372e935a
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# AI-medewerkers configureren

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Het is beschikbaar slechts in het milieu van de Sandbox van de Voorproef.</span>

>[!IMPORTANT]
>
>Content Reviewer is momenteel het enige beschikbare AI Collaborator-type. In de toekomst zijn er meer mogelijkheden voor AI Collaborator beschikbaar.

AI-medewerkers zijn een manier om AI-agents in uw projecten en taken op te nemen. U kunt een AI Medewerker vormen, dan het toewijzen zoals u een gebruiker zou.

U kunt bijvoorbeeld een AI Collaborator van het type revisor configureren met merkenrichtlijnen en die medewerker toewijzen om een document te reviseren.

Beschikbare typen AI-medewerkers zijn:

* Revisor: maak een medewerker met merken of Adobe Brand Intelligence en wijs de medewerker vervolgens toe als revisor voor middelen.

  Voor meer informatie, zie [ begonnen worden met de Recensent van de Inhoud van Workfront ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).


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
* <span class="preview"> om de Intelligentie van het Merk van Adobe voor een Medewerker AI van de Revisor te gebruiken, moet uw organisatie de verenigde overzicht en goedkeuringservaring in Workfront gebruiken. </span>

  <span class="preview"> voor meer informatie, zie [ begonnen met verenigde overzicht en goedkeuring ](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md). </span>

## Een nieuwe, van het type AI-deelnemer afkomstige revisor maken

Reviewer AI Collaborators kunnen worden geconfigureerd voor het gebruik van Workfront-merken of Adobe Brand Intelligence.

* **Banden**: De merken worden gecreeerd in Workfront. U kunt in Workfront merken maken door PDF-bestanden te uploaden die uw merkrichtlijnen bevatten of door handmatig merkelementen in te voeren.
* <span class="preview">**Intelligentie van het Merk Adobe**: Wanneer een Medewerker van AI activa gebruikend de Intelligentie van het Merk van Adobe herziet, kunt u commentaren bekijken die door de Recensent in Frame.io worden gemaakt.  </span>

>[!NOTE]
>
>Content Reviewer is niet beschikbaar in Sandbox-omgevingen.


{{step-1-to-setup}}

1. In de linkernavigatie, klik **AI Medewerkers**.
1. Klik **Nieuwe Medewerker** in de hoger-juiste hoek van het scherm.
1. Klik **Recensent**, dan klik **verdergaan**.

   >[!NOTE]
   >
   >Momenteel is alleen het type Revisor beschikbaar. In de toekomst zijn er meer AI-Collaboratortypen beschikbaar.

1. Voer in het veld Naam deelnemer een naam in voor de deelnemer. Dit is de naam die wordt weergegeven in de lijst met beschikbare toewijzingen voor een taak.
1. <span class="preview"> selecteer of de medewerker een merk of de Intelligentie van het Merk van Adobe voor zijn overzichten zal gebruiken.</span>
1. (Voorwaardelijk) Als de AI Collaborator een merk zal gebruiken, selecteert u het merk en de merkrichtlijn die het zal gebruiken.
1. Klik **sparen**.

## AI-medewerkers beheren

U kunt bestaande AI-medewerkers bewerken, kopiëren en verwijderen.

{{step-1-to-setup}}

1. In de linkernavigatie, klik **AI Medewerkers**.
1. (Voorwaardelijk) om een Medewerker uit te geven, klik de naam van de Medewerker u wilt uitgeven, om het even welke veranderingen in het Edit venster van de Medewerker aanbrengen, en **klikken sparen**.
1. (Voorwaardelijk) om een Medewerker te kopiëren, klik het pictogram van het Exemplaar ![ pictogram van het Exemplaar ](assets/copy-ai-collaborator.png) in de rij van de AI Medewerker u wilt kopiëren, de naam van het exemplaar klikken, om het even welke veranderingen in het Edit venster van de Medewerker aanbrengen, en **klikken sparen**.
1. (Voorwaardelijk) om een Medewerker te schrappen, klik het pictogram van de Schrapping ![ pictogram van de Schrapping ](assets/delete-collaborator-icon.png) in de rij van de AI Medewerker u wilt schrappen, dan **Schrapping** klikken.
