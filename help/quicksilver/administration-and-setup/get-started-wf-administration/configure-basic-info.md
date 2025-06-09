---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Basisinformatie voor uw systeem configureren
description: Als onderdeel van het configureren van uw Adobe Workfront-systeem kunt u gegevens over uw organisatie beheren in het gedeelte Basisinformatie van de pagina Klantgegevens.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 83d236a4d50c0eef7062f161757d2f9fe6bc4e06
workflow-type: tm+mt
source-wordcount: '829'
ht-degree: 0%

---

# Basisinformatie voor uw systeem configureren

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Als onderdeel van het configureren van uw Adobe Workfront-systeem kunt u gegevens over uw organisatie beheren in het gedeelte Basisinformatie van de pagina Klantgegevens.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   of
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

## Toegang tot klantgegevens

De klant vertegenwoordigt de Workfront-instantie voor uw organisatie. De opties op dit gebied zijn uniek voor u, als klant van Workfront.

De pagina Klantgegevens openen:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Info van de Klant**.

   Afhankelijk van het Workfront-abonnement dat u hebt aangeschaft, ontbreken sommige secties mogelijk op de pagina Klantgegevens. Neem contact op met uw accountvertegenwoordiger als u wilt weten welk Workfront-plan uw organisatie gebruikt.

   De volgende secties zijn beschikbaar in het gedeelte Klantgegevens:

   * **Basis Info**

     Voor informatie over het vormen van basisinformatie in Workfront, zie [ BasisInfo ](#configure-basic-info) vormen.

   * **API Zeer belangrijke Montages**

     Voor informatie over API zeer belangrijke montages, zie [ API sleutels beheren ](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP Lijst van gewenste personen**

     Voor informatie over het toevoegen van de IP adressen aan uw lijst van gewenste personen voor waar uw gebruikers tot Workfront kunnen toegang hebben, zie [ de lijst van gewenste personen van uw firewall ](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) vormen.

   * **Lijst van gewenste personen E-mail**

     Voor informatie over het toevoegen van e-mails aan uw lijst van gewenste personen, zie [ uw e-maillijst van gewenste personen ](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md) vormen.

   <!--
   * **License**

     For information about licenses, see [Manage available licenses in your system](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).-->

## Basisinformatie configureren {#configure-basic-info}

Binnen het gebied Basisinformatie van uw pagina van de Info van de Klant, worden sommige details over uw klant gevormd door Workfront en zij tonen op read-only wijze. Andere details kunnen door u worden gevormd. Alle opties die u in dit gebied kunt bewerken, hebben een algemeen effect op alle gebruikers in Workfront.

U kunt als volgt het gedeelte Basisinformatie in het gedeelte Klantgegevens configureren:

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Info van de Klant**.

1. In de **BasisInfo** sectie bij de bovenkant van de **Info van de Klant** pagina, vind de volgende informatie over uw instantie met Workfront:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Naam</td> 
      <td>De naam van uw organisatie, die ook de naam van uw bedrijf aanpast. Deze wordt toegevoegd door Workfront en kan niet worden bewerkt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Clusterinstelling </td> 
      <td>Het clusternummer voor uw instantie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">E-mailadres beheerder</td> 
      <td> <p>Het e-mailadres van uw Workfront-beheerder. U kunt dit veld bewerken zodat het overeenkomt met het e-mailadres van een van uw Workfront-beheerders. De gebruiker die aan dit e-mailadres is gekoppeld, wordt beschouwd als de belangrijkste Workfront-beheerder van uw Workfront-systeem. Alle communicatie van Workfront voor de hele site wordt naar dit e-mailadres gestuurd. Het is dus belangrijk dat u dit adres bijwerkt.</p> <p><b> NOTA </b>: U kunt niet, het Niveau van de Toegang van de gebruiker deactiveren schrappen of veranderen verbonden aan Admin E-mail.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domein</td> 
      <td> <p>Het domein wordt ingesteld door Workfront wanneer uw account wordt gemaakt.</p> <p>Het domein identificeert uw unieke subdomein van de URL die u gebruikt om toegang te krijgen tot Workfront.<p>Bijvoorbeeld, als uw organisatie het domein "mijnbedrijf"is toegewezen,"URL u gebruikt om tot Workfront toegang te hebben is <i> https://mycompany.my.workfront.com.</i></p><p>U kunt het domein niet zelf bewerken. Als je je domein wilt wijzigen, kun je contact opnemen met Customer Support van Workfront. Voor meer informatie over het contacteren van de Steun van de Klant van Workfront, zie <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref"> de Steun van de Klant van het Contact </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdzone</td> 
      <td> <p>Dit is de standaardtijdzone van uw Workfront-instantie. U kunt dit veld bewerken zodat het overeenkomt met de tijdzone van uw primaire Workfront-locatie. De tijdzone die u selecteert, bepaalt het volgende: </p> 
       <ul> 
        <li>De datum en tijd die in uitgaande e-mails worden weergegeven</li> 
        <li>De standaardtijdzone voor nieuwe gebruikers wanneer deze worden gemaakt</li> 
       </ul> <p>Gebruikers kunnen de tijdzone voor hun Workfront-exemplaar wijzigen onder hun profiel. Wanneer gebruikers hun tijdzone wijzigen, komen de datum en tijd in hun e-mails van Workfront overeen met hun profielvoorkeuren. Voor meer informatie over het wijzigen van de voorkeur van het gebruikersprofiel, zie <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref"> Mijn Montages </a> vormen. Het wordt geselecteerd als standaardtijdzone wanneer u een nieuw programma creeert. Voor meer informatie over het creëren van programma's, zie <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref"> een programma </a> creëren.</p> <p>Voor informatie over het gebruiken van programma's om gebruikers te helpen in Workfront over tijdstreken samenwerken, zie <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref"> Werkend over tijdstreken </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaard-e-maillandinstelling</td> 
      <td>Bepaalt de taal, datum en getalnotatie die in uitgaande e-mailberichten worden gebruikt. De hier geselecteerde landinstelling is de standaardlandinstelling wanneer nieuwe gebruikers worden gemaakt. Gebruikers kunnen hun landinstelling wijzigen in hun gebruikersprofiel. Wanneer gebruikers hun landinstelling wijzigen, komen de taal, de datum en de getalnotatie in hun e-mails van Workfront overeen met hun profielvoorkeuren. Voor meer informatie over het wijzigen van uw profielvoorkeur, zie <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref"> Mijn Montages </a> vormen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opslagquotum</td> 
      <td> <p>Dit is de hoeveelheid opslagruimte voor documenten die beschikbaar is in uw Workfront-exemplaar.<br> het quotum bevat documenten die u direct aan Workfront uploadt.<br> het omvat niet:</p> 
       <ul> 
        <li>Documenten die u via een andere externe serviceprovider (SharePoint, Google Drive, Webdam, Box, Dropbox, een andere leverancier van Document Asset Management) aan Workfront koppelt.</li> 
        <li>Uw Workfront-gegevens (projecten, taken, problemen, gebruikers, enzovoort).</li> 
       </ul> </td> 
     </tr>
    </tbody> 
   </table>

1. Klik **sparen**.
