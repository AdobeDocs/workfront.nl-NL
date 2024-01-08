---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Systeembeveiligingsvoorkeuren configureren
description: Als Adobe Workfront-beheerder kunt u beveiligingsvoorkeuren configureren voor uw Workfront-systeem.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '831'
ht-degree: 0%

---

# Systeemvoorkeuren configureren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Als Adobe Workfront-beheerder kunt u voorkeuren configureren voor uw Workfront-systeem:

* Toegang tot Workfront vanuit mobiele apps en andere geïntegreerde toepassingen
* Regels voor het insluiten van Workfront in een iFrame

Wijzigingen die u aanbrengt in de systeemvoorkeuren, zijn van invloed op alle gebruikers in uw systeem en op hun ervaring in Workfront.

We raden u aan uw systeemvoorkeuren tijdens de Workfront-implementatie te configureren en deze daarna slechts af en toe opnieuw te bekijken.

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

## Uw systeemvoorkeuren configureren

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Systeem** > **Voorkeuren**.

1. Selecteer een van de volgende velden om de instellingen voor uw organisatie vast te stellen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Snelle revisie inschakelen</p> </td> 
      <td>Hiermee kunt u maandelijkse Workfront-releases voor uw organisatie inschakelen in plaats van driemaandelijkse releases.</p><p>Voor meer informatie over het snelle versieproces, zie <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Snelle releases voor uw organisatie in- of uitschakelen</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Insluiten van <strong>Workfront</strong> in een iframe</p> </td> 
      <td>Hiermee kunt u Workfront insluiten in een iframe.<p>Deze optie is standaard uitgeschakeld.</p><p><b>BELANGRIJK</b>: Als u een webtoepassing weergeeft in een iframe, wordt de toepassing kwetsbaarder voor een clickjacking-beveiliging.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">SAML 2.0-verificatie toestaan in Office 365 add-ins</td> 
      <td> <p>Hiermee kunt u Workfront alleen insluiten in een iframe voor Office 365-invoegtoepassingen wanneer Workfront is geïntegreerd met een SAML 2.0-oplossing voor eenmalige aanmelding. </p> <p>Deze optie is standaard ingeschakeld.</p> <p><b>OPMERKING</b>: Als u de bovenstaande optie inschakelt, <strong>Insluiten van Workfront in een iframe toestaan</strong>, de optie <strong>SAML 2.0-verificatie toestaan in Office 365 add-ins</strong> is ingeschakeld en gedimd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Het gebruik van sessiegegevens inschakelen bij het maken van externe pagina-URL's</td> 
      <td> <p>Hiermee kunnen gebruikers de sessie-id-informatie van een site gebruiken wanneer ze een externe pagina aan een dashboard toevoegen.</p> <p>Ga voor meer informatie over het toevoegen van externe pagina's aan een dashboard naar <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Een externe webpagina insluiten in een dashboard</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Laat mensen Workfront mobiele toepassingen gebruiken en de <strong>Workfront</strong> Outlook Add-in</td> 
      <td> <p>Hiermee krijgen gebruikers toegang tot de mobiele apps (Workfront View for iPad and mobile phone apps) en de Workfront Outlook-app.</p> <p>Deze optie is standaard ingeschakeld. </p> <p>Voor informatie over de weergave van Workfront raadpleegt u <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront-weergave gebruiken</a>. Ga voor meer informatie over de mobiele apps naar <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">De mobiele Adobe Workfront-app gebruiken</a>.</p> <p>Voor meer informatie over de insteekmodule van Vooruitzichten, zie <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Adobe Workfront instellen voor Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samenwerking met personen zonder Workfront-accounts met e-mailadressen</p> </td> 
      <td>Hiermee kunnen Workfront-gebruikers bepaalde objecten delen met mensen zonder Workfront-account door hun e-mailadres in plaats van hun naam op te nemen. Gebruikers kunnen de volgende onderdelen delen met externe gebruikers door hun e-mailadres te gebruiken:
       <ul>
        <li>Document<br></li>
        <li>Documentaanvraag<br></li>
        <li>Documentgoedkeuring</li>
        <li>Kalender</li>
       </ul><p>Deze optie is standaard ingeschakeld.</p> <p><b>Belangrijk</b>: Het toegangsniveau voor externe gebruikers is niet beschikbaar in uw Workfront-instantie als deze optie is uitgeschakeld. Zie voor meer informatie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Ingebouwde toegangsniveaus</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Externe gebruikers verplichten zich met een wachtwoord te registreren</td> 
      <td> <p>Externe gebruikers moeten zich registreren voordat ze objecten in Workfront kunnen bekijken. Deze optie is standaard uitgeschakeld. Als u deze optie inschakelt, worden personen zonder Workfront-account die via hun e-mailadres in bepaalde updates zijn opgenomen, gevraagd een account te maken voordat ze het item kunnen bekijken waarop ze zijn opgenomen. Hiermee maakt u een externe gebruikersaccount voor deze gebruikers.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers automatisch afmelden na</td> 
      <td> Hier kunt u opgeven wanneer een gebruiker na een periode van inactiviteit uit Workfront wordt afgemeld. Standaard worden gebruikers afgemeld na 8 uur inactiviteit. <p>Deze optie is ook van toepassing op Workfront-klanten die één aanmeldingsoplossing gebruiken.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mobiele gebruikers automatisch afmelden na </td> 
      <td>Hier kunt u opgeven wanneer een gebruiker na een periode van inactiviteit uit de Workfront-toepassing wordt afgemeld. Gebruikers worden standaard afgemeld na 7 dagen inactiviteit. <p>Deze optie is ook van toepassing op Workfront-klanten die één aanmeldingsoplossing gebruiken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers in het systeem zien standaard de nieuwe Home-ervaring </td> 
      <td>Hier kunt u opgeven of gebruikers standaard de Nieuwe startervaring zien. Wanneer toegelaten, zullen de gebruikers de Nieuwe ervaring van het Huis door gebrek zien, maar kunnen nog verkiezen om Nieuwe Huis op individuele basis toe te laten of onbruikbaar te maken. Wanneer gehandicapt, zullen de gebruikers niet de banner zien die hen om aan Nieuw huis-nochtans toestaat over te schakelen, kunnen zij nog aan hun Nieuwe Homepage navigeren door manueel in te gaan <code>/home/workspaces</code> aan het einde van hun instantie-URL. Deze instelling is standaard ingeschakeld.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront en iedereen die met hen als externe gebruiker werkt.
