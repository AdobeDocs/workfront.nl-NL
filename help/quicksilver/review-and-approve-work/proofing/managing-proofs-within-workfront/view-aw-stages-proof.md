---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Geautomatiseerde werkstroomfasen weergeven op een proefdruk
description: U kunt de voortgang van een proefdruk die is geconfigureerd met een geautomatiseerde workflow eenvoudig bijhouden. U kunt het werk dat al in de proeffasen is uitgevoerd, weergeven, wijzigen, toevoegen, starten en vergrendelen.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Geautomatiseerde werkstroomfasen weergeven op een proefdruk

U kunt de voortgang van een proefdruk die is geconfigureerd met een geautomatiseerde workflow eenvoudig bijhouden. U kunt het werk dat al in de proeffasen is uitgevoerd, weergeven, wijzigen, toevoegen, starten en vergrendelen.

Voor informatie over het toevoegen van stadia en gebruikers aan een proef met een Geautomatiseerd Werkschema, zie [ stadia en gebruikers aan een Geautomatiseerd Werkschema op een proef ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md) toevoegen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Verouderd abonnement: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

## Bekijk het Geautomatiseerde diagram van het Werkschema

1. In een documentlijst die het document bevat, beweegt zich over de rij die het document bevat, dan klik **het Proofing Workflow**.

   Het diagram voor de Geautomatiseerde Werkstroom toont net onder de titel van het Werkschema.

   De fasen in het diagram zijn als volgt gemarkeerd:

   ![ dot.png ](assets/dot.png) Actief stadium

   ![ gray_dot.png ](assets/grey-dot.png) Inactief werkgebied\
   ![ sbw-key-icon.png ](assets/sbw-key-icon.png)  Privéstadium

   ![ sbw-hanglock-icon.png ](assets/sbw-padlock-icon.png)  Vergrendeld werkgebied

   De lijnen tussen de stadia geven de afhankelijkheden tussen de fasen aan. De lijnen die leiden tot inactieve stadia worden gestippeld tot het werkgebied wordt geactiveerd.

   U kunt de muisaanwijzer boven een werkgebied in het diagram plaatsen om de voortgang van het werkgebied weer te geven. Als het werkgebied niet actief is en u beschikt over bewerkingsrechten voor het werkgebied, kunt u op de knop Werkgebied activeren ![](assets/activate-stage-btn.png) klikken om het werkgebied te starten. Als het werkgebied actief is en u beschikt over bewerkingsrechten in het werkgebied, kunt u het vergrendelen. ![](assets/lock-stage-btn.png) Raadpleeg voor meer informatie over de voortgangsbalk (S, O, C, D)  [ Mening de Voortgang en de Status van een Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Een werkgebied weergeven

1. In een documentlijst die het document bevat, beweegt zich over de rij die het document bevat, dan klik **het Proofing Workflow**.
1. Klik in het diagram op het werkgebied dat u wilt weergeven.

   ![](assets/view-stage-diagram-350x204.png)

1. Als u de details van een werkgebied wilt uitvouwen, klikt u op de pijl sideways onder de naam van het werkgebied.

   ![](assets/stage-details-caret-350x167.png)

## Alle fasen weergeven

Om alle stadia in een Geautomatiseerde Werkschema te bekijken:

1. Klik de knoop van de Mening van de Verandering bij de bovenkant van de pagina ![](assets/change-view-btn.png), dan klik **Mening alle stadia**.

   Alle fasen van de geautomatiseerde workflow worden vermeld in de sectie, maar de details worden verborgen.

1. Klik op de pijl sideways onder de naam om de details van een werkgebied uit te vouwen.

## Alle fasen in detail weergeven

Om alle stadia van uw Geautomatiseerde Werkschema met hun uitgevouwen details te bekijken:

1. Klik de knoop van de Mening van de Verandering bij de bovenkant van de pagina ![](assets/change-view-btn.png), dan klik **Mening alle stadia in detail**.
1. Klik op de pijl omlaag onder de naam om de details van een werkgebied weer te geven.
