---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Een statische proefdruk maken voor een website of andere webinhoud
description: U kunt een nieuwe statische proefdruk of een nieuwe versie van een bestaande statische proefdruk voor webinhoud produceren. De inhoud van het Web kan dingen zoals advertenties met het stromen video, HTML animatie, of interactieve banners omvatten, maar het zal in veelvoudige het schermopnamen worden geknipt om het statische proef toe te staan.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 0%

---

# Een statische proefdruk maken voor een website of andere webinhoud

U kunt een nieuwe statische proefdruk of een nieuwe versie van een bestaande statische proefdruk voor webinhoud produceren. De inhoud van het Web kan dingen zoals advertenties met het stromen video, HTML animatie, of interactieve banners omvatten, maar het zal in veelvoudige het schermopnamen worden geknipt om het statische proef toe te staan.

Houd rekening met het volgende wanneer u statische proefdrukken maakt voor een website of andere webinhoud:

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Een statische proefdruk maken voor een website of andere webinhoud

Als u een statisch bewijs wilt maken, moet de website openbaar toegankelijk zijn (niet achter een firewall) of moet de lijst van gewenste personen van uw organisatie het Workfront-domein bevatten. Workfront kan een met een wachtwoord beveiligde website niet vastleggen als een statisch bewijs.

>[!TIP]
>
>We raden interactieve proefdrukken aan in plaats van statische proefdrukken voor interne pagina&#39;s waarvoor verificatie en met een wachtwoord beveiligde pagina&#39;s vereist zijn. Zie voor meer informatie [Overzicht van proefdrukken van interactieve inhoud](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Ga naar het project, de taak of de uitgave waar u een nieuwe websiteproef of een nieuwe versie van bestaande wilt tot stand brengen.
1. Klikken **Documenten** in het linkerdeelvenster.
1. (Voorwaardelijk) Als u een nieuwe proef creeert, klik **Nieuwe toevoegen** en klik vervolgens op **Proef** in het menu dat wordt weergegeven.
1. (Voorwaardelijk) Als u een nieuwe versie van een bestaand bewijs creeert:

   1. Plaats de muisaanwijzer boven de URL-proefdruk waarvoor u een nieuwe versie wilt maken en selecteer deze door op de lichtblauwe achtergrond eromheen te klikken.

      ![Select_proof_by_selecting_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Klikken **Nieuw toevoegen** > **Versie** > **Proef**.

1. Typ de URL van de website die u wilt controleren in het dialoogvenster **Bestanden toevoegen** gebied, dan drukken **Enter**.

   De URL wordt weergegeven onder het vak waarin u de URL hebt getypt.

   ![](assets/url-name-appears-below-350x142.png)

1. Klik op de URL die u hebt toegevoegd.

   Er worden opties weergegeven voor het configureren van de proefdruk van de website.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Optioneel) Als u de naam van de proefdruk wilt wijzigen van de URL van de website naar iets anders, typt u een **Proefnaam.**
1. Controleer of **Schermopname vastleggen** is geselecteerd en gebruikt een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Schermresolutie</strong> </td> 
      <td> <p>Pas de resolutie van de inhoud aan wanneer revisoren de proefdruk bekijken, zodat ze kunnen zien hoe deze wordt weergegeven op apparaten van verschillende formaten, zoals telefoons, tablets en monitoren.</p> <p>Als u meerdere resoluties selecteert, wordt voor elke resolutie die u selecteert een afzonderlijke proefdruk gemaakt.</p> <p>Opmerking: Wanneer een revisor opmerkingen maakt over de proefdruk, bevat de opmerking de resolutie die aangeeft wanneer de opmerking is gemaakt, zodat andere revisoren weten welke resolutie aan de opmerking is gekoppeld. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Zoeken naar subpagina's</strong> </td> 
      <td> <p>Leg de subpagina's van de website en de hoofdpagina's vast. U kunt op Alles selecteren klikken om alle pagina's op te nemen of u kunt alleen op bepaalde pagina's klikken die u wilt opnemen. Met de plus- en minknoppen kunt u de subpaginagebieden van de website uitvouwen en sluiten.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >U kunt de instelling voor schermopname vastleggen niet wijzigen voor volgende versies van de proefdruk die u maakt.

1. Klikken **Gereed**.

   Als u in stap 8 meerdere schermresoluties hebt geselecteerd, bevat de lijst een reeks schermafbeeldingen voor elke resolutie. U kunt deze schermafbeeldingen genereren als afzonderlijke proefdrukken of deze combineren tot één proefdruk (zie onder .). We raden u aan deze te combineren, vooral als u een statische proefdruk maakt voor websites.

   >[!NOTE]
   >
   >Als u een nieuwe versie toevoegt aan een bestaande URL-proefdruk, blijven de opties die op de oorspronkelijke proefdruk of vorige versie zijn geconfigureerd, behouden in deze versie.

1. Klikken **Proef maken** om een eenvoudige proefdruk te maken zonder controleproces.\
   of\
   Ga door met het configureren van een geavanceerde proefdruk:

   * [Een geavanceerde proefdruk maken met een standaardworkflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
