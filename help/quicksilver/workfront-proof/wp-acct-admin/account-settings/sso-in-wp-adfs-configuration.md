---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: '''Single Sign-On'' in [!DNL Workfront Proof]: AD FS-configuratie'''
description: Als u een beheerder bent op uw AD-server, kunt u AD FS installeren en configureren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '860'
ht-degree: 0%

---

# Single Sign-On [!DNL Workfront Proof]: AD FS-configuratie

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Als u een beheerder bent op uw AD-server, kunt u AD FS installeren en configureren.

## AD FS installeren en configureren

1. Downloaden [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) naar uw computer.
1. Open het gedownloade AdfsSetup.exe- dossier om de Tovenaar van de Installatie van ADFS (de Actieve Diensten van de Federatie van de Folder) te beginnen.
1. Voor het scherm van de Rol van de Server, selecteer één van de opties (u hebt minstens een Server van de Federatie nodig).
1. Als u IIS op uw server van de ADVERTENTIE aan Internet (havens 80 en 443 voor HTTP en HTTPS) niet wilt blootstellen, kunt u eerst opstelling een Server van de Federatie achter de firewall, dan een tweede Volmacht van de Server van de Federatie bouwen die verzoeken door de firewall tot de Server van de Federatie overgaat.
1. Selecteer **[!UICONTROL Start the AD FS 2.0 Management snap-in]** en klik vervolgens op **[!UICONTROL Finish]**. Zodra dit wordt voltooid, zou het venster van het Beheer AD FS 2.0 onmiddellijk moeten openen. Zo niet, dan kunt u het openen vanuit **[!UICONTROL Start]** > **[!UICONTROL Administrative Tools]** > **[!UICONTROL AD FS 2.0 Management]**. Dit is de belangrijkste AD FS besturingsapplicatie.

1. Klik eerst op AD FS 2.0 Federation Server Configuration Wizard.
Dit zal u helpen om AD FS te vormen en het met zowel Internet via IIS als met AD te verbinden.
1. Als u een nieuwe AD FS-server configureert, selecteert u **[!UICONTROL Create a new Federation Service]**.
1. Selecteren **[!UICONTROL Stand-alone federation server]** (voor test- en evaluatiedoeleinden).

1. Voor hoge beschikbaarheid en lading het in evenwicht brengen, klik het Nieuwe landbouwbedrijf van de federatieserver.
1. Geef de naam van uw Federation Service op.
Door gebrek wint de configuratietovenaar het SSL certificaat terug verbindend aan de StandaardWebsite in IIS en zal de onderwerpnaam gebruiken die daar wordt gespecificeerd. Als u een vervangingscertificaat gebruikt zult u de naam van de Dienst van de Federatie moeten ingaan.
Als er geen SSL-certificaat is geconfigureerd in IIS, zoekt de configuratietovenaar in het lokale certificaatarchief van de computer naar geldige certificaten. Deze worden weergegeven in de vervolgkeuzelijst SSL-certificaat. Als er geen certificaten worden gevonden, kunt u de Generator van het Certificaat van de Server in IIS gebruiken om één tot stand te brengen.

1. Ga met de configuratie verder, en klik **[!UICONTROL Close]** zodra het volledig is.

## Configureren [!DNL Workfront Proof] Single Sign-On

Als u een [!DNL Workfront Proof] beheerder, kunt u Enige Sign-On op vormen [!DNL Workfront Proof] zijde. Zie voor meer informatie [Single Sign-On [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Klikken **[!UICONTROL Settings]** > **[!UICONTROL Account Settings]** en open vervolgens de **[!UICONTROL Single sign-on]** tab.

1. In de **SSO-URL** plakken.
Hieronder ziet u een voorbeeld van een entiteit-id: http://*&lt;adfs.your-company.com>*/adfs/services/trust Your Entity ID can be found in your Federation Metadata XML file.
   ![ProefHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. De Meta-gegevens van de Federatie wordt gevonden in de omslag van de Onverwacht-binnen van de ADVERTENTIE 2.0 > van de Dienst > van Eindpunten. Zoek in de sectie Metagegevens het bestand met het type Federation Metadata. Plak dit eindpunt in uw browser om metagegevens weer te geven. U kunt ook rechtstreeks naar deze koppeling gaan: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml nadat u {adfs.your-company.com hebt vervangen door uw eigen gegevens.
1. In de **[!UICONTROL Login URL]** plakken uw SSO-aanmelding.
1. Hieronder ziet u een voorbeeld van een SSO-aanmelding:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Deze koppeling kan worden gevonden in het XML-bestand met metagegevens van de Federatie.
   ![ProefHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. In de **[!UICONTROL Logout URL]** , voert u de koppeling in en slaat u deze op.
Hieronder ziet u een voorbeeld van een aanmeldings-URL: https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Ga naar uw manager van ADVERTENTIE FS > Betrouwbaarheidsrelaties > Relying Party Trusts - ProefHQ eigenschappen.
   1. Klik onder Eindpunten op [!UICONTROL Add and entry] met de volgende gegevens:

      * Eindpunttype = SAML-uitloging
      * Binding = POST
      * URL = https://*&lt;adfs.your-company.com span=&quot;&quot; id=&quot;1&quot; translate=&quot;no&quot; />>/adfs/ls/?wa=wsignout1.0*
      * Deze stap kan na het vormen van het Vertrouwen van de Relying Partij (zie hieronder) in uw VALS van de ADVERTENTIE worden voltooid.
   1. In de **[!UICONTROL Certificate fingerprint]** voert u de gegevens van uw certificaat in.
   1. Ga naar uw onverwacht-binnen ADFS 2.0 navigeer aan de Dienst > Certificaten > Symbolische ondertekening.
   1. Klik met de rechtermuisknop op dit item om het certificaat weer te geven.
   1. Van de [!UICONTROL Certificate Details] kopieert u de Thumbprint en plakt u deze in het dialoogvenster **[!UICONTROL Workfront Proof Single Sign-On]** tabblad Configuratie.

   1. De vingerafdruktekens kunnen worden gescheiden met dubbele punten of spaties, maar deze worden wel verwijderd. Als u problemen hebt met uw Single Sign-On configuratie, neemt u contact op met het Customer Support-team.


## Een vertrouwen van een betrouwbare partij toevoegen

Zodra de configuratie volledig is, moet u in de Relying sectie van de Vertrouwen van de Partij in uw VALS van de ADVERTENTIE werken.

1. Navigeren naar **[!UICONTROL Trust Relationships]** > **[!UICONTROL Relying Party Trusts]** map, en klik vervolgens op **[!UICONTROL Add a Relying Party Trust]** om de configuratietovenaar te beginnen.

1. Selecteer de gegevensbron.
Alle metagegevens voor uw [!DNL ProofHQ] account bevindt zich onder een link als deze: https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq Dit zal het grootste deel van het Vertrouwen van de Relying Partij vormen.

   >[!NOTE]
   >
   >* Als u problemen hebt met het tot stand brengen van de verbinding via de URL, slaat u de metagegevens op als een bestand en kiest u ervoor gegevens uit een bestand te importeren.
   >* Wanneer u een volledig die domein van de Douane (b.v., www.your-proofing.com) op uw hebt wordt gevormd [!DNL ProofHQ] -account vervangt het volledige deel &quot;{yoursubdomain}.proofhq.com&quot; door uw eigen domein om uw [!DNL ProofHQ] koppeling naar metagegevens.



## Claimregels configureren

Zodra uw configuratie van het Vertrouwen van de Relying Partij volledig is, bent u bereid om de eisenregels te vormen om de opstelling te voltooien. U zult twee claimregels voor ProofHQ vormen: E-mail en naam-id.

1. Open de **[!UICONTROL Edit Claim Rules]** in.
1. Ga naar **[!UICONTROL ProofHQ Relying Party Trust]** en klik vervolgens op **[!UICONTROL Edit Claim Rules]** (1)\
   De pop-up zou automatisch moeten openen als u deze optie aan het eind van het vormen van het vertrouwen selecteerde.

1. Klikken **[!UICONTROL Add Rule]** (2) om het venster van de claimconfiguratie te openen.

   * E-mail (verzendt LDAP-kenmerken als Claims Rule-sjabloon)
   * NameID (een regelsjabloon voor inkomende claims transformeren)
