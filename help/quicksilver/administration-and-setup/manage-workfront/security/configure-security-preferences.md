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
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '894'
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
   <td><p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
      <td> <p>Hiermee krijgen gebruikers toegang tot de mobiele apps (Workfront View for iPad and mobile phone apps) en de Workfront Outlook-app.</p> <p>Deze optie is standaard ingeschakeld. </p> <p>Voor informatie over de Mening van Workfront, zie {de Mening van Adobe Workfront van 0} Gebruik <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">. </a> Voor meer informatie over mobiele apps, zie <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref"> Gebruik mobiele app van Adobe Workfront: artikelindex </a>.</p> <p>Voor meer informatie over de stop van Vooruitzichten, zie <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref"> Opstelling Adobe Workfront voor Vooruitzichten </a>.</p> </td> 
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
     <tr> 
      <td role="rowheader">Externe gebruikers verplichten zich met een wachtwoord te registreren</td> 
      <td> <p>Externe gebruikers moeten zich registreren voordat ze objecten in Workfront kunnen bekijken. Deze optie is standaard uitgeschakeld. Als u deze optie inschakelt, worden personen zonder Workfront-account die via hun e-mailadres in bepaalde updates zijn opgenomen, gevraagd een account te maken voordat ze het item kunnen bekijken waarop ze zijn opgenomen. Hiermee maakt u een externe gebruikersaccount voor deze gebruikers.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr>
<!-- DELETE THIS SECTION MARCH 2026   <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>  -->
     &lt;tr> 
     &lt;td rol= &quot;rowheader&quot;>De Hulp URL van de Douane&lt;/td> 
     &lt;td>Laat u een interne plaats van de douanehulp voor het Belangrijkste pictogram van het Menu bepalen om naar te gaan. Zie &lt;a href=&quot;/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md&quot;>Een aangepaste Help-URL configureren&lt;/a> voor meer informatie.&lt;/p>&lt;/td> 
    &lt;/tr> 
     &lt;tr> 
     &lt;td rol= &quot;rowheader&quot;>De gebruikers in het systeem zullen aan het zien van de Nieuwe ervaring van het Huis &lt;/td> 
     &lt;td>Hier specificeert u of de gebruikers de Nieuwe ervaring van het Huis door gebrek zullen zien. Wanneer toegelaten, zullen de gebruikers de Nieuwe ervaring van het Huis door gebrek zien, maar kunnen nog verkiezen om Nieuwe Huis op individuele basis toe te laten of onbruikbaar te maken. Als deze optie is uitgeschakeld, zien gebruikers niet de banner waarmee ze naar New Home kunnen schakelen. Ze kunnen echter wel naar hun nieuwe startpagina navigeren door handmatig &lt;code>/home/workspaces&lt;/code> in te voeren aan het einde van hun instantie-URL. Deze instelling is standaard ingeschakeld.&lt;/td> 
    &lt;/tr> 
     &lt;tr> 
     &lt;td rol= &quot;rowheader&quot;>laat de de werklijst van Prioriteiten &lt;/td> 
     &lt;td>Laat u verkiezen om de het werklijstervaring van Prioriteiten voor uw gebruikers toe te laten of onbruikbaar te maken. Gebruikers zien nog steeds de Prioriteitspictogrammen in Workfront, maar ze hebben geen toegang tot de functionaliteit. Zie &lt;a href=&quot;/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md&quot;>Aan de slag met prioriteiten&lt;/a> voor meer informatie over prioriteiten.&lt;/td> 
    &lt;/tr> 
     &lt;tr> 
     &lt;td rol= &quot;rowheader&quot;>De Milieu van de Test&lt;/td> 
     &lt;td>Laat u tot uw de testmilieu&#39;s van Workfront toegang hebben. Zie &lt;a href=&quot;/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md&quot;>De Adobe Workfront Preview Sandbox-omgeving&lt;/a> voor meer informatie.&lt;/p>&lt;/td>
    &lt;/tbody>
</table>

1. Klik **sparen**.

   De wijzigingen die u hier hebt opgeslagen, zijn van invloed op de ervaring van alle gebruikers in Workfront en van iedereen die als externe gebruiker met het systeem werkt.
