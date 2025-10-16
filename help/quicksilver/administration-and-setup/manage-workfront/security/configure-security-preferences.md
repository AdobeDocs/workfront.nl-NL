---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Systeemvoorkeuren configureren
description: Als Adobe Workfront-beheerder kunt u voorkeuren configureren voor uw Workfront-systeem, inclusief beveiligingsvoorkeuren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 1a56846647e443cf3f5f09eed8c3084434de5ddb
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Systeemvoorkeuren configureren

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

{{important-admin-console-onboard}}

Als Adobe Workfront-beheerder kunt u voorkeuren configureren voor uw Workfront-systeem, zoals:

* Toegang tot Workfront vanuit mobiele apps en andere geïntegreerde toepassingen
* Regels voor het insluiten van Workfront in een iFrame

Wijzigingen die u aanbrengt in de systeemvoorkeuren, zijn van invloed op alle gebruikers in uw systeem en op hun ervaring in Workfront.

We raden u aan uw systeemvoorkeuren tijdens de Workfront-implementatie te configureren en deze daarna slechts af en toe opnieuw te bekijken.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uw systeemvoorkeuren configureren

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Voorkeur**.

1. Selecteer een van de volgende velden om de instellingen voor uw organisatie vast te stellen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Snelle release inschakelen</p> </td> 
      <td>Hiermee kunt u maandelijkse Workfront-releases voor uw organisatie inschakelen in plaats van driemaandelijkse releases.</p><p>Voor meer informatie over het snelle versieproces, zie <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref"> snelle versies voor uw organisatie </a> toelaten of onbruikbaar maken.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Insluiten van Workfront in een iframe toestaan</p> </td> 
      <td>Hiermee kunt u Workfront insluiten in een iframe.<p>Deze optie is standaard uitgeschakeld.</p><p><b> BELANGRIJK </b>: Het tonen van een web-based toepassing in een iframe maakt de toepassing vatbaar voor een klik-jacking veiligheidskwetsbaarheid.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">SAML 2.0-verificatie toestaan in Office 365 add-ins</td> 
      <td> <p>Hiermee kunt u Workfront alleen insluiten in een iframe voor Office 365-invoegtoepassingen wanneer Workfront is geïntegreerd met een SAML 2.0-oplossing voor eenmalige aanmelding. </p> <p>Deze optie is standaard ingeschakeld.</p> <p><b> NOTA </b>: Als u de optie hierboven toelaat, <strong> het inbedden van Workfront in een iframe </strong> toestaan, staat de optie <strong> SAML 2.0 authentificatie in Bureau 365 toe:voegen-ins </strong> toe toegelaten en wordt gedimd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Het gebruik van sessiegegevens inschakelen bij het maken van externe pagina-URL's</td> 
      <td> <p>Hiermee kunnen gebruikers de sessie-id-informatie van een site gebruiken wanneer ze een externe pagina aan een dashboard toevoegen.</p> <p>Deze optie is standaard onveilig en uitgeschakeld. Aanbevolen wordt OAuth voor integratie te gebruiken.</p> <p>Voor meer informatie over het toevoegen van Externe Pagina's aan een Dashboard, zie <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref"> een externe Web-pagina in een dashboard </a> inbedden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers met mobiele Workfront-toepassingen en de Workfront Outlook Add-in toestaan</td> 
      <td> <p>Hiermee krijgen gebruikers toegang tot de mobiele apps (Workfront View for iPad and mobile phone apps) en de Workfront Outlook-app.</p> <p>Deze optie is standaard ingeschakeld. </p> <p>Voor informatie over de Mening van Workfront, zie {de Mening van Adobe Workfront van 0} Gebruik <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">. </a> Voor meer informatie over mobiele apps, zie <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref"> Gebruik mobiele app van Adobe Workfront: artikelindex </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Samenwerking met personen zonder Workfront-accounts met e-mailadressen</p> </td> 
      <td>Hiermee kunnen Workfront-gebruikers bepaalde objecten delen met mensen zonder Workfront-account door hun e-mailadres in plaats van hun naam op te nemen. Gebruikers kunnen de volgende onderdelen delen met externe gebruikers door hun e-mailadres te gebruiken:
       <ul>
        <li>Document<br></li>
        <li>Documentaanvraag<br></li>
        <li>Documentgoedkeuring</li>
        <li>Kalender</li>
       </ul><p>Deze optie is standaard ingeschakeld.</p> <p><b> Belangrijk </b>: Het Externe niveau van de gebruikerstoegang is niet beschikbaar in uw instantie van Workfront als deze optie gehandicapt is. Voor meer informatie, zie <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref"> Ingebouwde toegangsniveaus </a>.</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">Aangepaste Help-URL</td> 
      <td>Hiermee kunt u een interne aangepaste Help-site definiëren waarnaar het hulppictogram voor het hoofdmenu moet gaan. Voor meer informatie, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md"> een douanehulp URL </a> vormen.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">De werklijst Prioriteiten inschakelen </td> 
      <td>Hiermee kunt u ervoor kiezen om de werklijstervaring Prioriteiten in of uit te schakelen voor uw gebruikers. Gebruikers zien nog steeds de Prioriteitspictogrammen in Workfront, maar ze hebben geen toegang tot de functionaliteit. Voor meer informatie over Prioriteiten, zie <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md"> begonnen worden met Prioriteiten </a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">AI inschakelen </td> 
      <td>Hiermee kunt u AI inschakelen, inclusief AI Assistant. <p><b> Nota </b>: Uw organisatie moet aan specifieke vereisten voldoen om AI toe te laten. Voor meer informatie over AI, met inbegrip van de vereisten, zie <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md"> AI Hulpoverzicht </a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Formulier automatisch aanvullen </td> 
      <td>Hiermee kunt u de mogelijkheid inschakelen om aanvraagformulieren automatisch in te vullen op basis van eerdere aanvraaggegevens. Voor meer informatie over Auto-Volledige Vorm, zie <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md"> auto-Vul een verzoek van vorige gegevens </a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Aanmelden bij AI Betas </td> 
      <td>&gt;Hiermee kunt u AI-functies inschakelen die momenteel in Beta zijn geïnstalleerd. Als u deze optie inschakelt, kunt u selecteren welke AI Beta-functies u wilt inschakelen. Voor meer informatie over elke AI Beta-functie klikt u op het informatiepictogram naast die functie.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Testomgevingen</td> 
      <td>Hiermee hebt u toegang tot uw Workfront-testomgevingen. Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md"> het Milieu van Sandbox van de Voorproef van Adobe Workfront </a>.</p></td> 
    </tbody> 
   </table>

1. Klik **sparen**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront en van iedereen die als externe gebruiker met het systeem werkt.
