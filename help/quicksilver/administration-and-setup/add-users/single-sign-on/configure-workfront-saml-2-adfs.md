---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront configureren met SAML 2.0 via ADFS
description: U kunt verificatie inschakelen voor Workfront met SAML 2.0.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9bc5987b-6e32-47df-90c8-08ea4b1b7451
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 0%

---

# Adobe Workfront configureren met SAML 2.0 met behulp van ADFS

{{important-admin-console-onboard}}

Als beheerder van Adobe Workfront, kunt u Workfront met een oplossing van de Prijsverhoging van de Veiligheid van de Taal (SAML) 2.0 voor enig teken-op integreren terwijl het gebruiken van de Actieve Diensten van de Federatie van de Folder (ADFS).

Deze handleiding is gericht op het instellen van ADFS zonder automatische provisioning of kenmerktoewijzingen. We raden u aan de installatie te voltooien en deze te testen voordat u automatische provisioning instelt.

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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verificatie inschakelen voor Workfront met SAML 2.0

Voer de volgende secties in om verificatie in te schakelen voor de Workfront-webtoepassing en de mobiele Workfront-toepassing met SAML 2.0:

* [&#x200B; wint het de meta-gegevensdossier van Workfront terug SSO &#x200B;](#retrieve-the-workfront-sso-metadata-file)
* [&#x200B; vormt het Relying de Vertrouwen van de Partij &#x200B;](#configure-relying-party-trusts)
* [&#x200B; vorm de Regels van de Claim &#x200B;](#configure-claim-rules)
* [Upload het metagegevensbestand en test de verbinding](#upload-the-metadata-file-and-test-the-connection)

### Het Workfront SSO-metagegevensbestand ophalen {#retrieve-the-workfront-sso-metadata-file}

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Systeem** > **Enige Sign-On (SSO)**.
1. In het **Type** drop-down menu, klik **SAML 2.0** om extra informatie en opties te tonen.
1. Kopieer URL die na **Meta-gegevens URL** toont.
1. Ga aan de volgende sectie verder, [&#x200B; vormen het Vertrouwen van de Partij van het Vertrouwen &#x200B;](#configure-relying-party-trusts).

### Reliëfpartijtrusts configureren {#configure-relying-party-trusts}

1. Open de **Manager ADFS** gebruikend de server van Vensters 2008 R2 (de versie kan variëren).
1. Ga naar **Begin.**
1. Klik **Hulpmiddelen van het Beleid.**
1. Klik **ADFS 2.0 Beheer.**
1. Selecteer **ADFS** en breid **Vertrouwensrelaties** uit.
1. Klik met de rechtermuisknop op **Relying Party Trusts** en selecteer vervolgens **Relying Party Trust** toevoegen om de Add Relying Party Trust Wizard te starten.
1. Van de **Welkome Pagina**, uitgezochte **Begin**.
1. In de **Uitgezochte Datum Source** sectie, kleef de meta-gegevens URL van Workfront.
1. Klik **daarna**.
1. Klik **O.K.** om het waarschuwingsbericht te erkennen.
1. In **specificeer de Naam van de Vertoning** sectie, voeg de Naam van de a **Vertoning** en **Nota&#39;s** toe om het Vertrouwen te onderscheiden, dan klik **daarna**.
1. Selecteer **Toestaan alle gebruiker om tot deze vertrouwende partij** toegang te hebben (of **niets** als u dit later wilt vormen).
1. Klik **daarna**.

   Dit neemt u aan **Klaar om het Vertrouwen** sectie toe te voegen.

1. Ga aan de volgende sectie [&#x200B; verder vormen de Regels van de Claim &#x200B;](#configure-claim-rules).

### Claimregels configureren {#configure-claim-rules}

1. Klik **daarna** in **Klaar om de sectie van het Vertrouwen** toe te voegen, dan ervoor te zorgen dat **de Edit de dialoogdoos van de Regels van de Claim** optie wordt geselecteerd.

   Op deze manier kunt u de regels voor claims in een volgende stap bewerken.

1. Klik **dicht**.
1. Klik **toevoegen Regel.**
1. Selecteer **verzenden Attribuut LDAP als Claims**.
1. Klik **daarna** om **te tonen vormen de stap van de Regel van de Claim**.
1. Specificeer de volgende minimumvereisten om de claimregel te vormen: (Dit zal in **identiteitskaart van de Federatie** op de gebruikersopstelling gaan en wordt gebruikt om te onderscheiden wie het programma opent.)


   <table >                
      <tbody>
            <tr>
               <td>Naam van claimregel
               </td>
               <td>Geef een naam op voor de claimregel. Bijvoorbeeld "Workfront."</td>
            </tr>
            <tr>
               <td>Kenmerkarchief</td>
               <td >Selecteer <b> Actieve Folder </b> van het drop-down menu.</td>
            </tr>
            <tr>
               <td>LDAP-kenmerk</td>
               <td>Dit kan elk type kenmerk zijn. Wij adviseren gebruikend <b> SAM-rekening-Naam </b> voor dit attribuut.</td>
            </tr>
            <tr>
               <td>Type uitgaande vordering</td>
               <td>U moet <b> identiteitskaart van de Naam </b> als uitgaand claimtype selecteren</td>
            </tr>
      </tbody>
   </table>

1. (Optioneel) Als u automatische provisioning wilt instellen, voegt u de volgende aanvullende claims toe in zowel het LDAP-kenmerk als het type uitgaande claim:

   * Voornaam
   * Achternaam
   * E-mailadres

1. Klik **Afwerking**, dan klik O.K. **&#x200B;**&#x200B;op het volgende scherm.
1. Klik met de rechtermuisknop op het nieuwe **Vertrouwen van de Partij**, dan selecteren **Eigenschappen**.
1. Selecteer het **Geavanceerde Lusje**. En onder **Veilig algoritme van de Hash** uitgezochte SHA-1 of SHA-256.

   >[!NOTE]
   >
   >De optie die u onder Veilig algoritme van de Hash selecteert moet het Veilige gebied van het Algoritme van de Hash in Workfront onder Opstelling > Systeem > Enige Sign-ON (SSO) aanpassen.

1. Ga aan de volgende sectie [&#x200B; verder uploadt het meta-gegevensdossier en test de verbinding &#x200B;](#upload-the-metadata-file-and-test-the-connection).

### Upload het metagegevensbestand en test de verbinding {#upload-the-metadata-file-and-test-the-connection}

1. Open een browser en ga naar `https://<yourserver>/FederationMetadata/2007-06/FederationMetadata.xml` .

   Hiermee moet u het bestand FederationMetadata.xml van een metagegevensbestand downloaden.

1. Klik **kiezen Dossier** onder **bevolkt gebieden van de Metagegevens van Identiteitsprovider**, en selecteer het {**dossier 4} FederationMetadata.xml.**

1. (Optioneel) Als de certificaatinformatie niet met het metagegevensbestand is gevuld, kunt u een bestand afzonderlijk uploaden. Selecteer **kiezen Dossier** in de **sectie van het Certificaat**.

1. Klik **Verbinding van de Test**. Indien correct ingesteld, ziet u een pagina die vergelijkbaar is met de hieronder weergegeven pagina:

   ![&#x200B; SAML 2 succesbericht &#x200B;](assets/success-saml-2.png)

   >[!NOTE]
   >
   >Als u aan de afbeelding van opstellingsattributen wilt, zorg ervoor dat u de attributen van de Verbinding van de Test in het Attribuut van de Folder kopieert. Zie Toewijzing van gebruikerskenmerken voor meer informatie.

1. Selecteer **Vrijstelling Admin** om de beheerders van Workfront toe te staan om het programma te openen gebruikend de geloofsbrieven van Workfront met bypass url.

   Bladwijzers die naar `<yourdomain>` .my.workfront.com/login verwijzen, omzeilen de omleiding.

1. Selecteer **toelaten** doos om de configuratie toe te laten.
1. Klik **sparen**.

## Gebruikers voor SSO bijwerken

Na deze gids, zal **Sso- Gebruikersnaam** hun **Actieve Gebruikersnaam van de Folder** zijn.

Als Workfront-beheerder kunt u updategebruikers bulksgewijs verzenden naar SSO. Voor meer informatie over het bijwerken van gebruikers voor SSO, zie [&#x200B; de gebruikers van de Update voor enig teken-op &#x200B;](../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md).

Als Workfront-beheerder kunt u ook handmatig een federatie-id toewijzen die het profiel van de gebruiker bewerkt en het veld Federation ID invult. Voor meer informatie over het uitgeven van een gebruiker, zie [&#x200B; het profiel van een gebruiker &#x200B;](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) uitgeven.

>[!NOTE]
>
>Wanneer het uitgeven van gebruikers&#39; profielen om een identiteitskaart van de Federatie te omvatten, die **selecteert slechts SAML 2.0 Authentificatie** toestaat verwijdert de capaciteit aan login aan Workfront gebruikend bypass url (`<yourdomain>` .my.workfront.com/login).
