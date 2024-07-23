---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Een proefdruk van meerdere pagina's maken
description: U kunt meerdere bestanden combineren tot één proefdruk van meerdere pagina's. Revisoren kunnen de navigatiegereedschappen in de conceptviewer gebruiken om door de pagina's te bladeren in een proefdruk van meerdere pagina's.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 0%

---

# Een proefdruk van meerdere pagina&#39;s maken

U kunt meerdere bestanden combineren tot één proefdruk van meerdere pagina&#39;s. Revisoren kunnen de navigatiegereedschappen in de conceptviewer gebruiken om door de pagina&#39;s te bladeren in een proefdruk van meerdere pagina&#39;s.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunning, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Een proefdruk van meerdere pagina&#39;s maken

Als deze optie is ingeschakeld, zijn statische bestanden en websites beschikbaar in één proefdruk. Als deze optie is uitgeschakeld, worden alle documenten en websites gegenereerd als afzonderlijke proefdrukken en kunt u maximaal 100 bestanden tegelijk uploaden.

Een proefdruk van meerdere pagina&#39;s maken:

1. Ga naar het project, de taak, of de kwestie waar u de proef wilt, dan klik de **sectie van Documenten**.
1. Klik **toevoegen nieuw** > **Bewijs**.
1. Sleep de bestanden en zet ze neer of blader en selecteer ze in de bestandsverkenner. U kunt maximaal 50 bestanden tegelijk uploaden. Voor informatie over dossiergrenzen, zie de [ sectie van Overwegingen ](#considerations) in dit artikel.

   >[!NOTE]
   >
   >Interactieve bestanden, zoals video&#39;s en interactieve websites, kunnen niet worden gecombineerd tot één proefdruk.

1. Onder **Enige proef**, laat de optie toe, **combineer alle compatibele dossiers in enige proef**.
1. Op het **gebied van de naam van het Bewijs**, specificeer een nieuwe naam voor de gecombineerde proef.
1. (Optioneel) Wijzig de volgorde van de bestanden in de lijst met bestanden die u hebt geüpload door ze te slepen. De volgorde van de bestanden is de paginavolgorde van de gecombineerde proefdruk.
1. (Facultatief) om één enkel dossier uit de Nieuwe proefdruk te verwijderen pagina, over het dossier te bewegen en het **pictogram van het Afval** te klikken dat op het recht verschijnt.

   of

   Om alle geuploade dossiers te schrappen meteen, klik **schrapping allen** in de hoger-juiste hoek van de lijst.

1. Nadat alle bestanden zijn geüpload, moet u bepalen of u een standaardproefdruk of een automatische proefdruk wilt configureren:

   * Met een standaardproefdruk kunt u net zoveel revisoren toevoegen als u wilt aan een proefdruk, maar deze zijn niet geordend in stappen. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt. Om een basisproef te vormen, zie [ een geavanceerd bewijs met een Basiswerkschema ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) creëren.
   * Met een automatische proefdruk wordt de proefdruk van het stadium naar het stadium verplaatst en Adobe Workfront waarschuwt elke gebruiker wanneer het zijn beurt is om het te herzien. om een geautomatiseerd bewijs te vormen, zie [ een geavanceerd bewijs met een Geautomatiseerd werkschema ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md) creëren.

## Overwegingen {#considerations}

Houd rekening met het volgende wanneer u bestanden combineert tot één proefdruk:

* U kunt maximaal 500 afzonderlijke bestanden uploaden.
* U kunt statische bestanden van verschillende typen combineren (bijvoorbeeld PDF, JPG, DOC, PPT, EXC) tot een totaal van 2.000 pagina&#39;s.
* U kunt statische webvastleggingen combineren.
* U kunt GIF-bestanden combineren, maar geanimeerde GIFFEN worden als statische bestanden verwerkt.
* U kunt AV-bestanden en interactieve webvastleggingen niet combineren.
* Het duimnagelbeeld van de proef wordt genomen van de eerste pagina van de proef (zie [ Beheer de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* U kunt de namen controleren van bestanden die zijn gecombineerd om de proefdruk te maken op de pagina Proefgegevens. Voor meer informatie, zie [ Beheren de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Als de optie voor het downloaden van de originele bestanden is ingeschakeld op de proefdruk, kunt u alle gecombineerde bestanden downloaden om de proefdruk te maken als ZIP-bestand. Zie voor meer informatie  [ de Dossiers van de Download die in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md) worden opgeslagen.
