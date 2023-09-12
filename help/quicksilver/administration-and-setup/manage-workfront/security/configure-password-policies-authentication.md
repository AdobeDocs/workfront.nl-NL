---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Wachtwoordbeleid voor verificatie configureren
description: Als Adobe Workfront-beheerder kunt u wachtwoordbeleidsopties configureren om de verificatie aan te passen aan uw Workfront-systeem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 0%

---

# Wachtwoordbeleid voor verificatie configureren

{{important-admin-console-onboard}}

Als Adobe Workfront-beheerder kunt u wachtwoordbeleidsopties configureren om de verificatie aan te passen aan uw Workfront-systeem.

Wij adviseren dat u authentificatievoorkeur tijdens de implementatie van Workfront vormt en slechts af en toe hen daarna opnieuw beziet.

De verbeterde mogelijkheden voor wachtwoordbeheer zijn binnenkort beschikbaar voor uw organisatie. Gebruik één van beide volgende secties, afhankelijk van of uw organisatie toegang tot de nieuwe authentificatieervaring heeft.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verificatie configureren (beschikbaar voor alle klanten) {#configure-authentication-available-for-all-customers}

De opties van de authentificatie worden getoond voor alle klanten. De verbeterde mogelijkheden voor wachtwoordbeheer zijn binnenkort beschikbaar of zijn mogelijk al beschikbaar voor uw organisatie, zoals beschreven in de sectie [Uitgebreide verificatie configureren)](#configure-enhanced-authentication-coming-soon) in dit artikel.

Verificatievoorkeuren configureren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Verificatie**.

1. Selecteer een van de volgende velden om de verificatie-instellingen voor uw organisatie op te geven:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gebruikers dwingen hun wachtwoord elke <em>&lt;value&gt;</em> dagen</td> 
      <td>Hiermee bepaalt u de tijd die gebruikers nodig hebben om hun Workfront-wachtwoord opnieuw in te stellen. Deze optie is standaard uitgeschakeld. Wanneer u deze inschakelt, kunt u kiezen tussen 30, 60, 90, 120, 180 dagen. De standaardwaarde is 30 dagen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers mogen niet hetzelfde wachtwoord instellen als hun vorige wachtwoord <em>&lt;value&gt;</em> wachtwoorden</td> 
      <td> <p>In dit veld kunnen gebruikers geen wachtwoorden voor een bepaald aantal voorinstellingen opnieuw gebruiken. Dit veld is standaard uitgeschakeld. Wanneer u het toelaat, kunt u deze waarde aan 5 plaatsen, 10, of 15 terugstellen alvorens een wachtwoord kan worden opnieuw gebruikt.</p> <p>Als deze optie is geselecteerd, kunnen gebruikers hun wachtwoorden niet meer dan een keer op een bepaalde dag opnieuw instellen</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Als vijf opeenvolgende keren een onjuist wachtwoord is ingevoerd, moet u de account vergrendelen voor <em>&lt;value&gt;</em> minuten: </td> 
      <td> <p>Selecteer hoe lang een gebruiker uit Workfront zal worden gesloten na het ingaan van een onjuist wachtwoord vijf opeenvolgende tijden. Deze optie is standaard ingeschakeld en de wachttijd is 10 minuten. U kunt accounts 10 minuten, 30 minuten, 1 uur, 8 uur of 24 uur vergrendelen. </p> <p>Door het handmatig opnieuw instellen van het wachtwoord voor de gebruiker wordt deze standaardwachtwaarde genegeerd. <br>Gebruikers kunnen hun eigen wachtwoorden opnieuw instellen wanneer deze via het aanmeldingsscherm zijn vergrendeld. Voor meer informatie over hoe ze hun wachtwoord opnieuw kunnen instellen, raadpleegt u <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">Wachtwoord opnieuw instellen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wachtwoorden moeten ten minste bevatten <em>&lt;value&gt;</em> verschillende typen tekens:</td> 
      <td> <p>Hiermee bepaalt u hoe sterke gebruikerswachtwoorden moeten zijn door het aantal verschillende typen tekens te selecteren die in de wachtwoorden zijn vereist.</p> <p>Een herkenbaar woordenboek kan niet als wachtwoord worden gebruikt.<br>Workfront vereist standaard dat wachtwoorden ten minste twee van de volgende tekens bevatten (u kunt ook 3 van deze tekens invoeren als u een geldig wachtwoord wilt invoeren): </p> 
       <ul> 
        <li>Hoofdletters</li> 
        <li>Kleine letters</li> 
        <li>Getallen</li> 
        <li>Symbolen</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

## Uitgebreide verificatie configureren{#configure-enhanced-authentication-coming-soon}

Deze sectie beschrijft de verbeterde authentificatieervaring, die nog niet voor uw organisatie beschikbaar zou kunnen zijn. Als uw organisatie niet naar de nieuwe authentificatieervaring is gemigreerd, moet u de authentificatiemontages vormen, zoals die in worden beschreven [Verificatie configureren (beschikbaar voor alle klanten)](#configure-authentication-available-for-all-customers).

Uitgebreide verificatievoorkeuren configureren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Verbeterde verificatie**.
1. In de **Wachtwoordlengte** Voer het minimale aantal tekens in dat vereist is voor een geldig wachtwoord.

   Workfront vereist ten minste 6 tekens.

1. (Optioneel) In het dialoogvenster **Wachtwoordvereisten** selecteert u de typen tekens die in gebruikerswachtwoorden zijn vereist.

   U kunt de sterkte van gebruikerswachtwoorden verhogen door om het even welk of alle types van karakters in de sectie van de Vereiste van het Wachtwoord te vereisen. De volgende opties zijn beschikbaar:

   | Kleine letters | Ten minste één kleine letter vereisen |
   |---|---|
   | Hoofdletters | Ten minste één hoofdletter vereisen |
   | Getallen | Ten minste één getal vereisen |
   | Speciale tekens | Ten minste één speciaal teken vereisen |

   {style="table-layout:auto"}

1. Klikken **Opslaan**.
