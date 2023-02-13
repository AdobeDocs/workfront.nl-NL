---
title: Configureren [!DNL Workfront] with [!DNL Adobe Experience Manager] verouderde connector
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als [!DNL Adobe Workfront] beheerder, kunt u integreren [!DNL Workfront] met Adobe Experience Manager (AEM) Assets en biedt uw organisatie een uitgebreide oplossing voor inhoudsbeheer voor het maken, delen en onderhouden van middelen binnen uw workflow.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 024b8606-a9b7-413a-b393-8e5cdff37dd4
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 0%

---

# Configureren [!DNL Workfront] with [!DNL Adobe Experience Manager] verouderde connector

Als [!DNL Adobe Workfront] beheerder, kunt u integreren [!DNL Workfront] with [!UICONTROL Adobe Experience Manager (AEM) Assets] en biedt uw organisatie een uitgebreide oplossing voor inhoudsbeheer voor het maken, delen en onderhouden van middelen binnen uw workflow.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## [!DNL Workfront for AEM Assets]

De [!DNL Workfront for AEM Assets connector] staat uw organisatie toe om het volgende te doen:

* Creatieve inhoud samenwerken en beheren door AEM middelen en mappen te koppelen aan projecten, taken, problemen en verzoeken in [!DNL Workfront].

   Voor meer informatie over het vormen van documentatie integraties met derdetoepassingen, zie  [Documentintegratie configureren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

* Integreer met de [!DNL AEM Digital Asset Managemen]t (DAM)-opslagplaats, zodat u [!DNL Workfront] het beheren en delen van in de DAM opgeslagen digitale middelen.

   Zie voor meer informatie over het koppelen van documenten en elementmappen de   [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

* Combineer en pas meta-gegevens van beide toepassingen op activa toe.
* Een allesomvattende communicatiestream voor een element weergeven. Updates en opmerkingen die zijn gemaakt op een element in [!DNL Workfront] of [!UICONTROL AEM Assets] worden gesynchroniseerd met de andere toepassing, waarbij een uitgebreide geschiedenis wordt vastgesteld van de communicatie met het middel.

   Meer informatie over het maken van opmerkingen in [!DNL Workfront], zie [Een update toevoegen aan een document](../../documents/managing-documents/add-update-documents.md).

## Vereisten voor de installatie van de [!DNL AEM Assets] connector

Voordat u de [!DNL Workfront] connector voor [!UICONTROL AEM Assets]te waarborgen dat aan de volgende voorwaarden wordt voldaan:

* [!UICONTROL AEM Assets] geïnstalleerd en geconfigureerd, versie 6.5 of hoger. Voor informatie over installeren [!UICONTROL AEM Assets], zie de [[!DNL Adobe Experience Manager] documentatie](https://experienceleague.adobe.com/docs/experience-manager.html).
* (Voorwaardelijk) als uw firewallregels verkeer niet zoals verwacht toestaan, voeg het IP van uw cluster adres en/of domein aan uw lijst van gewenste personen toe. Zie voor meer informatie [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Installeer de [!DNL Workfront for AEM Assets] aansluitingspakket {#install-the-workfront-for-aem-assets-connector-package}

>[!IMPORTANT]
>
>De volgende instructies gelden voor een [!DNL Workfront with AEM Assets] verouderde aansluiting die is vervangen door de [[!DNL Workfront for Experience Manager] verbeterde aansluiting](../../documents/workfront-and-experience-manager-integrations/workfront-for-experience-manager-enhanced-connector/workfront-for-aem-enhanced-connector.md). Neem contact op met uw accountvertegenwoordiger voor meer informatie.

Als u het dialoogvenster [!DNL Workfront for AEM Assets] -aansluiting, moet u de connector in AEM importeren als een pakket met behulp van de [!UICONTROL CRX Package Manager].

1. Download op een werkstation waarop u al AEM hebt geïnstalleerd de [!DNL Workfront for AEM Assets] Installatiebestand van connector.

   U kunt de [!DNL Workfront for AEM Assets] aansluiting van uw [!DNL Workfront] vertegenwoordiger.

1. Meld u aan bij AEM met een beheerdersaccount.
1. Klik op **[!UICONTROL Tools]** > **[!UICONTROL Deployment]** > **[!UICONTROL Packages]**.

   De [!UICONTROL CRX Package Manager] wordt geopend.

1. Klik op **[!UICONTROL Upload Package].**

1. In de [!UICONTROL Upload Package] , bladert u naar de [!UICONTROL Workfront Connector] pakket maken en vervolgens klikken **[!UICONTROL OK]**.\
   Het pakket wordt weergegeven in het dialoogvenster [!UICONTROL CRX Package Manager].

1. Klik op **[!UICONTROL Install].**

1. Op de [!UICONTROL Package] , negeert u de geavanceerde instellingen en klikt u op **[!UICONTROL Install]**.
1. (Optioneel) Om te bevestigen dat de aansluiting is geïnstalleerd, dient u de volgende instructies weer te geven in het dialoogvenster [!UICONTROL Activity Log]:

   ```
   Package installed in <time>
   ```

1. Sluit de [!UICONTROL CRX Package Manager].

   De connector is geïnstalleerd en u kunt nu configureren [!DNL AEM Assets] om te integreren met [!DNL Workfront].

1. Doorgaan met [Configureren [!DNL AEM Assets] om te integreren met [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront).

## Configureren [!DNL AEM Assets] om te integreren met [!DNL Workfront] {#configure-aem-assets-to-integrate-with-workfront}

Nadat u de connector hebt geïnstalleerd, importeert u het aansluitingspakket om AEM te AEM en te configureren voor koppeling met documenten in [!DNL Workfront].

Voor informatie over het installeren van de connector raadpleegt u  [Installeer de [!DNL Workfront for AEM Assets] aansluitingspakket](#install-the-workfront-for-aem-assets-connector-package).

* [Vereisten](#prerequisites)
* [AEM integreren met [!DNL Workfront]](#integrate-aem-with-workfront)
* [Configureer de [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer)

### Vereisten {#prerequisites}

Voordat u begint, moet u machtigingen inschakelen voor workfront-service:

1. Ga in AEM naar **[!UICONTROL Tools]**> **[!UICONTROL Security]**> **[!UICONTROL Permissions]**.
1. Kies in de linkerbovenhoek de optie **[!UICONTROL Users]**&#x200B; in het drop-down menu en ga in *[!UICONTROL workfront-service]* in de **[!UICONTROL Search]**&#x200B;. Selecteer [!UICONTROL workfront-service] gebruiker.
1. Selecteer rechts van het scherm de optie **[!UICONTROL Add ACE]** om nieuwe vermeldingen te maken.
1. In de &#x200B;**[!UICONTROL Add New Entry]**&#x200B; venster, selecteer checkbox pictogram in **[!UICONTROL Path]**&#x200B; en kies de map: */conf*
1. Voer in het veld Bevoegdheden het volgende in: *jcr:lezen*
1. Selecteren **[!UICONTROL Add]**&#x200B; in de rechterbovenhoek
1. (Optioneel) Herhaal de stappen om meer items te maken.

### AEM integreren met [!DNL Workfront] {#integrate-aem-with-workfront}

1. Meld u als beheerder aan bij AEM Assets.
1. Klikken **[!UICONTROL Tools]** >**[!UICONTROL Cloud Services]**>**[!UICONTROL Workfront Integration Configuration]** >**[!UICONTROL Global-Workfront].**&#x200B;**&#x200B;**

1. (Voorwaardelijk) Als u dit nog niet hebt gedaan, maakt u een [!DNL Workfront] cloudconfiguratiebestand.

   1. Klikken  **[!UICONTROL Create]** in de rechterbovenhoek van het dialoogvenster [!DNL Global-Workfront] pagina.
   1. In de **[!UICONTROL Workfront URL]** de URL voor uw [!DNL Workfront] -instantie.

      Bijvoorbeeld: [!DNL https]://`<account>`.my.workfront.com, waar `<account>` Dit is de account die u gebruikt voor integratie met AEM.

   1. In de &#x200B;**[!UICONTROL Base Folder]** , selecteert u het pictogram van het selectievakje en selecteert u in de vervolgkeuzelijst het pad waar de documenten naartoe worden gekoppeld [!DNL Workfront] objecten worden opgeslagen.
   1. In het modaal AEM dat verschijnt, volg de weg aan de omslag met de documenten die met worden verbonden [!DNL Workfront] objecten. Kies de map en druk op **[!UICONTROL Select]**&#x200B; in de rechterbovenhoek.

      U kunt een koppeling maken naar elke map onder de hoofdmap /content/dam/.

   1. In de **[!UICONTROL Workfront API Key]** in, geeft u uw [!UICONTROL Workfront] API-sleutel.

      Om uw [!DNL Workfront] API-sleutel:

      1. Open een browsertabblad en meld u aan bij [!DNL Workfront] account als [!DNL Workfront] beheerder.
      1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

      1. Klik op **[!UICONTROL System]** >**[!UICONTROL Customer Info]**.

         Als u al een API-sleutel hebt gegenereerd, kunt u [!DNL Workfront] API-sleutel wordt weergegeven onder het sleutellabel van de API van uw gebruiker.

      1. (Voorwaardelijk) Als u nog geen API-sleutel hebt gegenereerd, moet u een sleutel genereren:

         1. In de **[!UICONTROL API Key Settings]** de **[!UICONTROL After Creation, API keys expire in]** is ingesteld op Geen.

            Als u een vervalperiode selecteert, zal de schakelaar ophouden werkend nadat de Sleutel van API verloopt. Vervolgens moet u een API-sleutel opnieuw genereren en uw [!DNL Workfront] configuratie.

         1. Onder de **[!UICONTROL Your User's API Key]** label, klik **[!UICONTROL Generate API Key]**.

            Een API-sleutel voor [!DNL Workfront] worden gegenereerd en weergegeven.
      1. Kopieer de API-sleutel naar het klembord.
      1. Open het browsertabblad voor AEM Connector en in het dialoogvenster **[!DNL Workfront API Key]** plakken de gekopieerde API-sleutel.
   1. (Voorwaardelijk) Klik op de knop **[!UICONTROL Advanced]** in de linkerbovenhoek van het dialoogvenster [!UICONTROL [!DNL Workfront] Integration Configuration] en selecteer indien van toepassing de volgende opties:

      **[!UICONTROL Allow Collection Browsing]:**&#x200B; Selecteer deze optie als uw organisatie dit toestaat [!DNL Workfront] gebruikers om AEM Assets-verzamelingen te koppelen aan [!DNL Workfront] objecten.

      **[!UICONTROL User Federated ID]:** Selecteer deze optie als uw organisatie Federatieve ID&#39;s of Single Sign-On (SSO) gebruikt wanneer u zich aanmeldt bij Workfront.

      **[!UICONTROL Ignore Email Domain]:** Selecteer deze optie als uw AEM gebruikers de domeinnaam niet in hun gebruikers-id gebruiken.

      **[!UICONTROL Restrict Access]:** Selecteer deze optie om het juiste op te geven [!DNL Workfront] IP adressen die aan de lijst van gewenste personen moeten worden toegevoegd. Voor meer informatie over de lijst van gewenste personen, zie [De lijst van gewenste personen van uw firewall configureren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   1. Klik op de knop **[!UICONTROL Basic]** in de linkerbovenhoek van de pagina van de Configuratie van de Integratie van Workfront, en klik dan **[!UICONTROL Connect]**.

      >[!NOTE]
      >
      >Het kan enige tijd duren om wijzigingen toe te passen. Door de bundel opnieuw te starten, kan het proces worden versneld.



1. (Voorwaardelijk) Als u al een [!DNL Workfront] wolkenconfiguratiebestand, selecteren **[!UICONTROL Global-[!DNL Workfront]]** en vervolgens in de linkerbovenhoek klikt u op **[!UICONTROL Properties]**.

1. De AEM API-sleutel genereren door te klikken **[!UICONTROL Generate Key],** kopieer vervolgens de AEM API-sleutel naar het klembord.

   U hebt de AEM API-sleutel later nodig wanneer u de configuratie [!UICONTROL Workfront] om te integreren met [!UICONTROL AEM Assets]. Zie voor meer informatie [Workfront configureren voor integratie met AEM middelen](#configure-workfront-to-integrate-with-aem-assets).

1. Klik in de rechterbovenhoek op **[!UICONTROL Save]**.

   De [!UICONTROL Global-[!DNL Workfront]] wordt weergegeven.

   ![Properties.png](assets/properties-350x117.png)

1. (Optioneel) Bidirectionele communicatie tussen AEM en [!DNL Workfront].

   1. Klik op **[!UICONTROL Global-[!DNL Workfront]].**
   1. Klik in de linkerbovenhoek van het venster op **[!UICONTROL Properties]**.

      De [!UICONTROL [!DNL Workfront] Integration Configuration] wordt weergegeven.

      ![Eigenschappen2.png](assets/properties2-350x444.png)

   1. (Optioneel) U kunt de synchronisatie van opmerkingen inschakelen tussen [!UICONTROL AEM Assets] en [!DNL Workfront], klikt u op **[!UICONTROL Enable Comment Sync]**.

      >[!IMPORTANT]
      >
      >U moet [!UICONTROL Document Sync] om de elementen te synchroniseren.

   1. (Optioneel) Klik op **[!UICONTROL Disable Comment Sync].**

      of

      Verwijder de [!UICONTROL NOTE CREATE] op uw AEM-exemplaar geregistreerd gebeurtenisabonnement.

      Voor informatie over gebeurtenisabonnementen, zie [Event Subscription API](../../wf-api/general/event-subs-api.md).

1. Doorgaan met [Configureer de [!UICONTROL AEM Externalizer]](#configure-the-aem-externalizer).

### Configureer de [!UICONTROL AEM Externalizer] {#configure-the-aem-externalizer}

De [!UICONTROL AEM Externalizer] staat AEM toe om URLs in een formaat over te gaan dat kan worden gebruikt binnen [!DNL Workfront]. Indien niet correct geconfigureerd, [!DNL Workfront] Kan geen aanroepen uitvoeren naar de AEM-API en de URL&#39;s die AEM documenten in Workfront koppelen, werken niet.

1. Klik in AEM op **[!UICONTROL Tools]** > **[!UICONTROL Operations]** >**[!UICONTROL Web Console]**.

1. Klikken **[!UICONTROL OSGI]** en klik vervolgens op **[!UICONTROL Configuration]** in het vervolgkeuzemenu.

1. Selecteer &#x200B; in de configuratielijst **[!UICONTROL Day CQ Link Externalizer].**

   De [!UICONTROL Externalizer] wordt weergegeven.

1. In de **[!UICONTROL Domains]** in, zorgt u voor het domein dat wordt vermeld in het dialoogvenster [!UICONTROL Author] Veld is de domeinnaam die extern toegankelijk is voor AEM gebruikers.

   De domeinnaam in het dialoogvenster [!UICONTROL author] veld moet overeenkomen met het domein dat wordt vermeld in de URL-regel van uw AEM.

   ![[!DNL Extenalizer].png](assets/extenalizer-350x128.png)

1. (Voorwaardelijk) Werk indien nodig het domein in de [!UICONTROL Author] veld.
1. Klik op **[!UICONTROL Save]**.

   [!UICONTROL AEM Assets] is nu geconfigureerd voor het koppelen van documenten met [!DNL Workfront]

1. Doorgaan met [Configureren [!DNL Workfront] om te integreren met [!DNL AEM assets]](#configure-workfront-to-integrate-with-aem-assets).

## Configureren [!DNL Workfront] om te integreren met [!DNL AEM assets] {#configure-workfront-to-integrate-with-aem-assets}

Nadat u de [!UICONTROL Workfront for AEM Assets] Connector (zoals beschreven in [Installeer de [!UICONTROL Workfront for AEM Assets] aansluitingspakket](#install-the-workfront-for-aem-assets-connector-package)) en configureren [!UICONTROL AEM Assets] (zoals beschreven in [Configureren[!UICONTROL  AEM Assets] om te integreren met [!DNL Workfront]](#configure-aem-assets-to-integrate-with-workfront)), moet u configureren [!DNL Workfront] documenten koppelen tussen [!DNL Workfront] en [!DNL AEM Assets].

1. Aanmelden bij [!DNL Workfront] als [!UICONTROL Workfront] beheerder.

   >[!TIP]
   >
   >[!UICONTROL Workfront] raadt u aan een [!UICONTROL Workfront] beheerder die uitsluitend is gewijd aan uw AEM integratie. Voor meer informatie over het toewijzen van de [!UICONTROL Workfront] toegangsniveau van de beheerder tot een gebruiker, zie [Gebruikers administratieve toegang verlenen tot bepaalde gebieden](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Documents]**> **[!UICONTROL Custom Integration].**

1. Klik op **[!UICONTROL Add Custom Integration]**.
1. In de **[!UICONTROL Name]** geeft u de naam van de aangepaste integratie op.

   Dit is de naam die gebruikers zien wanneer ze de integratie binnen gebruiken [!UICONTROL Workfront]; U kunt bijvoorbeeld *&quot;[!DNL AEM Assets]&quot;* voor de naam.

1. In de **[!UICONTROL Base API URL]** geeft u de URL voor uw AEM-instantie op.

   De basis-API-URL bestaat uit de URL voor uw AEM-instantie, gevolgd door het pad: /bin/webhooks/api/

   ![mceclip3.png](assets/mceclip3-350x130.png)

1. In de **[!UICONTROL Authentication Type]** vervolgkeuzelijst, selecteert u **[!UICONTROL ApiKey].**

1. In de &#x200B;**[!UICONTROL API Key]** vak, plak de AEM API-sleutel die u hebt gekopieerd toen u de configuratie hebt geconfigureerd [!UICONTROL AEM Assets].
1. Klik op **[!UICONTROL Save]**.
1. (Optioneel) Zorg ervoor dat de integratie is gemarkeerd [!UICONTROL Active].\
   ![aem_custom_integration_active.png](assets/aem-custom-integration-active-350x81.png)

   [!DNL Workfront] is nu geconfigureerd om te werken met [!DNL AEM Assets].

   Om in AEM tot activa toegang te hebben, elk [!DNL Workfront] de gebruiker die de schakelaar moet gebruiken moet opstelling als gebruiker in AEM zijn. Voor informatie over het maken van gebruikers raadpleegt u  [De gebruikers van de opstelling om de schakelaar te gebruiken](#set-up-users-to-use-the-connector).

## De gebruikers van de opstelling om de schakelaar te gebruiken {#set-up-users-to-use-the-connector}

Gebruikers hebben alleen toegang tot de aansluiting als ze een gebruikersprofiel in AEM hebben en tot een [!DNL Workfront] groep die de niveaus van de Toegang heeft die omvat [!UICONTROL Create] en [!UICONTROL Delete] machtigingen.

Meer informatie over [!DNL Workfront] machtigingen, zie [Aangepaste toegangsniveaus maken of wijzigen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* [Gebruikers instellen in [!DNL AEM assets]](#set-up-users-in-aem-assets)

### Gebruikers instellen in [!DNL AEM assets] {#set-up-users-in-aem-assets}

1. Aanmelden bij [!DNL AEM Assets] als [!DNL Workfront] beheerder.
1. Klik op **[!UICONTROL Tools]** >**&#x200B;**&#x200B;**[!UICONTROL Security]** >**[!UICONTROL Users]**.

1. (Voorwaardelijk) Als de gebruiker geen gebruikersprofiel in AEM heeft, maakt u een AEM gebruikersprofiel.

   1. Klik op **[!UICONTROL Create User].**
   1. Voer de persoonlijke gegevens van de gebruiker in.

      ![64NewUser.png](assets/64newuser-350x524.png)

      Het veld Id is het enige vereiste veld. De AEM-id van de gebruiker moet overeenkomen met [!DNL Workfront] ID, dat de gebruiker is [!DNL Workfront] e-mailadres.

      Als u [!UICONTROL Ignore Email Domain] optie wanneer u AEM hebt geconfigureerd om te integreren met [!DNL Workfront], komt de AEM-id niet overeen met de [!DNL Workfront] e-mailadres.

1. (Voorwaardelijk) Als de gebruiker een AEM profiel heeft, opent u het AEM van de gebruiker.

   1. Klik op&#x200B;**[!UICONTROL User].**

      De [!UICONTROL User Management] wordt weergegeven.

   1. Klik op de gebruiker die u wilt toevoegen en klik vervolgens op **[!UICONTROL Properties]**.

      De instellingenpagina van de gebruiker wordt weergegeven.

1. Klik op de knop **[!UICONTROL Groups]** tab.

   ![](assets/groupstab.png)

1. Zorg ervoor dat de gebruiker tot minstens één gebruiker behoort [!DNL Workfront] groep die de niveaus van de Toegang heeft die omvat [!UICONTROL Create] en [!UICONTROL Delete] machtigingen.

   1. Als u de gebruiker aan een bestaande groep wilt toevoegen, typt u de groepsnaam in het dialoogvenster **[!UICONTROL Type Group Name]** selecteert u vervolgens de groep wanneer deze wordt weergegeven in het keuzemenu.

      of

      Als u een groep wilt selecteren waarvan de gebruiker lid is, selecteert u een groep in het dialoogvenster **[!UICONTROL Groups that this user is a member of]** sectie.

1. Klik op **[!UICONTROL Save].**
