---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets-integratie
description: U kunt uw werk verbinden met de volgende Integraties van Adobe Experience Manager Assets.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '1481'
ht-degree: 0%

---

# Configureer de [!UICONTROL Experience Manager Assets as a Cloud Service] integratie

<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de omgeving van de voorvertoningssandbox.</span>

U kunt uw werk met uw inhoud verbinden in [!DNL Experience Manager Assets]&#x200B;:

* Elementen en metagegevens verschuiven vanuit [!DNL Adobe Workfront] tot [!DNL Experience Manager Assets]&#x200B;
* Elementen koppelen van [!DNL Experience Manager Assets] aan uw projecten en taken in [!DNL Workfront&#x200B;]
* Gebruiksgevallen voor versioning vereenvoudigen
* Mappen maken die zijn gekoppeld aan [!DNL Experience Manager Assets]
* Metagegevens bijhouden voor elementen en mappen
* Projectmetagegevens synchroniseren tussen [!DNL Workfront] en [!DNL Experience Manager Assets]

U kunt ook verschillende Experience Manager Assets-opslagruimten verbinden met één Workfront-omgeving of met verschillende Workfront-omgevingen met één Experience Manager Assets-opslagplaats voor alle organisatie-id&#39;s. Volg de configuratieinstructies in dit artikel voor elke integratie u opstelling zou willen.

## Toegangsvereisten

U moet het volgende hebben:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan*</strong>
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licenties*</strong>
   </td>
   <td>[!UICONTROL Plan]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] licentie</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td>U moet [!DNL Experience Manager Assets as a Cloud Service]en u moet als gebruiker aan het product worden toegevoegd.
   </td>
  </tr>
  <tr>
   <td>Configuraties op toegangsniveau*
   </td>
   <td>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <strong>Volledige administratieve toegang verlenen aan een gebruiker</strong>.
   </td>
  </tr>
</table>


*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.


## Vereisten

Voordat u begint,

* U moet [!DNL Workfront] en [!DNL Adobe Experience Manager Assets] gekoppeld aan een organisatie-id in het dialoogvenster [!DNL Adobe Admin Consol]e. Zie voor meer informatie [verschillen in toediening op basis van Platforms ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## De integratiegegevens instellen

1. Klik op de knop **[!UICONTROL Main Menu]** in de rechterbovenhoek van Adobe Workfront en klik vervolgens op **[!UICONTROL Setup]** .
1. Selecteren **[!UICONTROL Documents]** in het linkerdeelvenster selecteert u vervolgens **[!UICONTROL [!DNL Experience Manager] Integration]**.
   >[!NOTE]
   >
   >Dit configuratiegebied wordt alleen weergegeven als uw [!DNL Workfront] milieu is opgenomen onder een [!DNL Adobe Admin Console].

1. Selecteren **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. In de **[!UICONTROL Name]** Voer de naam in die gebruikers moeten zien wanneer ze in Workfront en Experience Manager Assets met deze integratie werken.
1. In de **[!UICONTROL Navigation URL]** wordt automatisch de navigatie-URL ingevuld. Deze alleen-lezen URL wordt gebruikt om een koppeling te maken naar de [!DNL Experience Manager] van de [!UICONTROL Main Menu] voor snelle toegang.
1. Kies een opslagplaats in het menu **[!UICONTROL [!DNL Experience Manager] Assets repository]** vervolgkeuzemenu. Het systeem vult automatisch alle [!DNL Experience Manager] opslagplaatsen die zijn gekoppeld aan de organisatie-id waaraan uw gebruikersprofiel is toegewezen.
   ![Kies een ervaringsbeheeropslagplaats](assets/setup-information.png)

1. Klikken **[!UICONTROL Save]** of ga naar de [Metagegevens instellen (optioneel)](#set-up-metadata-optional) in dit artikel.

   >[!NOTE]
   >
   >Vanwege de complexiteit van de integratie kunt u de repository niet wijzigen nadat u de eerste configuratie hebt opgeslagen.

## Metagegevens instellen (optioneel)

U kunt een kaart toewijzen [!DNL Workfront] objectgegevens naar elementmediavelden in [!DNL Experience Manager] Elementen.

>[!IMPORTANT]
>
>U kunt metagegevens slechts in één richting toewijzen: van [!DNL Workfront] tot [!DNL Experience Manager]. Metagegevens voor documenten die zijn gekoppeld aan [!DNL Workfront] van [!DNL Experience Manager] kan niet worden overgedragen aan [!DNL Workfront].

### Metagegevensvelden configureren

Voordat u metagegevensvelden gaat toewijzen, moet u metagegevensvelden zowel in Workfront als in Experience Manager Assets configureren.

U kunt als volgt metagegevensvelden configureren:

1. Een metagegevensschema configureren in [!DNL Experience Manager Assets] zoals uiteengezet in [Elementmetagegevenstoewijzing tussen Adobe configureren [!DNL Workfront] en [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Aangepaste formuliervelden configureren in Workfront. [!DNL Workfront] beschikt over veel ingebouwde aangepaste velden die u kunt gebruiken. U kunt echter ook uw eigen aangepaste velden maken, zoals wordt uitgelegd in [Een aangepast formulier maken of bewerken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Uitbreiden voor meer informatie over ondersteunde Workfront- en Experience Manager Assets-velden**

**Experience Manager Assets-tags**

U kunt elk door Workfront ondersteund veld toewijzen aan een tag in Experience Manager Assets. Hiervoor moet u ervoor zorgen dat de tagwaarden in Experience Manager Assets overeenkomen met die in Workfront.

* Tags en Workfront-veldwaarden moeten exact overeenkomen in spelling en opmaak.
* Workfront-veldwaarden die zijn toegewezen aan de tags voor de elementen van Manager moeten allemaal in kleine letters worden weergegeven, zelfs als de tag in Experience Manager Assets hoofdletters lijkt te bevatten.
* Workfront-veldwaarden mogen geen spaties bevatten.
* De veldwaarde in Workfront moet ook de mapstructuur van de Experience Manager Assets-tag bevatten.
* Als u meerdere tekstvelden met één regel wilt toewijzen aan labels, voert u een door komma&#39;s gescheiden lijst met de tagwaarden in aan de Workfront-zijde van de metagegevenstoewijzing, en `xcm:keywords` aan de zijde van Experience Manager Assets. Elke veldwaarde wordt toegewezen aan een afzonderlijke tag. U kunt een berekend veld gebruiken om meerdere Workfront-velden te combineren tot één door komma&#39;s gescheiden tekstveld.
* U kunt waarden toewijzen uit vervolgkeuzelijsten, keuzerondjes of selectievakjes door een lijst met door komma&#39;s gescheiden waarden in te voeren in het veld.


>[!INFO]
>
>**Voorbeeld**: Als u de tag in de mapstructuur hier wilt weergeven, krijgt de veldwaarde in Workfront de waarde `landscapes:trees/spruce`. Noteer de kleine letters in de veldwaarde van Workfront.
>
>Als u wilt dat het label het meest linkse item in de codestructuur is, moet het worden gevolgd door een dubbele punt. In dit voorbeeld wordt de veldwaarde in Workfront als volgt toegewezen aan de landscapes-tag `landscapes:`.
>
>![Mapstructuur in AEM](assets/aem-folder-structure-with-red-boxes.png)


Nadat u de tags in Experience Manager Assets hebt gemaakt, worden deze weergegeven onder de vervolgkeuzelijst Codes in de sectie Metagegevens. Als u een veld wilt koppelen aan een tag, selecteert u `xcm:keywords` in de vervolgkeuzelijst Experience Manager Assets-veld in het gebied voor metagegevenstoewijzing.

Ga voor meer informatie over tags in Experience Manager Assets, waaronder het maken en beheren van tags naar [Tags beheren](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Aangepaste Experience Manager Assets-metagegevensschemavelden**

U kunt zowel ingebouwde als aangepaste Workfront-velden toewijzen aan aangepaste metagegevensschemavelden in Experience Manager Assets.

Aangepaste metagegevensvelden die zijn gemaakt in Experience Manager Assets, worden in hun eigen sectie geordend in het instellingsgebied voor metagegevens.

![sectie Aangepaste metagegevens](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront-velden**

U kunt ingebouwde en aangepaste Workfront-velden toewijzen aan Experience Manager Assets. De volgende veldwaarden moeten in beide gevallen overeenkomen met de spelling tussen Workfront en Experience Manager Assets:

* Vervolgkeuzelijsten
* Meerdere velden selecteren

>[!TIP]
>
> Ga naar
>
> * Setup > Custom Forms in Workfront of het veld in het object
> * Middelen > Metagegevensschema&#39;s in Experience Manager Assets


+++

### Metagegevens toewijzen voor elementen

Metagegevens worden toegewezen wanneer een element wordt verschoven van [!DNL Workfront] voor het eerst. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst wordt verzonden naar [!DNL Experience Manager Assets].

Metagegevens toewijzen voor elementen:

1. Selecteren **[!UICONTROL Assets]** boven de tabel met metagegevens.
1. In de **[!UICONTROL [!DNL Workfront] field]** kiest u een ingebouwd of aangepast Workfront-veld.

   >[!NOTE]
   >
   >U kunt één kaart toewijzen [!DNL Workfront] veld naar meerdere [!UICONTROL Experience Manager Assets] velden. U kunt geen meerdere toewijzen [!DNL Workfront] velden naar één [!DNL Experience Manager Assets] veld.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->


1. In de [!DNL Experience Manager Assets] , doorzoeken in de vooraf ingevulde categorieën of ten minste twee letters invoeren in het zoekveld voor toegang tot extra categorieën.
1. Herhaal stap 2 en 3 zo nodig.
   ![metagegevensvelden](assets/asset-metadata.png)
1. Klikken [!UICONTROL Save] of ga naar de [Mappen](#folders) in dit artikel.

### Metagegevens toewijzen aan mappen

Wanneer gebruikers een gekoppelde map maken voor een project, worden de bijbehorende project-, portfolio- en programmagegevens toegewezen aan de metagegevensvelden van mappen in [!DNL Experience Manager Assets].

>[!NOTE]
>
>Deze integratie ondersteunt geen aangepaste metagegevens van [!DNL Adobe Experience Manager].

Metagegevens toewijzen voor mappen:

1. Selecteren **[!UICONTROL Folders]** boven de tabel met metagegevens.
1. In de **[!UICONTROL [!DNL Workfront] field]** kiest u een ingebouwd of aangepast Workfront-veld.

   >[!NOTE]
   >
   >U kunt één Workfront-veld toewijzen aan meerdere Experience Manager Assets-velden. U kunt geen meerdere toewijzen [!DNL Workfront] velden naar één [!DNL Experience Manager Assets] veld.

1. In de **[!DNL Experience Manager Assets]** , doorzoeken in de vooraf ingevulde categorieën of ten minste twee letters invoeren in het zoekveld voor toegang tot extra categorieën.
1. Herhaal stap 2 en 3 zo nodig.
   ![mapmetagegevens](assets/folder-metadata.png)
1. Klikken **[!UICONTROL Save]** of ga naar de [Synchronisatie van metagegevens van project](#project-metadata-sync) in dit artikel.


### Metagegevens van object synchroniseren

An [!DNL Experience Manager] velden die zijn toegewezen aan [!DNL Workfront] portfolio, programma, project, taak, uitgave en documentvelden worden automatisch bijgewerkt wanneer het veld wordt gewijzigd in [!DNL Workfront].

>[!IMPORTANT]
>
>Gebruikers moeten schrijftoegang hebben in [!DNL Experience Manager] voor elementen die in het object leven, zodat de metagegevens gesynchroniseerd worden wanneer deze worden bijgewerkt.

1. De optie **[!UICONTROL Sync object metadata]** veld.
1. Klikken **Opslaan** of ga naar de [Workflows instellen (optioneel)](#set-up-workflows-optional) in dit artikel.

<!--Courtney start here-->

<div class="preview">

## Workflows instellen (optioneel)

Een werkstroom is een reeks acties die Workfront verbinden met Adobe Experience Manager as a Cloud Service. Als Workfront-beheerder kunt u workflows configureren in Workfront en deze vervolgens toewijzen aan projectsjablonen. Wanneer een Project wordt gecreeerd gebruikend een Malplaatje van het Project waaraan een werkschema wordt toegewezen, worden de acties die in het werkschema worden bepaald teweeggebracht.

De standaardwerkschemawaarden die u in de integratie plaatst kunnen op de niveaus van het Malplaatje van het Project en van het Project worden met voeten getreden.

### Een workflow instellen voor het maken van aan Adobe Experience Manager gekoppelde mappen

1. Schakelen tussen **[!UICONTROL Create Linked folder]** op.
1. Kies een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.
   ![Navigatie naar gekoppelde mappen](assets/select-folder-aem-integration.png)
1. De optie **Portfolio- en programmanamen toevoegen** automatisch namen van Portfolio en Programma&#39;s opnemen aan het einde van de naam van de gekoppelde map.
1. Klikken **Opslaan** of ga naar de [Gekoppelde mappen instellen (optioneel)](#set-up-linked-folders-optional) in dit artikel.

</div>

<!--Courtney end here-->

## Gekoppelde mappen instellen (optioneel)

U kunt gebruikers toestaan om mappen te maken die zijn gekoppeld aan [!DNL Experience Manager] while in een [!DNL Workfront] project. Wanneer een map is gekoppeld, worden alle aan de map toegevoegde middelen automatisch in beide weergegeven [!DNL Workfront] en [!DNL Experience Manager]. Wanneer een middel aan de verbonden omslag in wordt toegevoegd [!DNL Workfront] voor het eerst worden de metagegevens van het element doorgegeven aan [!DNL Experience Manager Assets].

In de onderstaande stappen geeft u aan waar u de gekoppelde mappen wilt maken. Elke integratie kan slechts één locatie voor alle gekoppelde mappen hebben.

Gekoppelde mappen instellen:

1. Schakelen tussen **[!UICONTROL Enable Linked folder]** op.
1. Kies een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.

   >[!NOTE]
   >
   >Gebruikers hebben schrijftoegang nodig in [!DNL Adobe Experience Manager Assets] naar de opgegeven map om een gekoppelde map te maken.

1. Klik op **[!UICONTROL Save]**.
