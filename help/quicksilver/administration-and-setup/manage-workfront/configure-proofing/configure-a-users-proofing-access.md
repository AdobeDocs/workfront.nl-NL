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

Voor informatie over het proefdrukken van functionaliteit beschikbaar voor basis en geïntegreerd het proef, zie [ Toegang tot het proefdrukken van functionaliteit in Workfront ](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

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
   <td> <p>U moet een Workfront-beheerder of Workfront Proof-beheerder zijn. Voor informatie over de beheerders van Workfront, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Proofing voor een gebruiker inschakelen en uitschakelen (alleen oudere plannen) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Als uw organisatie een verouderd Select- of Premium Workfront-abonnement gebruikt, kunt u als Workfront-beheerder de proefdrukfunctionaliteit voor de gebruiker in- en uitschakelen.

Wanneer u het proef voor een gebruiker toelaat, laat Workfront de optie voor de proefdrukken van de gebruiker toe om automatisch te produceren.

Hoewel u een gebruiker als het proefdrukken gebruiker kunt toelaten, moet hij of zij beheerdertoestemmingen hebben om rechtstreeks aan de interface van Workfront Proof van het Hoofdmenu van Workfront te navigeren. Voor informatie over hoe u deze optie voor alle het proef gebruikers in uw systeem van Workfront kunt toelaten, zie [ de toegang van Workfront Proof via het Hoofdmenu van Workfront voor alle gebruikers ](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users) vormen.

1. In het **Belangrijkste Menu**, uitgezochte **Gebruikers**.

1. Selecteer een gebruiker, dan klik **uitgeven** pictogram.
1. In de **sectie van de Toegang**, selecteert of schrapt **Gebruiker kan proef** produceren.

## Het proefdrukmachtigingsprofiel van een gebruiker configureren

Het machtigingsprofiel dat u selecteert, wordt aan de gebruikers toegekend voor elke proef die binnen uw organisatie bestaat.

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Gebruikers** ![](assets/users-icon-in-main-menu.png).
1. Selecteer één of meerdere gebruikers, dan klik **uitgeven**.

1. In de **sectie van de Toegang**, klik één van de volgende de toestemmingsopties van Workfront Proof in het **drop-down menu van het Profiel van de Toestemming van de Bewijs**:

   >[!NOTE]
   >
   >Als u op een erfenisplan van Workfront bent, zorg ervoor de **Gebruiker bewijzen** optie kan produceren wordt toegelaten, zoals hierboven verklaard in de sectie [ toelaten en onbruikbaar maken het proef voor een gebruiker (erfenisplannen slechts) ](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Supervisor </strong> </td> 
      <td>Gebruikers kunnen alle proefdrukken beheren en weergeven die op de account van uw organisatie zijn gemaakt. Ze kunnen ook revisoren bewerken die aan deze proefdrukken zijn toegevoegd. Gebruikers met dit machtigingsprofiel kunnen geen gebruikers beheren of Workfront Proof-instellingen bewerken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Manager </strong> </td> 
      <td> <p> Gebruikers kunnen proefdrukken die zijn gemaakt of eigendom zijn van de account van uw organisatie, beheren en bekijken. Ze kunnen alleen proefdrukken van andere gebruikers weergeven wanneer ze als revisor worden toegevoegd. Dit is een standaardinstelling. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Beheerder </strong> </td> 
      <td> Gebruikers krijgen beheerdersmachtigingen in Workfront Proof en kunnen accountinstellingen bewerken. Gebruikers kunnen alle proefdrukken beheren en weergeven die op de account van uw organisatie zijn gemaakt. Dit omvat het toevoegen en verwijderen van revisoren, proefdrukken en opmerkingen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Douane </strong> </td> 
      <td> <p>Alleen beschikbaar als u een aangepast machtigingsprofiel hebt geconfigureerd in Workfront Proof.</p> <p><b> NOTA </b>:  <p>Zorg ervoor dat het toestemmingsprofiel u hier verleent geen hogere toegang dan het Niveau dat van de Toegang van de gebruiker in Workfront (zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> creeert of wijzigt douanetoegangsniveaus </a>) plaatst. Als het hogere toegang verleent, kan de gebruiker tot proeven binnen Workfront Proof toegang hebben die hij of zij niet binnen Workfront kan toegang hebben.</p> <p>Dit is vooral belangrijk als u alle gebruikers van Workfront wilt toestaan om tot Workfront Proof van Workfront direct toegang te hebben zoals die in <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref"> Workfront Proof van de Toegang van Adobe Workfront </a> wordt beschreven.</p> <p>Standaard hebben alleen Workfront-beheerders toegang tot een directe koppeling naar de Workfront Proof-site vanuit de algemene navigatiebalk van Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Het machtigingsprofiel dat u selecteert, wordt aan de gebruikers toegekend voor elke proef die binnen uw organisatie bestaat.

1. Klik **sparen Veranderingen** om de update aan de gebruikersmontages te voltooien.

   >[!NOTE]
   >
   >Wanneer u een gebruiker in Workfront maakt of bijwerkt en het Workfront-e-mailadres van de gebruiker overeenkomt met dat van een in licentie gegeven Workfront Proof-gebruiker, schakelt het systeem het maken van proefdrukken voor de gebruiker in Workfront in. Voor meer informatie, zie [ de synchronisatie van de Gebruiker tussen Adobe Workfront en Workfront Proof ](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Overwegingen

Neem de volgende informatie in overweging wanneer u machtigingen instelt:

* Als u het machtigingsprofiel van een gebruiker wijzigt in een profiel met minder machtigingen, verliest de gebruiker mogelijk de zichtbaarheid van bestaande proefdrukken in Workfront. Dit kan voorkomen wanneer iemand een taak met een gebruiker binnen Workfront deelt, maar deelt niet de proef verbonden aan de taak (zie [ een proef binnen Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [ delen een proef binnen Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* U kunt Workfront Proof-machtigingen alleen instellen vanuit Workfront als uw Workfront-omgeving is geïntegreerd met een Workfront Proof Premium-account. Neem contact op met de Workfront-beheerder als u geen proef kunt gebruiken zoals in deze sectie wordt beschreven.
* Ten minste één gebruiker in uw Workfront-omgeving moet beheerdersmachtigingen hebben voor proofing. Er wordt een foutbericht weergegeven als u probeert beheerdersmachtigingen voor proefdrukken te verwijderen voor alle gebruikers.
* Wanneer u het Workfront Access-niveau van een gebruiker wijzigt in een ander niveau dan Systeembeheerder, wordt het Workfront Proof-machtigingsprofiel van de gebruiker standaard ingesteld op Manager.

* Als u het Workfront Access-niveau wijzigt in Systeembeheerder, verandert het profiel voor Proefmachtigingen in Beheerder.

## Workfront Proof-toegang configureren via Workfront Main Menu voor alle gebruikers {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Door gebrek, slechts kunnen de gebruikers met administratieve rechten binnen Workfront tot Workfront Proof toegang hebben zoals beschreven [ Workfront Proof van de Toegang van Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

U kunt alle gebruikers toegang tot de Workfront Proof-knop geven in het Workfront Main Menu door contact op te nemen met de ondersteuning van Workfront en een aanvraag in te dienen.

>[!IMPORTANT]
>
> Als u alle Workfront-gebruikers rechtstreeks vanuit de Workfront Global Navigation Bar toegang wilt geven tot Workfront Proof, moet u ervoor zorgen dat het machtigingsprofiel voor elke gebruiker niet meer toegang biedt dan het toegangsniveau van de gebruiker in Workfront. Zo voorkomt u dat gebruikers in Workfront Proof proefdrukken openen die ze niet in Workfront kunnen openen. Voor meer informatie, zie [ toelaten en onbruikbaar maken het proef voor een gebruiker (erfenisplannen slechts) ](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Gebruikerstoegang tot de Desktop Proofing Viewer configureren

Als de gebruikers in uw organisatie liever de Desktop Proofing Viewer gebruiken in plaats van de Web Proofing Viewer om interactieve inhoud te controleren, kunt u de Desktop Proofing Viewer zo configureren dat deze automatisch wordt gestart wanneer gebruikers interactieve inhoudsproefdrukken openen. Voor informatie over dit ziet de Desktop het Proofing Kijker en hoe het van de Web het Proofing Kijker verschilt, [ de Desktop het Proofing Kijker ](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) begrijpen en [ Verschillen tussen de Web Proofing Kijker en het Overzicht van de Kijker van de Desktop Proofing ](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Klik vanuit Workfront op het Workfront Proof-pictogram in de algemene navigatiebalk om Workfront Proof te openen.

   ![](assets/proof-access-proofhq-350x39.png)

1. Klik **montages van de Rekening** dichtbij de hoger-juiste hoek van Workfront Proof, dan klik de **Montages** tabel.

1. Onder **Gebreken van het Bewijs**, aan het eind van de **Desktop Proofing Viewer voor Interactieve het proef** rij, klik **Opstelling**.

1. Wijzig de montages van de Kijker van het Proofing van de Desktop, zoals die in [ Desktop het ProofingKijker ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) in het artikel [ worden beschreven vormt proefdrukmontages voor uw organisatie ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Klik **sparen**.

## Aangepaste apparaten configureren voor interactieve proefdrukken

U kunt aangepaste apparaten aan uw systeem toevoegen, zodat gebruikers interactieve inhoud kunnen bekijken en kunnen simuleren hoe de inhoud op een specifiek apparaat wordt weergegeven wanneer zij de Desktop Proofing Viewer gebruiken. (Deze functionaliteit is niet beschikbaar in de webtestviewer, waar gebruikers interactieve inhoud kunnen bekijken, maar alleen zoals deze wordt weergegeven in verschillende resoluties, niet op verschillende apparaten.)

Voor meer informatie, zie [ de interactieve proefdrukresolutie van de Verandering in de het proef kijker ](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Van Workfront, heb toegang tot de interface van Workfront Proof, zoals die in [ wordt beschreven Toegang Workfront Proof van Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Wijzig de montages van de Kijker van de Desktop Proofing, zoals die in [ worden beschreven vormt douaneapparaten voor proeven ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) in het artikel [ bewijsmontages voor uw organisatie ](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) vormen.
