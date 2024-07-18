---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront configureren met SAML 2.0
description: Als beheerder van Adobe Workfront, kunt u het Web van Workfront en mobiele toepassingen vormen om met een oplossing van de Prijsverhoging van de Veiligheid (SAML) 2.0 voor enig teken-binnen (SSO) te integreren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1011'
ht-degree: 0%

---

# Adobe Workfront configureren met SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u het Web van Workfront en mobiele toepassingen vormen om met een oplossing van de Prijsverhoging van de Veiligheid (SAML) 2.0 voor enig teken-binnen (SSO) te integreren.

Nadat u SAML 2.0 in Workfront hebt gevormd, zoals die in de volgende secties wordt beschreven, kunt u de configuratie handhaven, zoals die in [ wordt beschreven Update SAML 2.0 meta-gegevens in uw identiteitsleverancier ](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td><p>Nieuw: Standaard </p>
       <p>of</p> 
       <p>Huidig: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verificatie inschakelen voor Workfront met SAML 2.0

{{step-1-to-setup}}

1. Klik **Systeem** > **Enige Sign-On (SSO).**

1. In de **drop-down lijst van het Type**, uitgezochte **SAML 2.0.**

1. Dichtbij de bovenkant van de opties die verschijnen, klik **de Metagegevens van SAML 2.0 van de Download** om het dossier op uw computer te downloaden.

   Uw SAML 2.0-identiteitsprovider vereist een XML-bestand met informatie die in uw Workfront-instantie is gegenereerd. Nadat u het bestand hebt gedownload, hebt u toegang tot uw SAML 2.0 Identity Provider-server en moet u het XML-bestand met Workfront SAML 2.0-metagegevens daar uploaden.

1. Geef de volgende informatie op in Workfront:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Service Provider-id </td>
      <td> Deze URL, die al voor u is ingevuld, identificeert Workfront aan uw identiteitsprovider. Bijvoorbeeld: <code>&lt;yourcompany&gt;.com/SAML2</code> .</td>
     </tr>
     <tr>
      <td role="rowheader">Type binding </span> </td>
      <td> <p>Selecteer de methode die door uw IDP-server wordt ondersteund voor het verzenden van verificatiegegevens:</p>
       <ul>
       <li>POST</li>
       <li>OMLEIDING</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Velden vullen met metagegevens van identiteitsprovider </td> 
      <td>Exporteer in uw SAML 2.0 Identity Provider-oplossing een XML-bestand met metagegevens van een Service Provider en sla dit op een tijdelijke locatie op uw computer op. Selecteer <strong> kiezen Dossier </strong>, dan vinden en selecteren het dossier u bewaarde om het aan uw configuratie van Workfront toe te voegen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Aanmeldingsportal-URL </span> </td> 
      <td>Voer de gemeenschappelijke aanmeldingsportaal van uw organisatie in. Dit is URL waar de gebruikers login om tot Workfront en alle andere toepassingen toegang te hebben die met SAML 2.0 worden geïntegreerd.</td> 
     </tr>
     <tr>
      <td role="rowheader">Afmeldings-URL </span> </td> 
      <td> <p>Voer de aanmeldings-URL voor de IDP-server in. Workfront verzendt een HTTP-aanvraag naar deze URL voordat het zich afmeldt bij Workfront. Hiermee wordt de sessie van de gebruiker op de externe server gesloten wanneer de Workfront-sessie wordt gesloten.</p> <p><b> NOTA </b>: U wordt opnieuw gericht aan sign-out URL slechts als u de optie <strong> hebt slechts SAML 2.0 Authentificatie </strong> toelaat die in uw gebruikersprofiel wordt toegelaten.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Wachtwoord-URL wijzigen </td> 
      <td> <p> Geef de URL op waar gebruikers hun wachtwoorden moeten wijzigen. </p> <p>Omdat de SAML 2.0 geloofsbrieven worden gebruikt om tot Workfront toegang te hebben, moeten de gebruikers aan een pagina worden opnieuw gericht waar zij hun wachtwoord van SAML 2.0 kunnen veranderen in plaats van deze activiteit door Workfront te voltooien.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beveiligd hash-algoritme </td> 
      <td> <p>Selecteer het Veilige Algorithm (SHA) dat uw IDP ondersteunt:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gebruikers voor automatische voorzieningen </span> </td> 
      <td> <p>Met deze optie wordt automatisch een gebruiker in het systeem gemaakt wanneer een nieuwe gebruiker met een gebruikersnaam en wachtwoord voor de directory zich voor het eerst bij Workfront aanmeldt.</p> <p>Als u gebruikers in Workfront wilt maken, moet u Workfront-gegevenskenmerken toewijzen aan de volgende gebruikersgegevenskenmerken in uw mappenprovider:</p> 
       <ul> 
       <li>Voornaam</li> 
       <li>Achternaam</li> 
       <li>E-mailadres</li> 
       </ul> 
       <p>Als u het selectievakje inschakelt, worden de volgende opties weergegeven:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selecteer het Workfront-gebruikerskenmerk dat u wilt toewijzen in de vervolgkeuzelijst en geef vervolgens het bijbehorende Directory-kenmerk op in de gebruikersmap.</p> 
       <p>Het <strong> gebied van het Attribuut van de Folder </strong> zou de Naam van het Attribuut van de Folder van de lijst van het Attribuut van de Gebruiker moeten bevatten u wanneer met succes het testen van uw configuratie SAML 2.0 bewaarde.</p> 
       <p>U kunt een StandaardWaarde van Workfront op het <strong> Standaardgebied van de Waarde </strong> plaatsen. U kunt regels ook instellen op basis van de waarden van uw SAML 2.0-identiteitsprovider.</p> 
       <p><b> WAARSCHUWING </b>: Workfront probeert om de hieronder vermelde attributen in kaart te brengen telkens als een gebruiker zich in het systeem aanmeldt. Wegens dit, adviseren wij kaarttoegangsniveaus niet. U kunt beheertoegang eenvoudig verwijderen als een kenmerk onjuist is toegewezen. Klik <strong> Toewijzing </strong> toevoegen om extra regels toe te voegen.
       </p> 
       <p>U kunt de volgende Workfront-kenmerken toewijzen:</p> 
      <ul> 
      <li> <p>Toegangsniveau</p> </li> 
      <li> <p>Adres</p> </li> 
      <li> <p>Adres2</p> </li> 
      <li> <p>Facturering per uur</p> </li> 
      <li> <p>Plaats</p> </li> 
      <li> <p>Bedrijf</p> </li> 
      <li> <p>Kosten per uur</p> </li> 
      <li> <p>E-mailadres</p> </li> 
      <li> <p>Extensie</p> </li> 
      <li> <p>Voornaam</p> </li> 
      <li> <p>Thuisgroep</p> </li> 
      <li> <p>Thuisteam</p> </li> 
      <li> <p>Functie</p> </li> 
      <li> <p>Achternaam</p> </li> 
      <li> <p>Lay-outsjabloon</p> </li> 
      <li> <p>Manager</p> </li> 
      <li> <p>Mobiele telefoon</p> </li> 
      <li> <p>Telefoonnummer</p> </li> 
      <li> <p>Postcode</p> </li> 
      <li> <p>Schema</p> </li> 
      <li> <p>Staat</p> </li> 
      <li> <p>Tijdbladprofiel</p> </li> 
      <li> <p>Titel</p> </li> 
      </ul>
      <p>Klik <strong> sparen </strong> wanneer u voltooide attributen van de kaartgebruiker bent.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificaat </td> 
      <td> <p>Upload een geldig SSL-certificaat voor een veilige verbinding tussen de verificatieservice en Workfront. Voor OnDemand-accounts is altijd een certificaat vereist. U kunt dit certificaat verkrijgen van uw SAML 2.0 systeembeheerder.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Admin-vrijstelling </td> 
      <td> <p>Hiermee krijgen Workfront-beheerders toegang tot Workfront via hun Workfront-aanmelding. Als deze optie niet is geselecteerd, moeten Workfront-beheerders hun SAML 2.0-gebruikersnaam en -wachtwoord gebruiken.</p> 
      <p>Workfront probeert zich eerst via SAML 2.0 aan te melden bij Workfront voor gebruikers met het toegangsniveau van Workfront System Administrator. Als de SAML 2.0-verificatie mislukt, gebruikt Workfront lokale verificatie voor Workfront-beheerders.</p> 
      <p>We raden u aan deze optie altijd in te schakelen, zodat uw Workfront-beheerder zich kan aanmelden bij Workfront als uw SAML 2.0-provider ooit tijdelijk niet beschikbaar is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inschakelen </td> 
      <td> <p>Activeert SSO op het systeem van Workfront. Zorg ervoor dat u aanmeldingsinstructies aan uw gebruikers hebt doorgegeven.</p> <p>Nadat u uw configuratie SSO in Workfront toelaat, moet u <strong> toelaten slechts SAML 2.0 Authentificatie </strong> die voor alle gebruikers plaatst zodat zij SSO kunnen gebruiken.</p> <p>Voor meer informatie over het bijwerken van gebruikers voor SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref"> de gebruikers van de Update voor enig teken-op </a>.</p> <p>Voor meer informatie over gebruikersmontages, zie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref"> het profiel van een gebruiker </a> uitgeven.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuratie bevestigen </td> 
      <td> 
      <p>Klik <strong> Verbinding van de Test </strong> om te verifiëren dat Workfront en SAML 2.0 de Leverancier van de Identiteit met elkaar kunnen communiceren. Deze verbinding is alleen gelukt als u de XML-bestanden hebt uitgewisseld.
      </p> 
      <p>Nadat u de koppeling tussen uw SAML 2.0-identiteitsprovider en Workfront hebt getest, wordt een scherm weergegeven dat lijkt op de onderstaande afbeelding.</p>
      <p><b> NOTA </b>: Dit scherm wordt getoond in browser pop-up, zodat zorg ervoor dat u pop-up blockers in uw browser onbruikbaar maakt.</p>
      <p>Sla de informatie op die in de tabel wordt weergegeven, zodat u deze later kunt gebruiken.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klik **sparen** om SAML 2.0 configuratie te bewaren.
