---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Basisinformatie voor uw systeem configureren
description: Als onderdeel van het configureren van uw Adobe Workfront-systeem kunt u gegevens over uw organisatie beheren in het gedeelte Basisinformatie van de pagina Klantgegevens.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Basisinformatie voor uw systeem configureren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Als onderdeel van het configureren van uw Adobe Workfront-systeem kunt u gegevens over uw organisatie beheren in het gedeelte Basisinformatie van de pagina Klantgegevens.

## Toegangsvereisten

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn. Zie voor meer informatie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Toegang tot klantgegevens

De klant vertegenwoordigt de Workfront-instantie voor uw organisatie. De opties op dit gebied zijn uniek voor u, als klant van Workfront.

De pagina Klantgegevens openen:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Systeem** > **Klantgegevens**.

   Afhankelijk van het Workfront-abonnement dat u hebt aangeschaft, ontbreken sommige secties mogelijk op de pagina Klantgegevens. Neem contact op met uw accountvertegenwoordiger als u wilt weten welk Workfront-plan uw organisatie gebruikt.

   De volgende secties zijn beschikbaar in het gedeelte Klantgegevens:

   * **Basisinformatie**

      Voor informatie over het configureren van basisinformatie in Workfront raadpleegt u [Basisinformatie configureren](#configure-basic-info).

   * **Instellingen API-sleutel**

      Voor informatie over API-sleutelinstellingen raadpleegt u [API-sleutels beheren](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP Lijst van gewenste personen**

      Voor informatie over het toevoegen van de IP adressen aan uw lijst van gewenste personen voor waar uw gebruikers tot Workfront kunnen toegang hebben, zie [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **Licentie**

      Voor informatie over licenties raadpleegt u [Beschikbare licenties in uw systeem beheren](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## Basisinformatie configureren {#configure-basic-info}

Binnen het gebied Basisinformatie van uw pagina van de Info van de Klant, worden sommige details over uw klant gevormd door Workfront en zij tonen op read-only wijze. Andere details kunnen door u worden gevormd. Alle opties die u in dit gebied kunt bewerken, hebben een algemeen effect op alle gebruikers in Workfront.

U kunt als volgt het gedeelte Basisinformatie in het gedeelte Klantgegevens configureren:

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Systeem** > **Klantgegevens**.

1. In de **Basisinformatie** aan de bovenkant van **Klantgegevens** op Workfront de volgende informatie over je exemplaar vindt:

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
      <td> <p>Het e-mailadres van uw Workfront-beheerder. U kunt dit veld bewerken zodat het overeenkomt met het e-mailadres van een van uw Workfront-beheerders. De gebruiker die aan dit e-mailadres is gekoppeld, wordt beschouwd als de belangrijkste Workfront-beheerder van uw Workfront-systeem. Alle communicatie van Workfront voor de hele site wordt naar dit e-mailadres gestuurd. Het is dus belangrijk dat u dit adres bijwerkt.</p> <p><b>OPMERKING</b>: U kunt het toegangsniveau van de gebruiker die aan de beheermail is gekoppeld, niet deactiveren, verwijderen of wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Domein</td> 
      <td> <p>Het domein wordt ingesteld door Workfront wanneer uw account wordt gemaakt.</p> <p>Het domein identificeert uw unieke subdomein van de URL die u gebruikt om toegang te krijgen tot Workfront.<p>Als aan uw organisatie bijvoorbeeld het domein 'mijnbedrijf' is toegewezen, is de URL die u gebruikt om toegang te krijgen tot Workfront <i>https://mycompany.my.workfront.com.</i></p><p>U kunt het domein niet zelf bewerken. Als je je domein wilt wijzigen, kun je contact opnemen met Customer Support van Workfront. Ga voor meer informatie over het contact opnemen met de klantenondersteuning van Workfront naar <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact opnemen met Klantenondersteuning</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tijdzone</td> 
      <td> <p>Dit is de standaardtijdzone van uw Workfront-instantie. U kunt dit veld bewerken zodat het overeenkomt met de tijdzone van uw primaire Workfront-locatie. De tijdzone die u selecteert, bepaalt het volgende: </p> 
       <ul> 
        <li>De datum en tijd die in uitgaande e-mails worden weergegeven</li> 
        <li>De standaardtijdzone voor nieuwe gebruikers wanneer deze worden gemaakt</li> 
       </ul> <p>Gebruikers kunnen de tijdzone voor hun Workfront-exemplaar wijzigen onder hun profiel. Wanneer gebruikers hun tijdzone wijzigen, komen de datum en tijd in hun e-mails van Workfront overeen met hun profielvoorkeuren. Zie voor meer informatie over het wijzigen van voorkeuren voor gebruikersprofielen <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Mijn instellingen configureren</a>. Het wordt geselecteerd als standaardtijdzone wanneer u een nieuw programma creeert. Voor meer informatie over het creëren van programma's, zie <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Een schema maken</a>.</p> <p>Voor informatie over het gebruiken van programma's om gebruikers te helpen in Workfront over tijdstreken samenwerken, zie <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">Werken in tijdzones</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Landinstelling</td> 
      <td>Bepaalt de taal, datum en getalnotatie die in uitgaande e-mailberichten worden gebruikt. De hier geselecteerde landinstelling is de standaardlandinstelling wanneer nieuwe gebruikers worden gemaakt. Gebruikers kunnen hun landinstelling wijzigen in hun gebruikersprofiel. Wanneer gebruikers hun landinstelling wijzigen, komen de taal, de datum en de getalnotatie in hun e-mails van Workfront overeen met hun profielvoorkeuren. Ga voor meer informatie over het wijzigen van uw profielvoorkeuren naar <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Mijn instellingen configureren</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opslagquotum</td> 
      <td> <p>Dit is de hoeveelheid opslagruimte voor documenten die beschikbaar is in uw Workfront-exemplaar.<br>De quota bevat documenten die u rechtstreeks uploadt naar Workfront.<br>Hieronder vallen niet:</p> 
       <ul> 
        <li>Documenten die u via een andere externe serviceprovider (SharePoint, Google Drive, Webdam, Box, Dropbox, een andere leverancier van Document Asset Management) aan Workfront koppelt.</li> 
        <li>Uw Workfront-gegevens (projecten, taken, problemen, gebruikers, enzovoort).</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Productversie</td> 
      <td>Dit is het type Workfront-instantie dat aan u is toegewezen. De productversie voor de meeste Workfront-klanten is <strong>Enterprise</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.
