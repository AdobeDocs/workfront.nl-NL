---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Standaardproofingrollen configureren
description: Als beheerder van Adobe Workfront, kunt u de standaard het proefdrukken rollen voor gebruikers en gastgebruikers vormen die tot proeven toegang hebben die in Workfront worden gecreeerd. Iedereen die gebruikers aan een proef toevoegt kan deze rollen voor hen aanpassen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: d64213bf-f270-404f-a45a-6f94c7b7cb91
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Standaardproofingrollen configureren

Als beheerder van Adobe Workfront, kunt u de standaard het proefdrukken rollen voor gebruikers en gastgebruikers vormen die tot proeven toegang hebben die in Workfront worden gecreeerd. Iedereen die gebruikers aan een proef toevoegt kan deze rollen voor hen aanpassen.

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
   <td> <p>U moet een Workfront-beheerder zijn. Voor informatie over de beheerders van Workfront, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref"> een gebruiker volledige administratieve toegang verlenen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Standaardproofingrollen configureren

1. Klik het **Belangrijkste pictogram van het Menu** ![](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, dan klik **Opstelling** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klik **Overzicht en Goedkeuring** dichtbij de bodem van de lijst die op de linkerzijde verschijnt.
1. In de **Rollen voor aangewezen ontvangers van een sectie van de documentproef**, selecteer de standaardrol voor gebruikers en gastgebruikers die aan het werkschema van een bewijs worden toegevoegd.

   Zie [ Rechten verbonden aan het proef rollen ](#rights-associated-with-proofing-roles) hieronder voor een lijst van elke het proef rol en de rechten verbonden aan het.

   >[!NOTE]
   >
   >* Deze instelling is alleen van toepassing op gebruikers die in het Workfront-systeem zijn gemaakt nadat de rol is ingesteld, en niet op bestaande gebruikers.
   >* De persoon die gebruikers aan de proef toevoegt kan deze rol aanpassen, zoals die in [ wordt beschreven voegt gebruikers aan een proef ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [ een proef binnen Adobe Workfront ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) toe.

1. In de **Rollen voor niet-ontvangers die een sectie van de documentproef** openen, selecteer de standaardrol voor gebruikers en gastgebruikers die tot een proef kunnen toegang hebben, maar niet aan het werkschema van de proef worden toegevoegd.

   Deze situatie doet zich voor wanneer gebruikers en gasten toegang hebben tot een document waarvoor een bewijs is gemaakt: zelfs als ze niet zijn toegevoegd aan de proefdrukworkflow, kunnen ze de proefdrukproef openen.

   **Voorbeelden:** hier zijn voorbeelden van hoe u dit het plaatsen kon gebruiken:

   * U selecteert **Gelezen slechts** om alle proefdrukactiviteit zoals het toevoegen van commentaren en het nemen van besluiten aan die te beperken die zijn gevraagd om het te doen.
   * U selecteert **Recensent** omdat u een lid van het team markeringen en commentaren op een proef wilt kunnen toevoegen.

1. Klik **sparen**.

## Rechten verbonden aan het proefdrukken van rollen {#rights-associated-with-proofing-roles}

In de volgende tabel worden elke rol en de bijbehorende rechten weergegeven:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong> Mening een proef </strong> </p> </th> 
   <th> <p><strong> voeg markeringen </strong> toe </p> </th> 
   <th> <p><strong> voeg commentaren </strong> toe </p> </th> 
   <th> <p><strong> geeft eigen commentaren uit als er geen antwoorden zijn </strong> </p> </th> 
   <th> <p><strong> maak een besluit </strong> </p> </th> 
   <th> <p><strong> Schrap commentaren die door anderen worden gemaakt </strong> </p> </th> 
   <th>Opmerkingen oplossen</th> 
   <th>Handelingen toepassen op opmerkingen</th> 
   <th> <p><strong> geef de proef </strong> uit </p> </th> 
   <th>De proefdruk delen met anderen</th> 
   <th>Nieuwe versie maken</th> 
   <th> <p><strong> de goedkeuringsverzoeken van de Mening op het gebied van het Huis </strong> </p> </th> 
   <th>Nieuwe revisoren toevoegen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong> las slechts </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Recensent </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Fiatteur </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Recensent &amp; Fiatteur </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> </td> 
   <td>✓</td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p><strong> Auteur </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p><strong> Moderator </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong> ✓ </strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> <p> </p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> <p>✓</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>De gebruikers op nieuwe plannen van Workfront kunnen auteur of moderatorrollen aan om het even welke gebruikers in het systeem verlenen. De gebruikers op erfenisplannen kunnen auteur of moderatorrollen aan om het even welke gebruiker met een proefvergunning in het systeem verlenen.
