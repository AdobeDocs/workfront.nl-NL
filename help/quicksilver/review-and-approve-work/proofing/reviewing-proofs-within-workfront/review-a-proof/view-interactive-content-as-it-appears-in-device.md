---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: De resolutie voor interactieve proefdrukken wijzigen in de proefdrukviewer
description: U kunt een voorvertoning weergeven van de weergave van een interactieve proefdruk op verschillende apparaten, zodat u kunt zien hoe inhoud wordt weergegeven en hoe hierop wordt gereageerd op basis van verschillende resoluties.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: d4fa663e22daf25fec77be79a452eb207857bdda
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# De resolutie voor interactieve proefdrukken wijzigen in de proefdrukviewer

U kunt een voorvertoning weergeven van de weergave van een interactieve proefdruk op verschillende apparaten, zodat u kunt zien hoe inhoud wordt weergegeven en hoe hierop wordt gereageerd op basis van verschillende resoluties.

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
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

## Weergaven apparaat en resolutie in Desktop Proofing Viewer versus Web Proofing Viewer

Uw Adobe Workfront-beheerder heeft uw systeem zo geconfigureerd dat u interactieve inhoud in de Desktop Proofing Viewer of, als gebundelde inhoud in een ZIP-bestand, in de Web Proofing Viewer bekijkt:

* In de Desktop Proofing Viewer kunt u zien hoe inhoud wordt weergegeven en hoe hierop wordt gereageerd in verschillende resoluties en op verschillende apparaten. Wanneer een revisor een bepaald apparaat opgeeft, wordt de inhoud weergegeven zoals op dat apparaat, met de gebruikersinterfacespecificaties voor het apparaat. Een rode knop op één merk smartphone kan bijvoorbeeld blauw zijn op een ander merk.

* In de webtestviewer kunt u interactieve inhoud weergeven zoals deze wordt weergegeven in de resoluties voor de verschillende apparaten. Maar de Web Proofing Viewer emuleert de inhoud niet met behulp van interfacespecificaties op deze apparaten, zoals knopkleur.

  >[!NOTE]
  >
  >Uw beheerder van Workfront kan douaneapparaten voor gebruikers in uw organisatie vormen, zoals die in [ wordt beschreven het Vormen de Apparaten van de Douane voor Bewijzen ](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) in het artikel [ vormt proefdrukmontages voor uw organisatie ](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

## Een proefdruk weergeven met een vooraf ingesteld apparaat of een vooraf ingestelde resolutie

1. Ga naar de documentlijst met de proefdruk die u wilt openen.
1. Beweeg over het document, dan klik **Open proef**.
1. Klik **Responsief** bij de centrum-bodem van de het proef kijker.

   ![ Resolution_option_in_DPV.png ](assets/resolution-option-in-dpv-350x64.png)

1. Klik in de Desktop Proofing Viewer in de lijst met apparaten en resoluties die wordt weergegeven op de gewenste versie.

   of

   Klik in de webtestviewer in de lijst met resoluties die wordt weergegeven op de gewenste resolutie.

   Als u informatie over nodig hebt hoe deze twee kijkers verschillen, zie [ Verschillen tussen de Web Proofing Kijker en het Overzicht van de Kijker van het Proofing van de Desktop ](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   De interactieve proefdruk wordt weergegeven in de resolutie die u selecteert.

## Een proefdruk weergeven met een aangepaste resolutie-instelling

1. Ga naar de documentlijst met de proefdruk die u wilt openen.
1. Beweeg over het document, dan klik **Open proef**.
1. Klik **Responsief** bij het centrum-onder van de het Proofing Kijker.
1. Typ een douane **Responsieve** resolutie.

   ![ Type_a_custom_resolution_DPV.png ](assets/type-a-custom-resolution-dpv.png)

   of

   Plaats de muisaanwijzer op de interactieve inhoud en sleep de blauwe rand in de rechterbenedenhoek of de rechterrand of onderrand naar de gewenste resolutie.

   ![ Drag_blue_edges_for_resolution.png ](assets/drag-blue-edges-for-resolution-350x251.png)

   De aangepaste resolutie wordt op de volgende locaties weergegeven:

   * In het **paneel van de Resolutie** bij het bodem-centrum van de kijker.\
     ![ Screenshot_2018-05-15_10-27-54.png ](assets/screenshot-2018-05-15-10-27-54.png)

   * In om het even welke commentaren voegen de recensenten aan het bewijs toe. Elke opmerking bevat de schermresolutie die is geselecteerd toen de revisor de opmerking maakte.
