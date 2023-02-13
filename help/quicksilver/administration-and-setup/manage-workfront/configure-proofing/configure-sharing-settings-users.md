---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Instellingen voor delen configureren voor uw gebruikers
description: Als beheerder van Adobe Workfront of Workfront Proof, kunt u de gebruikersrekeningen vormen waarmee de proefdrukken kunnen worden gedeeld, of de gebruikers alle versies van een proef, en de timing kunnen zien wanneer de gebruikers toegang tot gedeelde punten krijgen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Instellingen voor delen configureren voor uw gebruikers

Als beheerder van Adobe Workfront of Workfront Proof, kunt u de gebruikersrekeningen vormen waarmee de proefdrukken kunnen worden gedeeld, of de gebruikers alle versies van een proef, en de timing kunnen zien wanneer de gebruikers toegang tot gedeelde punten krijgen.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Premium of Selecteren</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Beheerder moet zijn geselecteerd in het machtigingsprofiel voor proefdrukken. Zie voor meer informatie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">De proefdruktoegang van een gebruiker configureren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Delen met andere accounts configureren

1. Vanuit Workfront klikt u op het hoofdmenu ![](assets/main-menu-icon.png)en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om toegang te krijgen tot Workfront Proof.

1. Klikken **Instellingen** > **Accountinstellingen** klikt u op de knop **Instellingen** tab.

1. In de **Delen** , rechts van **Delen met toestaan**, klikt u op **Instellen**.

1. Selecteer in de vervolgkeuzelijst die wordt weergegeven een optie om op te geven of u proefdrukken beschikbaar wilt maken voor iedereen, het delen van proefdrukken wilt beperken tot alleen uw eigen account of het wilt beperken tot uw eigen account en eventuele partneraccounts waarmee u samenwerkt.
1. Klikken **Opslaan.**

## Zichtbaarheid voor alle versies van een gedeelde proefdruk configureren

1. Vanuit Workfront klikt u op het hoofdmenu ![](assets/main-menu-icon.png)en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om toegang te krijgen tot Workfront Proof.

1. Klikken **Instellingen** > **Accountinstellingen** klikt u op de knop **Instellingen** tab.

1. In de **Delen** , rechts van **Ontvangers kunnen alle versies weergeven**, selecteert u **Inschakelen** of **Uitschakelen** om aan te geven of u wilt dat ontvangers alle versies van een proefdruk in de proefdrukviewer kunnen weergeven wanneer de URL van proef is ingeschakeld.

## Zichtbaarheid van proefdrukken configureren op basis van werkstroomwerkgebiedactiviteit

U kunt opgeven wanneer proefdrukken met een geautomatiseerde workflow zichtbaar zijn voor gebruikers die aan een bepaald werkgebied zijn gekoppeld.

>[!NOTE]
>
>* Deze optie is alleen beschikbaar als u de zelfstandige Workfront Proof-toepassing gebruikt. is niet beschikbaar bij het gebruik van een Workfront Proof-instantie die is geïntegreerd met Workfront of bij proefdrukken in Workfront.
>* Gebruikers ontvangen pas een e-mailmelding over de proefdruk nadat de gebruiker het werkgebied heeft betreden waaraan deze is gekoppeld, ongeacht deze instelling.
>


Om te configureren wanneer proefdrukken met een geautomatiseerde workflow zichtbaar zijn voor gebruikers:

1. Vanuit Workfront klikt u op het hoofdmenu ![](assets/main-menu-icon.png)en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om toegang te krijgen tot Workfront Proof.

1. Klikken **Instellingen** > **Accountinstellingen** klikt u op de knop **Instellingen** tab.

1. In de **Delen** sectie, in- of uitschakelen **Zichtbaarheid proefdrukken op basis van werkgebiedactivering**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Uitgeschakeld</strong> (standaard)</td> 
      <td>De proefdrukken zijn zichtbaar voor gebruikers op het tijdstip dat de proefdruk wordt gemaakt.<br><p>Elke gebruiker die bij een werkgebied voor de proefdruk hoort, kan de proefdruk direct na het maken van de proefdruk in de zoekresultaten zien.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ingeschakeld</strong> </td> 
      <td> <p>Proefdrukken zijn pas zichtbaar voor gebruikers nadat het werkgebied waaraan ze zijn gekoppeld, is voltooid <strong>actief.</strong></p> <p><b>OPMERKING</b>:   
        <ul> 
         <li><em style="font-style: normal;">Nadat u deze optie hebt ingeschakeld, zijn bestaande proefdrukken nog steeds zichtbaar voor gebruikers die deze konden bekijken toen ze werden gemaakt.</em> </li> 
         <li>Nadat een gebruiker toegang heeft tot een versie van een proefdruk (omdat het werkgebied waaraan de gebruiker is gekoppeld actief wordt), kan de gebruiker alleen de versie zien waarin het werkgebied is geactiveerd. Als een vorige versie het werkgebied nooit heeft bereikt waaraan de gebruiker is gekoppeld, kan de gebruiker die versie van de proefdruk niet zien.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
