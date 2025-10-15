---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Gebruikers een proef laten delen
description: Wanneer u opmerkingen maakt over een proefdruk in de conceptviewer, kunt u andere gebruikers een tag toewijzen om hun opmerkingen via e-mail te verzenden en ze toe te voegen aan de workflow van de proefdruk.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: fe269b088c82e7045ffbb5155d54432e0b413cbe
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Gebruikers een proef laten delen

Wanneer u opmerkingen maakt over een proefdruk in de conceptviewer, kunt u andere gebruikers een tag toewijzen om hun opmerkingen via e-mail te verzenden en ze toe te voegen aan de workflow van de proefdruk.

Wanneer gebruikers worden gelabeld in opmerkingen op een proefdruk, kunnen de gebruikers die u kunt labelen verschillen, afhankelijk van verschillende factoren, zoals de individuele gebruikersmachtigingen en uw lidmaatschap van de organisatie:

* Als u de maker van de proefdruk bent, eigenaar bent of specifieke machtigingen hebt ingeschakeld, kunt u gebruikers buiten de proefdrukworkflow een label geven en de proefdruk met hen delen.
* Als u als externe gebruiker aan de proefdruk bent toegevoegd en u lid bent van een andere omgeving met een andere proefdrukaccount, kunt u alleen die gebruikers van uw oorspronkelijke omgeving een tag toewijzen. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Toegangsvereisten {#access-requirements}

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Alle</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Proefdrukrol</td> 
   <td>Auteur, moderator</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Bewijs van machtigingsprofiel</td> 
   <td>Supervisor of beheerder</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p></td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gebruikers een proef laten delen

De gebruikers met het Profiel van de Toestemming van het Bewijs of de rol van het Bewijs die in de [&#x200B; sectie van de Vereisten van de Toegang &#x200B;](#access-requirements) hierboven wordt geschetst kunnen gebruikers etiketteren om een proef door gebrek te delen. U kunt gebruikers ook labelen om een proefdruk te delen, ongeacht het machtigingsprofiel of de proefdrukrol als u de eigenaar of maker van de proefdruk bent. U kunt gebruikers met een lager machtigingsprofiel of een lagere proefdrukrol toestaan een proefdruk te maken door gebruikers een proefdruk te laten delen tijdens het maken van een proefdruk. Voor meer informatie, zie [&#x200B; het werkschema vormen en reviewers &#x200B;](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) sectie in [&#x200B; toevoegen creeer een geavanceerde proef met een Basis werkschema &#x200B;](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) artikel.

>[!NOTE]
>
>U kunt alleen tags toewijzen aan een externe medewerker die zijn e-mailadres gebruikt als een van de volgende twee dingen waar is:>
>* Een gebruiker in de Workfront-account van uw organisatie heeft het e-mailadres van de medewerker aan een proefdruk toegevoegd.
>* De medewerker heeft het e-mailadres gebruikt om te abonneren op een proefdruk in de Workfront-account van uw organisatie.
>

Een proefdruk in een opmerking labelen en delen:

1. Als u commentaar geeft op een proefdruk, typt u een apestaartje (@) gevolgd door de naam of het e-mailadres van de persoon. Wanneer u begint te typen, verschijnen de beschikbare namen in een drop-down lijst.
1. Selecteer de naam van de persoon wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   >[!TIP]
   >
   >Als u de drop-down lijst wilt sluiten zonder iedereen te selecteren, kunt u de **sleutel van Esc** drukken of overal buiten de lijst klikken.

1. Herhaal stap 1-2 voor alle andere gebruikers die u in de opmerking wilt voorzien van tags.
1. Voltooi de commentaar, dan klik **Post**.
1. (Voorwaardelijk) als u iedereen etiketteerde die niet reeds aan de proef werd toegevoegd, specificeer de rol van het a **Bewijs** en **E-mail alarm** plaatsend voor elke gebruiker die in de doos wordt vermeld die verschijnt, dan klik **mensen en post commentaar** toevoegt.

   ![&#x200B; voeg mensen aan proef &#x200B;](assets/add-people-to-proof-350x220.png) toe

   Voor informatie over proefdrukrollen, zie. Voor informatie over proefe-mailalarm, zie de sectie in artikel [&#x200B; de montages van het e-mailbericht in Workfront Proof &#x200B;](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) vormen.

   Als de proefdruk een Geautomatiseerde Workflow heeft, worden de gebruikers u markering toegevoegd aan het werkgebied u in bent. Voor meer informatie, zie [&#x200B; Geautomatiseerd overzicht van het Werkschema &#x200B;](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Iedereen die u een tag aanbrengt, ontvangt een e-mailbericht over uw proefdrukopmerking, ongeacht de instellingen voor e-mailwaarschuwingen voor proefdrukken die hij gebruikt:

   * Als de gebruiker een dagelijkse samenvatting of per uur per e-mail ontvangt, verzendt Workfront het bericht afzonderlijk en bevat het de informatie over uw proefdrukcommentaar in het samenvattingsbericht.
   * Als de gebruiker waarschuwingen ontvangt voor alle activiteiten of voor reacties op zijn opmerkingen, vervangt de melding de meldingen over deze opmerkingen en antwoorden.

Voor informatie over andere manieren om gebruikers aan een proef toe te voegen, zie [&#x200B; een proef binnen Adobe Workfront &#x200B;](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) delen.
