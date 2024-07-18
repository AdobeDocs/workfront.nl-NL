---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Een proef maken voor interactieve inhoud in een ZIP-bestand
description: U kunt een proef voor niet website interactieve inhoud produceren die in een dossier van het PIT wordt opgeslagen. Voorbeelden van dit type webinhoud zijn onder andere advertenties met streaming video of audio, HTML-animaties, interactieve banners.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Een proef maken voor interactieve inhoud in een ZIP-bestand

U kunt een proef voor niet website interactieve inhoud produceren die in een dossier van het PIT wordt opgeslagen. Voorbeelden van dit type webinhoud zijn onder andere advertenties met streaming video of audio, HTML-animaties, interactieve banners.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Verouderd plan: Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
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
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

## Een proef maken voor interactieve inhoud in een ZIP-bestand

Nadat u interactieve inhoud in een ZIP-bestand aan een proefdruk hebt toegevoegd, maakt Adobe Workfront een proefdruk van de gecomprimeerde documenten. Afhankelijk van de bestandsgrootte kan de laadtijd voor het uploaden variëren. Het maken van grotere bestanden duurt langer. U kunt verder van de pagina navigeren en Workfront gaat door met het maken van uw bestand. De maximale grootte voor het uploaden van bestanden is 4 GB. 

1. Bereid uw inhoud voor door een ZIP-gebundeld bestand te maken.

   Het ZIP-bestand moet aan de volgende vereisten voldoen:

   * Alle elementen, zoals CSS, JavaScript, video&#39;s, geluiden en afbeeldingen, moeten in het bundelbestand worden opgenomen.
   * Zorg ervoor dat het hoofdbestand (zoals index.html, index.htm) zich in de hoofdmap bevindt en dat dit het enige .html/.htm-bestand is dat daar is opgeslagen.

     Als het hoofdbestand niet in de hoofdmap is geplaatst, zoekt Workfront in de map naar het hoofdbestand.

   * De maximale bundelgrootte is 500 MB.
   * In het geval van ZIP-bestanden die in iOS zijn gemaakt, identificeert het programma automatisch de juiste map waarin de inhoud is geplaatst.

1. Ga naar het project, de taak of het probleem waar u het ZIP-bestand wilt uploaden.
1. Klik **Documenten** in het linkerpaneel.
1. Klik **toevoegen Nieuw**, dan klik **Bewijs** in het menu dat verschijnt.
1. In **voeg Dossiers** sectie toe, sleep en laat vallen of doorblader voor het dossier van het PIT u wenst.
1. Klik **creeer proef** om een eenvoudige proef zonder overzichtsproces tot stand te brengen.\
   of\
   Doorgaan met het configureren van een geavanceerde proefdruk:

   * [Een geavanceerde proefdruk maken met een standaardworkflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
