---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: De proefdruktoegang van een gebruiker configureren
description: Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u de toegang van een gebruiker configureren om proefdrukken te maken en weer te geven in Workfront en Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# De proefdruktoegang van een gebruiker configureren

Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u de toegang van een gebruiker configureren om proefdrukken te maken en weer te geven in Workfront en Workfront Proof.

Voor informatie over de proefdrukfunctionaliteit beschikbaar voor basis en geïntegreerde proefdrukken, zie [Toegang tot proefdrukfunctionaliteit in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een Workfront-beheerder of Workfront Proof-beheerder zijn. Voor informatie over Workfront-beheerders raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Proofing voor een gebruiker inschakelen en uitschakelen (alleen oudere plannen) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Als uw organisatie een verouderd Select- of Premium Workfront-abonnement gebruikt, kunt u als Workfront-beheerder de proefdrukfunctionaliteit voor de gebruiker in- en uitschakelen.

Wanneer u het proef voor een gebruiker toelaat, laat Workfront de optie voor de proefdrukken van de gebruiker toe om automatisch te produceren.

Hoewel u een gebruiker als het proefdrukken gebruiker kunt toelaten, moet hij of zij beheerdertoestemmingen hebben om rechtstreeks aan de interface van het Bewijs van Workfront van het Hoofdmenu van Workfront te navigeren. Voor informatie over hoe u deze optie kunt inschakelen voor alle proefdrukgebruikers in uw Workfront-systeem, raadpleegt u [Workfront Proeftoegang voor alle gebruikers configureren via het hoofdmenu van Workfront](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. In de **Hoofdmenu**, selecteert u **Gebruikers**.

1. Selecteer een gebruiker en klik op de knop **Bewerken** pictogram.
1. In de **Toegang** sectie, selecteren of deselecteren **Gebruiker kan proefdrukken genereren**.

## Het proefdrukmachtigingsprofiel van een gebruiker configureren

Het machtigingsprofiel dat u selecteert, wordt aan de gebruikers toegekend voor elke proef die binnen uw organisatie bestaat.

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer een of meer gebruikers en klik op **Bewerken**.

1. In de **Toegang** klikt u op een van de volgende Workfront Proof-machtigingsopties in het dialoogvenster **Bewijs van machtigingsprofiel** vervolgkeuzemenu:

   >[!NOTE]
   >
   >Als u een verouderd Workfront-plan hebt, controleert u of de **Gebruiker kan proefdrukken genereren** deze optie is ingeschakeld, zoals hierboven in de sectie wordt uitgelegd [Proofing voor een gebruiker inschakelen en uitschakelen (alleen oudere plannen)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Gebruikers kunnen alle proefdrukken beheren en weergeven die op de account van uw organisatie zijn gemaakt. Ze kunnen ook revisoren bewerken die aan deze proefdrukken zijn toegevoegd. Gebruikers met dit machtigingsprofiel kunnen geen gebruikers beheren of Workfront Proof-instellingen bewerken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Gebruikers kunnen proefdrukken die zijn gemaakt of eigendom zijn van de account van uw organisatie, beheren en bekijken. Ze kunnen alleen proefdrukken van andere gebruikers weergeven wanneer ze als revisor worden toegevoegd. Dit is een standaardinstelling. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beheerder</strong> </td> 
      <td> Gebruikers krijgen beheerdersmachtigingen in Workfront Proof en kunnen accountinstellingen bewerken. Gebruikers kunnen alle proefdrukken beheren en weergeven die op de account van uw organisatie zijn gemaakt. Dit omvat het toevoegen en verwijderen van revisoren, proefdrukken en opmerkingen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Aangepast</strong> </td> 
      <td> <p>Alleen beschikbaar als u een aangepast machtigingsprofiel hebt geconfigureerd in Workfront Proof.</p> <p><b>OPMERKING</b>:  <p>Zorg ervoor dat het machtigingsprofiel dat u hier toekent, geen hogere toegang biedt dan de instelling Toegangsniveau van de gebruiker in Workfront (zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>). Als het hogere toegang verleent, kan de gebruiker tot proef binnen Workfront Bewijs toegang hebben dat hij of zij niet binnen Workfront kan toegang hebben.</p> <p>Dit is vooral belangrijk als u alle Workfront-gebruikers rechtstreeks vanuit de Workfront toegang wilt geven tot de Workfront Proof, zoals beschreven in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Workfront Proof openen vanuit Adobe Workfront</a>.</p> <p>Standaard hebben alleen Workfront-beheerders toegang tot een directe koppeling naar de Workfront Proof-site vanuit de algemene navigatiebalk van Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Het machtigingsprofiel dat u selecteert, wordt aan de gebruikers toegekend voor elke proef die binnen uw organisatie bestaat.

1. Klikken **Wijzigingen opslaan** om de update van de gebruikersinstellingen te voltooien.

   >[!NOTE]
   >
   >Wanneer u een gebruiker in Workfront maakt of bijwerkt en het Workfront-e-mailadres van de gebruiker overeenkomt met dat van een in licentie gegeven Workfront Proof-gebruiker, schakelt het systeem het testen voor de gebruiker in Workfront in. Zie voor meer informatie [Gebruikerssynchronisatie tussen Adobe Workfront en Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Overwegingen

Neem de volgende informatie in overweging wanneer u machtigingen instelt:

* Als u het machtigingsprofiel van een gebruiker wijzigt in een profiel met minder machtigingen, verliest de gebruiker mogelijk de zichtbaarheid van bestaande proefdrukken in Workfront. Dit kan zich voordoen wanneer iemand een taak deelt met een gebruiker in Workfront, maar de proefdruk die aan de taak is gekoppeld niet deelt (zie [Een proefdruk delen in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Een proefdruk delen in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* U kunt Workfront Proof-machtigingen alleen instellen vanuit Workfront als uw Workfront-omgeving is geïntegreerd met een Workfront Proof Premium-account. Neem contact op met de Workfront-beheerder als u geen proef kunt gebruiken zoals in deze sectie wordt beschreven.
* Ten minste één gebruiker in uw Workfront-omgeving moet beheerdersmachtigingen hebben voor proofing. Er wordt een foutbericht weergegeven als u probeert beheerdersmachtigingen voor proefdrukken te verwijderen voor alle gebruikers.
* Wanneer u het Workfront Access-niveau van een gebruiker wijzigt in een ander niveau dan Systeembeheerder, wordt het Workfront Proof-machtigingsprofiel van de gebruiker standaard ingesteld op Manager.

* Als u het Workfront Access-niveau wijzigt in Systeembeheerder, verandert het profiel voor Proefmachtigingen in Beheerder.

## Workfront Proeftoegang voor alle gebruikers configureren via het hoofdmenu van Workfront {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Standaard hebben alleen gebruikers met beheerdersrechten in Workfront toegang tot Workfront Proof zoals beschreven  [Workfront Proof openen vanuit Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

U kunt alle gebruikers toegang geven tot de knop Workfront-proef in het hoofdmenu van Workfront door contact op te nemen met de ondersteuning van Workfront en een aanvraag in te dienen.

>[!IMPORTANT]
>
> Als u alle Workfront-gebruikers rechtstreeks vanuit de Workfront Global Navigation Bar toegang wilt geven tot Workfront Proof, moet u ervoor zorgen dat het machtigingsprofiel voor elke gebruiker niet meer toegang biedt dan het toegangsniveau van de gebruiker in Workfront. Zo voorkomt u dat gebruikers proefdrukken openen in Workfront Proof waartoe ze geen toegang hebben in Workfront. Zie voor meer informatie [Proofing voor een gebruiker inschakelen en uitschakelen (alleen oudere plannen)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Gebruikerstoegang tot de Desktop Proofing Viewer configureren

Als de gebruikers in uw organisatie liever de Desktop Proofing Viewer gebruiken in plaats van de Web Proofing Viewer om interactieve inhoud te controleren, kunt u de Desktop Proofing Viewer zo configureren dat deze automatisch wordt gestart wanneer gebruikers interactieve inhoudsproefdrukken openen. Voor informatie hierover raadpleegt u de Desktop Proofing Viewer en hoe deze afwijkt van de Web Proofing Viewer. [De Desktop Proofing Viewer begrijpen](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) en [Verschillen tussen de webtestviewer en het overzicht van de Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Klik in Workfront op het Workfront-proefdrukpictogram in de algemene navigatiebalk om Workfront Proof te openen.

   ![](assets/proof-access-proofhq-350x39.png)

1. Klikken **Accountinstellingen** in de rechterbovenhoek van Workfront Proof en klik vervolgens op de knop **Instellingen** tab.

1. Onder **Standaardwaarden proefdrukken** aan het einde van de **Desktop Proofing Viewer voor interactieve proefdrukken** rij, klik **Instellen**.

1. De instellingen van de Desktop Proofing Viewer wijzigen, zoals beschreven in [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) in het artikel [Proofinginstellingen voor uw organisatie configureren](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Klikken **Opslaan**.

## Aangepaste apparaten configureren voor interactieve proefdrukken

U kunt aangepaste apparaten aan uw systeem toevoegen, zodat gebruikers interactieve inhoud kunnen bekijken en kunnen simuleren hoe de inhoud op een specifiek apparaat wordt weergegeven wanneer zij de Desktop Proofing Viewer gebruiken. (Deze functionaliteit is niet beschikbaar in de webtestviewer, waar gebruikers interactieve inhoud kunnen bekijken, maar alleen zoals deze wordt weergegeven in verschillende resoluties, niet op verschillende apparaten.)

Zie voor meer informatie [De resolutie voor interactieve proefdrukken wijzigen in de proefdrukviewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Vanuit Workfront opent u de interface van Workfront Proof, zoals beschreven in [Workfront Proof openen vanuit Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. De instellingen van de Desktop Proofing Viewer wijzigen, zoals beschreven in [Aangepaste apparaten configureren voor proefdrukken](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) in het artikel [Proofinginstellingen voor uw organisatie configureren](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
