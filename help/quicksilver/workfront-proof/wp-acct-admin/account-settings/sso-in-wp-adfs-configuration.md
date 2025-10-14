---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Single Sign-On in  [!DNL Workfront Proof]: Configuratie AD FS'
description: Als u een beheerder bent op uw AD-server, kunt u AD FS installeren en configureren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: 690b0817dfe4ff200982ffe8d67ad93e563e30ac
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 0%

---

# Single Sign-On in [!DNL Workfront Proof]: AD FS-configuratie

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

Als u een beheerder bent op uw AD-server, kunt u AD FS installeren en configureren.

## AD FS installeren en configureren

1. Download Microsoft AD FS 2.0 naar uw computer.
1. Open het gedownloade AdfsSetup.exe- dossier om de Tovenaar van de Installatie van ADFS (de Actieve Diensten van de Federatie van de Folder) te beginnen.
1. Voor het scherm van de Rol van de Server, selecteer één van de opties (u hebt minstens een Server van de Federatie nodig).
1. Als u IIS op uw server van de ADVERTENTIE aan Internet (havens 80 en 443 voor HTTP en HTTPS) niet wilt blootstellen, kunt u eerst opstelling een Server van de Federatie achter de firewall, dan een tweede Volmacht van de Server van de Federatie bouwen die verzoeken door de firewall tot de Server van de Federatie overgaat.
1. Als u de installatie van AD FS hebt voltooid, selecteert u **[!UICONTROL Start the AD FS 2.0 Management snap-in]** en klikt u op **[!UICONTROL Finish]** . Zodra dit wordt voltooid, zou het venster van het Beheer AD FS 2.0 onmiddellijk moeten openen. Als dat niet het geval is, kunt u deze openen vanuit **[!UICONTROL Start]** > **[!UICONTROL Administrative Tools]** > **[!UICONTROL AD FS 2.0 Management]** . Dit is de belangrijkste AD FS besturingsapplicatie.

1. Klik eerst op AD FS 2.0 Federation Server Configuration Wizard.
Dit zal u helpen om AD FS te vormen en het met zowel Internet via IIS als met AD te verbinden.
1. Selecteer **[!UICONTROL Create a new Federation Service]** als u een nieuwe AD FS-server configureert.
1. Selecteer **[!UICONTROL Stand-alone federation server]** (voor test- en evaluatiedoeleinden).

1. Voor hoge beschikbaarheid en lading het in evenwicht brengen, klik het Nieuwe landbouwbedrijf van de federatieserver.
1. Geef de naam van uw Federation Service op.
Door gebrek wint de configuratietovenaar het SSL certificaat terug verbindend aan de StandaardWebsite in IIS en zal de onderwerpnaam gebruiken die daar wordt gespecificeerd. Als u een vervangingscertificaat gebruikt zult u de naam van de Dienst van de Federatie moeten ingaan.
Als er geen SSL-certificaat is geconfigureerd in IIS, zoekt de configuratietovenaar in het lokale certificaatarchief van de computer naar geldige certificaten. Deze worden weergegeven in de vervolgkeuzelijst SSL-certificaat. Als er geen certificaten worden gevonden, kunt u de Generator van het Certificaat van de Server in IIS gebruiken om tot één te leiden.

1. Ga verder met de configuratie en klik op **[!UICONTROL Close]** zodra deze is voltooid.

## [!DNL Workfront Proof] Single Sign-On configureren

Als u een [!DNL Workfront Proof] -beheerder bent, kunt u Single Sign-On configureren aan de [!DNL Workfront Proof] -zijde. Voor meer informatie, zie [&#x200B; Enige Sign-On in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Klik op **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** en open vervolgens het tabblad **[!UICONTROL Single sign-on]** .

1. In het **vak van SSO URL**, plak uw identiteitskaart van de Entiteit.
Hieronder ziet u een voorbeeld van een entiteit-id:
http://*&lt;adfs.your-company.com>* /adfs/services/trust
Uw entiteitskaart kan in uw dossier van Meta-gegevensXML van de Federatie worden gevonden.
   ![&#x200B; ProofHQ_configuration_02.png &#x200B;](assets/proofhq-configuration-02-350x80.png)

1. De Meta-gegevens van de Federatie wordt gevonden in de omslag van de Onverwacht-binnen van de ADVERTENTIE 2.0 > van de Dienst > van Eindpunten. Zoek in de sectie Metagegevens het bestand met het type Federation Metadata. Plak dit eindpunt in uw browser om metagegevens weer te geven. U kunt ook rechtstreeks naar deze verbinding gaan: https://*&lt;adfs.your-company.com>* /FederationMetadata/2007-06/FederationMetadata.xml na het vervangen van {adfs.your-company.com} met uw eigen details.
1. Plak in het vak **[!UICONTROL Login URL]** de SSO-aanmelding.
1. Hieronder ziet u een voorbeeld van een SSO-aanmelding:
1. http://*&lt;adfs.your-company.com>* /adfs/ls.
1. Deze koppeling kan worden gevonden in het XML-bestand met metagegevens van de Federatie.
   ![&#x200B; ProofHQ_configuration_03.png &#x200B;](assets/proofhq-configuration-03-350x90.png)

1. Voer in het vak **[!UICONTROL Logout URL]** de koppeling in en sla deze op.
Hieronder ziet u een voorbeeld van een aanmeldings-URL:
https://*&lt;adfs.your-company.com>* /adfs/ls/?wa=wsignout1.0

   1. Ga naar uw manager van ADVERTENTIE FS > Betrouwbaarheidsrelaties > Relying Party Trusts - ProefHQ eigenschappen.
   1. Klik onder Eindpunten op [!UICONTROL Add and entry] met de volgende details:

      * Eindpunttype = SAML-uitloging
      * Binding = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Deze stap kan na het vormen van het Vertrouwen van de Relying Partij (zie hieronder) in uw VALS van de ADVERTENTIE worden voltooid.
   1. Voer in het vak **[!UICONTROL Certificate fingerprint]** de gegevens van het certificaat in.
   1. Ga naar uw onverwacht-binnen ADFS 2.0 navigeer aan de Dienst > Certificaten > Symbolische ondertekening.
   1. Klik met de rechtermuisknop op dit item om het certificaat weer te geven.
   1. Kopieer op het tabblad [!UICONTROL Certificate Details] de Thumbprint en plak deze op het tabblad **[!UICONTROL Workfront Proof Single Sign-On]** Configuratie.

   1. De vingerafdruktekens kunnen worden gescheiden met dubbele punten of spaties, maar deze worden wel verwijderd. Als u problemen hebt met uw Single Sign-On configuratie, neemt u contact op met het Customer Support-team.


## Een vertrouwen van een betrouwbare partij toevoegen

Zodra de configuratie volledig is, moet u in de Relying sectie van de Vertrouwen van de Partij in uw VALS van de ADVERTENTIE werken.

1. Navigeer naar de map **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** en klik vervolgens op **[!UICONTROL Add a Relying Party Trust]** om de configuratietovenaar te starten.

1. Selecteer de gegevensbron.
Alle metagegevens voor uw [!DNL ProofHQ] -account bevinden zich onder een koppeling als deze:
https://`<yoursubdomain*>` .proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Dit zal het grootste deel van het Relying Vertrouwen van de Partij vormen.

   >[!NOTE]
   >
   >* Als u problemen hebt met het tot stand brengen van de verbinding via de URL, slaat u de metagegevens op als een bestand en kiest u ervoor gegevens uit een bestand te importeren.
   >* Wanneer u een volledig aangepast domein (bijvoorbeeld www.your-proofing.com) hebt dat op uw [!DNL ProofHQ] -account is geconfigureerd, vervangt u het volledige deel &quot; {yoursubdomain} .proofhq.com&quot; door uw eigen domein om een koppeling naar [!DNL ProofHQ] -metagegevens te maken.


## Claimregels configureren

Zodra uw configuratie van het Vertrouwen van de Relying Partij volledig is, bent u bereid om de eisenregels te vormen om de opstelling te voltooien. U zult twee claimregels voor ProefHQ vormen: E-mail en Naam ID.

1. Open het dialoogvenster **[!UICONTROL Edit Claim Rules]** .
1. Ga naar **[!UICONTROL ProofHQ Relying Party Trust]** en klik vervolgens op **[!UICONTROL Edit Claim Rules]** (1).\
   De pop-up zou automatisch moeten openen als u deze optie na het vormen van het vertrouwen selecteerde.

1. Klik op **[!UICONTROL Add Rule]** (2) om het venster voor claimconfiguratie te openen.

   * E-mail (verzendt LDAP-kenmerken als Claims Rule-sjabloon)
   * NameID (een regelsjabloon voor inkomende claims transformeren)
