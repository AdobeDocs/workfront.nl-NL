---
product-area: documents
navigation-topic: approvals
title: De Adobe Experience Manager gebruiken met de integratie Frame.io
description: De Adobe Experience Manager gebruiken met de integratie Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c5202bcdb367266d31a2e056eed9a286f286518
workflow-type: tm+mt
source-wordcount: '1595'
ht-degree: 0%

---


# De Adobe Experience Manager gebruiken met de integratie Frame.io

Met de &#x200B; [!DNL Experience Manager Assets] &#x200B; kunt u uw digitale middelen beheren en opslaan die de controle- en goedkeuringscyclus hebben doorlopen. Dankzij deze integratie kunt u de mogelijkheden van Adobe Experience Manager, Frame.io en Workfront benutten om uw contentbeheer en samenwerkingsprocessen te stroomlijnen.

## De Experience Manager Assets-integratie configureren

U kunt uw werk in [!DNL Experience Manager Assets] &#x200B; met uw inhoud verbinden:

* Elementen en metagegevens verplaatsen van [!DNL Adobe Workfront] naar [!DNL Experience Manager Assets] &#x200B;
* Gebruiksgevallen voor versioning vereenvoudigen
* Metagegevens bijhouden voor elementen
* Metagegevens van een project synchroniseren tussen [!DNL Workfront] en [!DNL Experience Manager Assets]

>[!NOTE]
>
>U kunt ook verschillende [!DNL Experience Manager Assets] repositories verbinden met één [!UICONTROL Workfront] -omgeving of verschillende [!DNL Workfront] -omgevingen met één [!DNL Experience Manager Assets] -opslagplaats via organisatie-id&#39;s. Volg de configuratieinstructies in dit artikel voor elke integratie u opstelling zou willen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table>
  <tr>
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Prime of Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront-licenties
   </td>
   <td>
  <p>De integratie configureren:</p>
   <p>Standard</p>
   <p>Plan</p>

<p>Documenten verzenden naar Experience Manager Assets:</p>
   <p>Medewerker of hoger</p>
   <p>Aanvraag of hoger</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Adobe Experience Manager-licenties
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td>Aanvullende producten
   </td>
   <td>U moet [!DNL Experience Manager Assets as a Cloud Service] hebben, en u moet aan het product als gebruiker worden toegevoegd.
   </td>
  </tr>
   <tr>
   <td>Configuraties op toegangsniveau
   </td>
   <td>U moet een [!DNL Workfront] beheerder zijn.
   </td>
  </tr>
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

Voordat u begint,

* U moet [!DNL Workfront] en [!DNL Adobe Experience Manager Assets] aan een Organisatie-id hebben gekoppeld in de [!DNL Adobe Admin Console] . Voor meer informatie zie, [&#x200B; Op platform-gebaseerde beleidsverschillen ([!DNL Adobe Workfront]/ [!DNL Adobe Business Platform]) &#x200B;](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
* Uw Workfront-exemplaar moet gebruikmaken van Adobe Enterprise Storage.


## De integratiegegevens instellen

{{step-1-to-setup}}

1. Selecteer **[!UICONTROL Documents]** in het linkerdeelvenster en selecteer vervolgens **[!UICONTROL [!DNL Experience Manager] Integration]** .
1. Selecteer **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. Voer in het veld **[!UICONTROL Name]** de naam in die gebruikers moeten zien wanneer ze met deze integratie werken in Workfront en Experience Manager Assets.
1. In het veld **[!UICONTROL Navigation URL]** vult het systeem automatisch de URL van de navigatie. Deze alleen-lezen URL wordt gebruikt om vanuit [!DNL Experience Manager] snel toegang te krijgen tot de [!UICONTROL Main Menu] -instantie van uw organisatie.
1. Kies een gegevensopslagruimte in het vervolgkeuzemenu **[!UICONTROL [!DNL Experience Manager] Assets repository]** . Het systeem vult automatisch alle [!DNL Experience Manager] opslagplaatsen in die zijn gekoppeld aan de organisatie-id waaraan uw gebruikersprofiel is toegewezen.
   ![&#x200B; kies de bewaarplaats van de ervaringsmanager &#x200B;](assets/setup-information.png)

1. Klik **[!UICONTROL Save]** of beweging op [&#x200B; de meta-gegevens van de Opstelling (Facultatieve) &#x200B;](#set-up-metadata-optional) sectie in dit artikel.

   >[!IMPORTANT]
   >
   >Vanwege de complexiteit van de integratie kunt u de repository niet wijzigen nadat u de eerste configuratie hebt opgeslagen.


## Metagegevens instellen (optioneel)

U kunt [!DNL Workfront] -objectgegevens toewijzen aan middelenmediavelden in [!DNL Experience Manager] Assets.

>[!NOTE]
>
>U kunt metagegevens slechts in één richting toewijzen: van [!DNL Workfront] tot [!DNL Experience Manager] . Metagegevens voor documenten die zijn gekoppeld aan [!DNL Workfront] vanuit [!DNL Experience Manager] kunnen niet worden overgebracht naar [!DNL Workfront] .

### Metagegevensvelden configureren

Voordat u metagegevensvelden gaat toewijzen, moet u metagegevensvelden zowel in Workfront als in Experience Manager Assets configureren.

U kunt als volgt metagegevensvelden configureren:

1. Vorm een meta-gegevensschema in [!DNL Experience Manager Assets] zoals die in [&#x200B; wordt verklaard vormt activa meta-gegevensafbeelding tussen Adobe  [!DNL Workfront]  en  [!DNL Experience Manager Assets] &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. Aangepaste formuliervelden configureren in Workfront. [!DNL Workfront] bevat veel ingebouwde aangepaste velden die u kunt gebruiken. Nochtans, kunt u uw eigen douanegebieden ook tot stand brengen zoals die in [&#x200B; worden verklaard creeer een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **breid uit om meer informatie over gesteunde gebieden van Workfront en van Experience Manager Assets te zien** 

**de Markeringen van Experience Manager Assets**

U kunt elk door Workfront ondersteund veld toewijzen aan een tag in Experience Manager Assets. Hiervoor moet u ervoor zorgen dat de tagwaarden in Experience Manager Assets overeenkomen met die in Workfront.

* Tags en Workfront-veldwaarden moeten exact overeenkomen in spelling en opmaak.
* Workfront-veldwaarden die zijn toegewezen aan de tags voor de elementen van Manager moeten allemaal in kleine letters worden weergegeven, zelfs als de tag in Experience Manager Assets hoofdletters lijkt te bevatten.
* Workfront-veldwaarden mogen geen spaties bevatten.
* De veldwaarde in Workfront moet ook de mapstructuur van de Experience Manager Assets-tag bevatten.
* Als u meerdere tekstvelden met één regel wilt toewijzen aan labels, voert u een door komma&#39;s gescheiden lijst van de tagwaarden in aan de Workfront-zijde van de metagegevenstoewijzing en `xcm:keywords` aan de Experience Manager Assets-zijde. Elke veldwaarde wordt toegewezen aan een afzonderlijke tag. U kunt een berekend veld gebruiken om meerdere Workfront-velden te combineren tot één door komma&#39;s gescheiden tekstveld.
* U kunt waarden toewijzen uit vervolgkeuzelijsten, keuzerondjes of selectievakjes door een lijst met door komma&#39;s gescheiden waarden in te voeren in het veld.


>[!INFO]
>
>**Voorbeeld**: Om de markering aan te passen die in de omslagstructuur hier wordt getoond, zou de gebiedswaarde in Workfront `landscapes:trees/spruce` zijn. Noteer de kleine letters in de veldwaarde van Workfront.
>
>Als u wilt dat het label het meest linkse item in de codestructuur is, moet het worden gevolgd door een dubbele punt. In dit voorbeeld zou de veldwaarde in Workfront `landscapes:` zijn om aan de landscapes-tag toe te wijzen.
>
>![&#x200B; de structuur van de Omslag in AEM &#x200B;](assets/aem-folder-structure-with-red-boxes.png)


Nadat u de tags in Experience Manager Assets hebt gemaakt, worden deze weergegeven onder de vervolgkeuzelijst Codes in de sectie Metagegevens. Als u een veld aan een tag wilt koppelen, selecteert u `xcm:keywords` in het vervolgkeuzemenu Experience Manager Assets-veld in het gebied voor metagegevenstoewijzing.

Voor meer informatie over markeringen in Experience Manager Assets, met inbegrip van hoe te om markeringen tot stand te brengen en te beheren, zie [&#x200B; het Beheer Markeringen &#x200B;](https://experienceleague.adobe.com/nl/docs/experience-manager-64/administering/contentmanagement/tags).

**de gebieden van het de douaneschema-meta-gegevens van Experience Manager Assets**

U kunt zowel ingebouwde als aangepaste Workfront-velden toewijzen aan aangepaste metagegevensschemavelden in Experience Manager Assets.

Aangepaste metagegevensvelden die zijn gemaakt in Experience Manager Assets, worden in hun eigen sectie geordend in het instellingsgebied voor metagegevens.

![&#x200B; sectie van douanemetagegevens &#x200B;](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**de gebieden van Workfront**

U kunt ingebouwde en aangepaste Workfront-velden toewijzen aan Experience Manager Assets. De volgende veldwaarden moeten in beide gevallen overeenkomen met de spelling tussen Workfront en Experience Manager Assets:

* Vervolgkeuzelijsten
* Meerdere velden selecteren

>[!TIP]
>
> Als u wilt controleren of de veldwaarden exact overeenkomen, gaat u naar
>
> * Setup > Custom Forms in Workfront of het veld in het object
> * Assets > Metagegevensschema&#39;s in Experience Manager Assets

+++

### Metagegevens toewijzen voor elementen

Metagegevens worden toegewezen wanneer een element voor het eerst vanuit [!DNL Workfront] wordt geduwd. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst naar [!DNL Experience Manager Assets] wordt verzonden.

Metagegevens toewijzen voor elementen:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Kies in de kolom **[!UICONTROL [!DNL Workfront] field]** een ingebouwd of aangepast Workfront-veld.

   >[!NOTE]
   >
   >U kunt één [!DNL Workfront] -veld toewijzen aan meerdere [!UICONTROL Experience Manager Assets] -velden. U kunt niet meerdere [!DNL Workfront] velden toewijzen aan één [!DNL Experience Manager Assets] veld.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Doorzoek in het veld [!DNL Experience Manager Assets] de vooraf ingevulde categorieën of voer in het zoekveld ten minste twee letters in voor toegang tot extra categorieën.
1. Herhaal stap 2 en 3 zo nodig.
   ![&#x200B; meta-gegevensgebieden &#x200B;](assets/metadata-no-asset-toggle.png)
1. Klik [!UICONTROL **sparen**] of beweging aan de [&#x200B; sectie van de meta-gegevenssynchronisatie van Objecten &#x200B;](#object-metadata-sync) in dit artikel.



### Metagegevens van object synchroniseren

Een [!DNL Experience Manager] -veld dat is toegewezen aan [!DNL Workfront] -portfolio, -programma, -project, -taak, -uitgave en documentvelden, wordt automatisch bijgewerkt wanneer het veld wordt gewijzigd in [!DNL Workfront] .

Als deze optie is ingeschakeld, wordt op elk element dat is doorgegeven aan Adobe Experience Manager in real-time een weergave weergegeven van de Adobe Experience Manager-metagegevens van het document op de pagina Documentdetails in Workfront.

1. Laat het **[!UICONTROL Sync object metadata]** gebied toe, dan klik **sparen**.

>[!IMPORTANT]
>
>Gebruikers moeten schrijftoegang hebben in [!DNL Experience Manager] voor elementen die in het object leven, zodat de metagegevens gesynchroniseerd kunnen worden wanneer deze worden bijgewerkt.


## Een document verzenden naar Experience Manager Assets of Elementen

U kunt documenten van Workfront naar Experience Manager Assets of Assets Essentials verzenden. Documenten die van Workfront naar Assets Essentials zijn geüpload en verzonden, tellen nog steeds mee voor de totale opslag van documenten.

Assets die naar Experience Manager door deze integratie wordt verzonden heeft een groottegrens van **5o TB**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Metagegevensvelden worden eerst toegewezen wanneer u een element verzendt van Workfront naar Experience Manager Assets of Elementen. Eventuele metagegevens die zijn geconfigureerd om toe te wijzen voor bovenliggende objecten, worden ook verzonden. Voor meer informatie bij het vormen meta-gegevensafbeelding, zie [&#x200B; de integratie van Experience Manager Assets as a Cloud Service &#x200B;](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) vormen of [&#x200B; vormen de integratie van de Hoofdzaak van Experience Manager Assets &#x200B;](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Voorbeeld** wanneer u eerst een activa verzendt in bijlage aan een project, de meta-gegevenskaarten aan Experience Manager Assets of de Hoofdzaak van Activa evenals om het even welke in kaart gebrachte meta-gegevens van oudervoorwerpen zoals een portefeuille en een programma.



### Een document verzenden vanuit Workfront

Wanneer een gebruiker een document van Workfront naar Experience Manager Assets of Assets Essentials verzendt, worden de toegewezen metagegevens over het document overgedragen. Nadat het document is verzonden, worden wijzigingen die zijn aangebracht in de metagegevens van het document in Workfront, niet doorgevoerd in Assets of Assets Essentials. Als een toegewezen veld in Workfront wordt gewijzigd, moet u een nieuwe versie van het document met de bijgewerkte metagegevens verzenden naar Assets of Assets Essentials.

Een document verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en selecteer het document u wilt verzenden.
1. Klik **verzenden naar**, dan kies de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek vermeld.

   ![&#x200B; verzendt naar &#x200B;](assets/send-to-aem.png)

1. Kies waar u de activa wilt gaan, dan klik **Uitgezochte Omslag**.
1. Wanneer u uw gewenste bestemming vindt, klik **sparen**.

### Nieuwe versie verzenden

U kunt een nieuwe versie toevoegen aan een document dat u eerder naar Workfront hebt geüpload. Voor meer informatie, zie [&#x200B; een nieuwe versie van een document &#x200B;](/help/quicksilver/documents/managing-documents/upload-new-document-version.md) uploaden. Nadat de meest recente versie is geüpload, kunt u deze naar Elementen verzenden. Als een toegewezen veld in Workfront is gewijzigd, werkt de nieuwe versie de metagegevens in Elementen bij wanneer deze worden verzonden.

>[!IMPORTANT]
>
>Voordat u een nieuwe versie naar Workfront uploadt, raden we u aan de naam van het bestand te wijzigen. Als u een nieuwe versie uploadt met precies dezelfde bestandsnaam als een vorige versie, kan alleen de meest recente versie worden gedownload van Workfront. Alle versies kunnen ongeacht de bestandsnaam worden gedownload van Experience Manager Assets of Assets Essentials. <!--Is this still a thing with ESM?-->

De meest recente versie verzenden:

1. Ga naar het **gebied van Documenten** in Workfront, en bepaal de plaats van het document.
1. Selecteer **verzenden naar**, dan kies de integratie van Experience Manager uw beheerderopstelling.

   >[!NOTE]
   >
   >De Workfront-beheerder kan een willekeurige naam voor deze integratie kiezen, dus Assets of Assets Essentials wordt niet specifiek genoemd.

   ![&#x200B; verzendt naar &#x200B;](assets/send-to-aem.png)

1. Klik **sparen**. De nieuwe versie slaat op dezelfde locatie op als de vorige versie.
