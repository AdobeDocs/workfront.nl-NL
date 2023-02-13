---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Een proefdruk van meerdere pagina's maken
description: U kunt meerdere bestanden combineren tot één proefdruk van meerdere pagina's. Revisoren kunnen de navigatiegereedschappen in de conceptviewer gebruiken om door de pagina's te bladeren in een proefdruk van meerdere pagina's.
author: Courtney
feature: Digital Content and Documents
exl-id: a8ad80d8-0758-4fea-824e-8c206424e295
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 0%

---

# Een proefdruk van meerdere pagina&#39;s maken

U kunt meerdere bestanden combineren tot één proefdruk van meerdere pagina&#39;s. Revisoren kunnen de navigatiegereedschappen in de conceptviewer gebruiken om door de pagina&#39;s te bladeren in een proefdruk van meerdere pagina&#39;s.

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

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, licentie of proefmachtigingsprofiel u hebt.

## Een proefdruk van meerdere pagina&#39;s maken

Als deze optie is ingeschakeld, zijn statische bestanden en websites beschikbaar in één proefdruk. Als deze optie is uitgeschakeld, worden alle documenten en websites gegenereerd als afzonderlijke proefdrukken en kunt u maximaal 100 bestanden tegelijk uploaden.

Een proefdruk van meerdere pagina&#39;s maken:

1. Ga naar het project, de taak, of de kwestie waar u het proef wilt, dan klik **Documenten** sectie.
1. Klikken **Nieuw toevoegen** > **Proef** .
1. Sleep de bestanden en zet ze neer of blader en selecteer ze in de bestandsverkenner. U kunt maximaal 50 bestanden tegelijk uploaden. Voor informatie over bestandslimieten raadpleegt u de [Overwegingen](#considerations) in dit artikel.

   >[!NOTE]
   >
   >Interactieve bestanden, zoals video&#39;s en interactieve websites, kunnen niet worden gecombineerd tot één proefdruk.

1. Onder **Enkelvoudig bewijs** de optie in te schakelen, **Alle compatibele bestanden combineren tot één proefdruk**.
1. In de **Proefnaam** geeft u een nieuwe naam op voor de gecombineerde proefdruk.
1. (Optioneel) Wijzig de volgorde van de bestanden in de lijst met bestanden die u hebt geüpload door ze te slepen. De volgorde van de bestanden is de paginavolgorde van de gecombineerde proefdruk.
1. (Optioneel) Als u één bestand van de pagina Nieuwe proefdruk wilt verwijderen, plaatst u de muis boven het bestand en klikt u op de knop **Prullenbak** aan de rechterkant.

   of

   Als u alle geüploade bestanden tegelijk wilt verwijderen, klikt u op **Alles verwijderen** in de rechterbovenhoek van de lijst.

1. Nadat alle bestanden zijn geüpload, moet u bepalen of u een standaardproefdruk of een automatische proefdruk wilt configureren:

   * Met een standaardproefdruk kunt u net zoveel revisoren toevoegen als u wilt aan een proefdruk, maar deze zijn niet geordend in stappen. Alle revisoren die u toevoegt, hebben direct toegang tot de proefdruk nadat u deze hebt gemaakt. Om een basisproef te vormen, zie [Een geavanceerde proefdruk maken met een standaardworkflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md).
   * Met een automatische proefdruk wordt de proefdruk van het stadium naar het stadium verplaatst en Adobe Workfront waarschuwt elke gebruiker wanneer het zijn beurt is om het te herzien. om een geautomatiseerde proef te vormen, zie [Een geavanceerde proefdruk maken met een geautomatiseerde workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Overwegingen {#considerations}

Houd rekening met het volgende wanneer u bestanden combineert tot één proefdruk:

* U kunt maximaal 500 afzonderlijke bestanden uploaden.
* U kunt statische bestanden van verschillende typen combineren (bijvoorbeeld PDF, JPG, DOC, PPT, EXC) tot een totaal van 2.000 pagina&#39;s.
* U kunt statische webvastleggingen combineren.
* U kunt GIFFEN bestanden combineren. geanimeerde GIFFEN worden echter verwerkt als statische bestanden.
* U kunt AV-bestanden en interactieve webvastleggingen niet combineren.
* De miniatuurafbeelding van de proefdruk is afkomstig van de eerste pagina van de proefdruk (zie [Proefdrukgegevens beheren in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md)).
* U kunt de namen controleren van bestanden die zijn gecombineerd om de proefdruk te maken op de pagina Proefgegevens. Zie voor meer informatie [Proefdrukgegevens beheren in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
* Als de optie voor het downloaden van de originele bestanden is ingeschakeld op de proefdruk, kunt u alle gecombineerde bestanden downloaden om de proefdruk te maken als ZIP-bestand. Zie voor meer informatie  [Bestanden downloaden die zijn opgeslagen in Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/download-files-stored.md).
