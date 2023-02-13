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
source-wordcount: '508'
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
   <td> <p>U moet een Workfront-beheerder zijn. Voor informatie over Workfront-beheerders raadpleegt u <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Standaardproofingrollen configureren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

   <!--
   <li In the left panel, click Proofs Proof roles.
   -->

1. Klikken **Controle en goedkeuring** onder aan de lijst die links wordt weergegeven.
1. In de **Rollen voor aangewezen ontvangers van een documentbewijs** selecteert u de standaardrol voor gebruikers en gastgebruikers die zijn toegevoegd aan de workflow van een proefdruk.

   Zie [Rechten verbonden aan het proefdrukken van rollen](#rights-associated-with-proofing-roles) hieronder vindt u een lijst van elke proefnemingen en de daaraan verbonden rechten .

   >[!NOTE]
   >
   >* Deze instelling is alleen van toepassing op gebruikers die na het instellen van de rol in het Workfront-systeem zijn gemaakt. niet aan bestaande gebruikers.
   >* De persoon die gebruikers aan de proef toevoegt kan deze rol aanpassen, zoals die in wordt beschreven [Gebruikers aan een proefdruk toevoegen](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md#add) in [Een proefdruk delen in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).


1. In de **Rollen voor niet-ontvangers die een documentbewijs openen** selecteert u de standaardrol voor gebruikers en gastgebruikers die toegang hebben tot een proefdruk, maar die niet worden toegevoegd aan de workflow van de proefdruk.

   Dit gebeurt wanneer gebruikers en gasten toegang hebben tot een document waarvoor een bewijs is gemaakt: zelfs als ze niet zijn toegevoegd aan de proefdrukworkflow, kunnen ze de proefdrukproef openen.

   **Voorbeelden:** Hier volgen enkele voorbeelden van het gebruik van deze instelling:

   * U selecteert **Alleen-lezen** om alle bewijsactiviteiten, zoals het toevoegen van opmerkingen en het nemen van beslissingen, te beperken tot degenen die daartoe zijn gevraagd.
   * U selecteert **Revisor** omdat u wilt dat een teamlid markeringen en opmerkingen kan toevoegen aan een proefdruk.

1. Klikken **Opslaan**.

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
   <th> <p><strong>Een proefdruk weergeven</strong> </p> </th> 
   <th> <p><strong>Markeringen toevoegen</strong> </p> </th> 
   <th> <p><strong>Opmerkingen toevoegen</strong> </p> </th> 
   <th> <p><strong>Eigen opmerkingen bewerken als er geen reacties zijn</strong> </p> </th> 
   <th> <p><strong>Beslissing geven</strong> </p> </th> 
   <th> <p><strong>Opmerkingen van anderen verwijderen</strong> </p> </th> 
   <th>Opmerkingen oplossen</th> 
   <th>Handelingen toepassen op opmerkingen</th> 
   <th> <p><strong>De proefdruk bewerken</strong> </p> </th> 
   <th>De proefdruk delen met anderen</th> 
   <th>Nieuwe versie maken</th> 
   <th> <p><strong>Goedkeuringsaanvragen weergeven in het gedeelte Home</strong> </p> </th> 
   <th>Nieuwe revisoren toevoegen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Alleen-lezen</strong> </p> </td> 
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
   <td> <p><strong>Revisor</strong> </p> </td> 
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
   <td> <p><strong>Fiatteur</strong> </p> </td> 
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
   <td> <p><strong>Revisor en fiatteur</strong> </p> </td> 
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
   <td> <p><strong>Auteur</strong> </p> </td> 
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
   <td> <p><strong>Moderator</strong> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p><strong>✓</strong> </p> </td> 
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
