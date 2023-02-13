---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront configureren met SAML 2.0
description: Als beheerder van Adobe Workfront, kunt u het Web van Workfront en mobiele toepassingen vormen om met een oplossing van de Prijsverhoging van de Veiligheid (SAML) 2.0 voor enig teken-binnen (SSO) te integreren.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 0%

---

# Adobe Workfront configureren met SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u het Web van Workfront en mobiele toepassingen vormen om met een oplossing van de Prijsverhoging van de Veiligheid (SAML) 2.0 voor enig teken-binnen (SSO) te integreren.

Nadat u SAML 2.0 in Workfront hebt gevormd, zoals die in de volgende secties wordt beschreven, kunt u de configuratie handhaven, zoals die in wordt beschreven [SAML 2.0-metagegevens bijwerken in uw identiteitsprovider](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

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
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Verificatie inschakelen voor Workfront met SAML 2.0

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Single Sign-On (SSO).**

1. In de **Type** vervolgkeuzelijst, klikt u op **SAML 2.0**

1. Klik boven aan de opties die worden weergegeven op **SAML 2.0-metagegevens downloaden** om het bestand op uw computer te downloaden.

   Uw SAML 2.0-identiteitsprovider vereist een XML-bestand met informatie die in uw Workfront-instantie is gegenereerd. Nadat het bestand is gedownload, moet u naar de SAML 2.0 Identity Provider-server gaan en daar het XML-bestand met Workfront SAML 2.0-metagegevens uploaden.

1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Service Provider-id </td> 
      <td> Deze URL, die al voor u is ingevuld, identificeert Workfront aan uw identiteitsprovider. Bijvoorbeeld: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Type binding</span> </td> 
      <td> <p>Selecteer de methode die door uw IDP-server wordt ondersteund voor het verzenden van verificatiegegevens:</p> 
       <ul> 
        <li>POST</li> 
        <li>OMLEIDING</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Velden vullen met metagegevens van identiteitsprovider </td> 
      <td>Exporteer in uw SAML 2.0 Identity Provider-oplossing een XML-bestand met metagegevens van een Service Provider en sla dit op een tijdelijke locatie op uw computer op. Selecteren <strong>Bestand kiezen</strong>, zoekt en selecteert u het bestand dat u hebt opgeslagen om het toe te voegen aan uw Workfront-configuratie.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL aanmeldingsportaal</span> </td> 
      <td>Geef de gemeenschappelijke aanmeldingsportaal van uw organisatie op. Dit is URL waar de gebruikers login om tot Workfront en alle andere toepassingen toegang te hebben die met SAML 2.0 worden geïntegreerd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Afmeldings-URL</span> </td> 
      <td> <p>Geef de aanmeldings-URL voor de IDP-server op. Workfront verzendt een HTTP-aanvraag naar deze URL voordat het zich afmeldt bij Workfront. Hiermee wordt de sessie van de gebruiker op de externe server gesloten wanneer de Workfront-sessie wordt gesloten.</p> <p><b>OPMERKING</b>: U wordt alleen omgeleid naar de aanmeldings-URL als u de optie Alleen SAML 2.0-verificatie toestaan hebt ingeschakeld in uw gebruikersprofiel.</p> </td> 
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
      <td role="rowheader">Gebruikers voor automatische voorzieningen</span> </td> 
      <td> <p>Er wordt automatisch een gebruiker in het systeem gemaakt wanneer een nieuwe gebruiker met een gebruikersnaam en wachtwoord voor de directory zich voor het eerst bij Workfront aanmeldt.</p> <p>Als u gebruikers in Workfront wilt maken, moet u Workfront-gegevenskenmerken toewijzen aan de volgende gebruikersgegevenskenmerken in uw directoryprovider:</p> 
       <ul> 
        <li>Voornaam</li> 
        <li>Achternaam</li> 
        <li>E-mailadres</li> 
       </ul> 
       <p>U kunt dit doen met de volgende opties:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selecteer het Workfront-gebruikerskenmerk dat u wilt toewijzen in de vervolgkeuzelijst en geef vervolgens het bijbehorende Directory-kenmerk op in de gebruikersmap.</p> 
       <p>De <strong>Directory-kenmerk</strong> het gebied zou de Naam van het Attribuut van de Folder van de lijst van het Attribuut van de Gebruiker moeten bevatten u wanneer met succes het testen van uw configuratie SAML 2.0 bewaarde.</p> 
       <p>U kunt een standaard Workfront-waarde instellen in het dialoogvenster <strong>Standaardwaarde</strong> veld. U kunt regels ook instellen op basis van de waarden van uw SAML 2.0-identiteitsprovider.</p> 
       <p><b>WAARSCHUWING</b>: Workfront probeert de hieronder vermelde kenmerken elke keer dat een gebruiker zich bij het systeem aanmeldt, toe te wijzen. Wegens dit, adviseren wij kaarttoegangsniveaus niet. U kunt beheertoegang eenvoudig verwijderen als een kenmerk onjuist is toegewezen. Klik op Toewijzing toevoegen om extra regels toe te voegen.
       </p> 
       <p>U kunt de volgende Workfront-kenmerken toewijzen:</p> 
      <ul> 
      <li> <p>Toegangsniveau</p> </li> 
      <li> <p>Adres</p> </li> 
      <li> <p>Address2</p> </li> 
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
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>Klikken <strong>Opslaan</strong> wanneer u klaar bent met het toewijzen van gebruikerskenmerken.</p> </td> 
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
      <td> <p>Activeert SSO op het systeem van Workfront. Zorg ervoor dat u aanmeldingsinstructies aan uw gebruikers hebt doorgegeven.</p> <p>Nadat u de SSO-configuratie in Workfront hebt ingeschakeld, moet u de <strong>Alleen SAML 2.0-verificatie toestaan</strong> het plaatsen voor alle gebruikers zodat zij SSO kunnen gebruiken.</p> <p>Voor meer informatie over het bijwerken van gebruikers voor SSO, zie <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Gebruikers bijwerken voor eenmalige aanmelding</a>.</p> <p>Voor meer informatie over gebruikersinstellingen raadpleegt u <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Gebruikersprofiel bewerken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Configuratie bevestigen </td> 
      <td> 
      <p>Klikken <strong>Verbinding testen</strong> om te controleren of Workfront en SAML 2.0 Identity Provider met elkaar kunnen communiceren. Deze verbinding is alleen gelukt als u de XML-bestanden hebt uitgewisseld.
      </p> 
      <p>Nadat u de koppeling tussen uw SAML 2.0-identiteitsprovider en Workfront hebt getest, ziet u een scherm dat lijkt op het onderstaande scherm.</p>
      <p><b>OPMERKING</b>: Dit scherm wordt weergegeven in een pop-upbrowser, zodat u de optie voor het blokkeren van pop-ups in uw browser uitschakelt.</p>
      <p>Sla de informatie op die in de tabel wordt weergegeven, zodat u deze later kunt gebruiken.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan** om de SAML 2.0-configuratie op te slaan.
