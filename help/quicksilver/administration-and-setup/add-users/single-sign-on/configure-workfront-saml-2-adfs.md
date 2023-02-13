---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront configureren met SAML 2.0 met behulp van ADFS
description: U kunt verificatie inschakelen voor Workfront met SAML 2.0.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Adobe Workfront configureren met SAML 2.0 met behulp van ADFS

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u Workfront met een oplossing van de Prijsverhoging van de Veiligheid van de Taal (SAML) 2.0 voor enig teken-op integreren terwijl het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS).

Deze handleiding is gericht op het instellen van ADFS zonder automatische provisioning of kenmerktoewijzingen. We raden u aan de installatie te voltooien en deze te testen voordat u automatische provisioning instelt.

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

Voer de volgende secties in om verificatie in te schakelen voor de Workfront-webtoepassing en de mobiele Workfront-toepassing met SAML 2.0:

* [Het Workfront SSO-metagegevensbestand ophalen](#retrieve-the-workfront-sso-metadata-file)
* [Reliëfpartijtrusts configureren](#configure-relying-party-trusts)
* [Claimregels configureren](#configure-claim-rules)
* [Upload het metagegevensbestand en test de verbinding](#upload-the-metadata-file-and-test-the-connection)

### Het Workfront SSO-metagegevensbestand ophalen {#retrieve-the-workfront-sso-metadata-file}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).
1. Klik in het linkerdeelvenster op **Systeem** > **Single Sign-On (SSO)**.
1. In de **Type** vervolgkeuzelijst, klikt u op **SAML 2.0** om aanvullende informatie en opties weer te geven.
1. Kopieer de URL die wordt weergegeven na **URL metagegevens**.
1. Ga verder met het volgende gedeelte. [Reliëfpartijtrusts configureren](#configure-relying-party-trusts).

### Reliëfpartijtrusts configureren {#configure-relying-party-trusts}

1. Open de **ADFS Manager** het gebruiken van de server van Vensters 2008 R2 (versie kan variëren).
1. Ga naar **Start.**
1. Klikken **Beheertools.**
1. Klikken **ADFS 2.0 Management.**
1. Selecteren **ADFS** en uitbreiden **Betrouwbaarheidsrelaties**.
1. Klikken met rechtermuisknop **Vertrouwden op een partij** selecteert u vervolgens **Betrouwbaarheid van derden toevoegen** om de Add Relying Party Trust Wizard te starten.
1. Van de **Welkomstpagina**, selecteert u **Start**.
1. In de **Datumbron selecteren** plakken, plakt u de URL van de metagegevens vanuit Workfront.
1. Klikken **Volgende**.
1. Klikken **OK** om het waarschuwingsbericht te bevestigen.
1. In de **Weergavenaam opgeven** een sectie toevoegen **Weergavenaam** en **Notities** om het vertrouwen te onderscheiden, klikt u vervolgens op **Volgende**.
1. Selecteren **Alle gebruikers toegang geven tot deze betrouwbare partij** (of **Geen** als u dit later wilt vormen).
1. Klikken **Volgende**.

   Hiermee gaat u naar de **Gereed om vertrouwen toe te voegen** sectie.

1. Doorgaan naar de volgende sectie [Claimregels configureren](#configure-claim-rules).

### Claimregels configureren {#configure-claim-rules}

1. Klikken **Volgende** in de **Gereed om vertrouwen toe te voegen** en zorgt u ervoor dat de **Dialoogvenster Regels voor claim bewerken openen** is geselecteerd.

   Op deze manier kunt u de regels voor claims in een volgende stap bewerken.

1. Klikken **Sluiten**.
1. Klikken **Regel toevoegen.**
1. Selecteren **LDAP-kenmerk verzenden als claims**.
1. Klikken **Volgende** om de **Claimregel configureren** stap.
1. Specificeer de volgende minimumvereisten om de claimregel te vormen: (Dit gaat over de **Federatie-id** op de gebruikersinstelling en wordt gebruikt om te onderscheiden wie zich aanmeldt.)


   <table >                
      <tbody>
            <tr>
               <td>Naam van claimregel
               </td>
               <td>Geef een naam op voor de claimregel. Bijvoorbeeld "Workfront."</td>
            </tr>
            <tr>
               <td>Kenmerkarchief</td>
               <td >Selecteren <b>Active Directory</b> in het keuzemenu.</td>
            </tr>
            <tr>
               <td>LDAP-kenmerk</td>
               <td>Dit kan elk type kenmerk zijn. We raden u aan <b>SAM-accountnaam</b> voor dit kenmerk.</td>
            </tr>
            <tr>
               <td>Type uitgaande vordering</td>
               <td>U moet <b>Naam-id</b> als het type uitgaande vordering</td>
            </tr>
      </tbody>
   </table>

1. (Optioneel) Als u automatische provisioning wilt instellen, voegt u de volgende aanvullende claims toe in zowel het LDAP-kenmerk als het type uitgaande claim:

   * Voornaam
   * Achternaam
   * E-mailadres

1. Klikken **Voltooien** en klik vervolgens op **OK** op het volgende scherm.
1. Klik met de rechtermuisknop op de nieuwe **Betrouwbaarheid partij** selecteert u vervolgens **Eigenschappen**.
1. Selecteer **Geavanceerde tab**. en onder **Beveiligd hash-algoritme** Selecteer SHA-1 of SHA-256.

   >[!NOTE]
   >
   >De optie die u onder Veilig algoritme van de Hash selecteert moet het Veilige gebied van het Algoritme van de Hash in Workfront onder Opstelling > Systeem > Enige Sign-ON (SSO) aanpassen.

1. Doorgaan naar de volgende sectie [Upload het metagegevensbestand en test de verbinding](#upload-the-metadata-file-and-test-the-connection).

### Upload het metagegevensbestand en test de verbinding {#upload-the-metadata-file-and-test-the-connection}

1. Een browser openen en naar `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Hiermee moet u het bestand FederationMetadata.xml van een metagegevensbestand downloaden.

1. Klikken **Bestand kiezen** krachtens **Velden vullen met metagegevens van identiteitsprovider** en selecteert u de **FederationMetadata.xml** bestand.

1. (Optioneel) Als de certificaatinformatie niet met het metagegevensbestand is gevuld, kunt u een bestand afzonderlijk uploaden. Selecteren **Bestand kiezen** in de **Certificaat** sectie.

1. Klikken **Verbinding testen**. Indien correct ingesteld, ziet u een pagina die vergelijkbaar is met de hieronder weergegeven pagina:

   ![](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Als u aan de afbeelding van opstellingsattributen wilt, zorg ervoor dat u de attributen van de Verbinding van de Test in het Attribuut van de Folder kopieert. Zie Toewijzing van gebruikerskenmerken voor meer informatie.

1. Selecteren **Admin-vrijstelling** om Workfront-beheerders toe te staan zich aan te melden met Workfront-referenties met de bypass-URL.

   Bladwijzers naar `<yourdomain>`.my.workfront.com/login.

1. Selecteer **Inschakelen** om de configuratie in te schakelen.
1. Klikken **Opslaan**.

## Gebruikers voor SSO bijwerken

In het kader van deze handleiding **SSO-gebruikersnaam** zullen **Active Directory-gebruikersnaam**.

Als Workfront-beheerder kunt u updategebruikers bulksgewijs verzenden naar SSO. Voor meer informatie over het bijwerken van gebruikers voor SSO, zie [Gebruikers bijwerken voor eenmalige aanmelding](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Als Workfront-beheerder kunt u ook handmatig een federatie-id toewijzen die het profiel van de gebruiker bewerkt en het veld Federation ID invult. Voor meer informatie over het bewerken van een gebruiker raadpleegt u [Gebruikersprofiel bewerken](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

>[!NOTE]
>
>Als u gebruikersprofielen wilt bewerken om een federatie-id op te nemen, selecteert u **Alleen SAML 2.0-verificatie toestaan** Hiermee wordt de mogelijkheid om zich aan te melden bij Workfront verwijderd met de URL bypass (`<yourdomain>`.my.workfront.com/login).
