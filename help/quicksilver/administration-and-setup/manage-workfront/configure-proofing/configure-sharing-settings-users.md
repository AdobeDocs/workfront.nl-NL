---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Instellingen voor delen configureren voor uw gebruikers
description: Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u de gebruikersaccounts configureren waarmee proefdrukken kunnen worden gedeeld, aangeven of gebruikers alle versies van een proefdruk kunnen zien en wanneer gebruikers toegang krijgen tot gedeelde items.
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

Als Adobe Workfront-beheerder of Workfront Proof-beheerder kunt u de gebruikersaccounts configureren waarmee proefdrukken kunnen worden gedeeld, aangeven of gebruikers alle versies van een proefdruk kunnen zien en wanneer gebruikers toegang krijgen tot gedeelde items.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Ouder abonnement: Premium of Selecteren</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Beheerder moet zijn geselecteerd in het machtigingsprofiel voor proefdrukken. Voor meer informatie, zie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref"> de het proefdrukken van een gebruiker toegang </a> vormen.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Delen met andere accounts configureren

1. Klik in Workfront op het hoofdmenu ![](assets/main-menu-icon.png) en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om Workfront Proof te openen.

1. Klik **Montages** > **montages van de Rekening**, dan klik de **Montages** tabel.

1. In **het Delen** sectie, rechts van **toestaat delend met**, klik **Opstelling**.

1. Selecteer in de vervolgkeuzelijst die wordt weergegeven een optie om op te geven of u proefdrukken beschikbaar wilt maken voor iedereen, het delen van proefdrukken wilt beperken tot alleen uw eigen account of het wilt beperken tot uw eigen account en eventuele partneraccounts waarmee u samenwerkt.
1. Klik **sparen.**

## Zichtbaarheid voor alle versies van een gedeelde proefdruk configureren

1. Klik in Workfront op het hoofdmenu ![](assets/main-menu-icon.png) en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om Workfront Proof te openen.

1. Klik **Montages** > **montages van de Rekening**, dan klik de **Montages** tabel.

1. In **het Delen** sectie, rechts van **Ontvangers kan alle versies** bekijken, **toelaten** of **onbruikbaar maken** om erop te wijzen of u ontvangers wilt toestaan om alle versies van een proef binnen de het proeven kijker te bekijken wanneer het Bewijs URL wordt toegelaten.

## Zichtbaarheid van proefdrukken configureren op basis van werkstroomwerkgebiedactiviteit

U kunt opgeven wanneer proefdrukken met een geautomatiseerde workflow zichtbaar zijn voor gebruikers die aan een bepaald werkgebied zijn gekoppeld.

>[!NOTE]
>
>* Deze optie is alleen beschikbaar bij gebruik van de zelfstandige Workfront Proof-toepassing. Deze optie is niet beschikbaar bij gebruik van een Workfront Proof-instantie die is geïntegreerd met Workfront of bij proefdrukken in Workfront.
>* Gebruikers ontvangen pas een e-mailmelding over de proefdruk nadat de gebruiker het werkgebied heeft betreden waaraan deze is gekoppeld, ongeacht deze instelling.
>

Om te configureren wanneer proefdrukken met een geautomatiseerde workflow zichtbaar zijn voor gebruikers:

1. Klik in Workfront op het hoofdmenu ![](assets/main-menu-icon.png) en klik vervolgens op Proofing ![](assets/proofing-in-main-menu.png) om Workfront Proof te openen.

1. Klik **Montages** > **montages van de Rekening**, dan klik de **Montages** tabel.

1. In de **het Delen** sectie, laat of maakt **zicht van het Bewijs onbruikbaar dat op werkgebiedactivering** wordt gebaseerd.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Gehandicapten </strong> (gebrek)</td> 
      <td>De proefdrukken zijn zichtbaar voor gebruikers op het tijdstip dat de proefdruk wordt gemaakt.<br><p>Alle gebruikers die zijn gekoppeld aan een werkgebied voor de proefdruk, kunnen de proefdruk direct na het maken van de proefdruk in de zoekresultaten zien.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Toegelaten </strong> </td> 
      <td> <p>De proef is zichtbaar aan gebruikers slechts na het stadium zij met worden <strong> actief.</strong></p> <p><b> NOTA </b>:   
        <ul> 
         <li><em style="font-style: normal;"> nadat u deze optie toelaat, zijn de bestaande proefdrukken nog zichtbaar aan gebruikers die het konden bekijken toen het werd gecreeerd.</em> </li> 
         <li>Nadat een gebruiker toegang heeft tot een versie van een proefdruk (omdat het werkgebied waaraan de gebruiker is gekoppeld actief wordt), kan de gebruiker alleen de versie zien waarin het werkgebied is geactiveerd. Als een vorige versie het werkgebied nooit heeft bereikt waaraan de gebruiker is gekoppeld, kan de gebruiker die versie van de proefdruk niet zien.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
