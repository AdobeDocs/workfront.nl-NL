---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De integratie van [!UICONTROL Experience Manager Assets as a Cloud Service] configureren
description: U kunt uw werk met uw inhoud in  [!DNL Experience Manager Assets] verbinden.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 315428ec517b3a6c0edae387b3a866093a49a2b2
workflow-type: tm+mt
source-wordcount: '1669'
ht-degree: 0%

---

# De integratie met [!UICONTROL Experience Manager Assets as a Cloud Service] configureren

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Deze functionaliteit is alleen beschikbaar voor organisaties die zijn aangemeld bij de [!DNL Adobe Admin Console] .

U kunt uw werk in [!DNL Experience Manager Assets] &#x200B; met uw inhoud verbinden:

* Elementen en metagegevens verplaatsen van [!DNL Adobe Workfront] naar [!DNL Experience Manager Assets] &#x200B;
* Elementen van [!DNL Experience Manager Assets] koppelen aan uw projecten en taken in [!DNL Workfront&#x200B;]
* Gebruiksgevallen voor versioning vereenvoudigen
* Aan [!DNL Experience Manager Assets] gekoppelde mappen maken
* Metagegevens bijhouden voor elementen en mappen
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
   <td>Standard
   <p>Plan</p>
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


## De integratiegegevens instellen

{{step-1-to-setup}}

1. Selecteer **[!UICONTROL Documents]** in het linkerdeelvenster en selecteer vervolgens **[!UICONTROL [!DNL Experience Manager] Integration]** .

   >[!NOTE]
   >
   >Dit configuratiegebied wordt alleen weergegeven als uw [!DNL Workfront] -omgeving is opgenomen onder een [!DNL Adobe Admin Console] .

1. Selecteer **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. Voer in het veld **[!UICONTROL Name]** de naam in die gebruikers moeten zien wanneer ze met deze integratie werken in Workfront en Experience Manager Assets.
1. In het veld **[!UICONTROL Navigation URL]** vult het systeem automatisch de URL van de navigatie. Deze alleen-lezen URL wordt gebruikt om vanuit [!DNL Experience Manager] snel toegang te krijgen tot de [!UICONTROL Main Menu] -instantie van uw organisatie.
1. Kies een gegevensopslagruimte in het vervolgkeuzemenu **[!UICONTROL [!DNL Experience Manager] Assets repository]** . Het systeem vult automatisch alle [!DNL Experience Manager] opslagplaatsen in die zijn gekoppeld aan de organisatie-id waaraan uw gebruikersprofiel is toegewezen.
   ![&#x200B; kies de bewaarplaats van de ervaringsmanager &#x200B;](assets/setup-information.png)

1. Klik **[!UICONTROL Save]** of beweging op [&#x200B; de meta-gegevens van de Opstelling (Facultatieve) &#x200B;](#set-up-metadata-optional) sectie in dit artikel.

   >[!NOTE]
   >
   >Vanwege de complexiteit van de integratie kunt u de repository niet wijzigen nadat u de eerste configuratie hebt opgeslagen.

## Metagegevens instellen (optioneel)

U kunt [!DNL Workfront] -objectgegevens toewijzen aan middelenmediavelden in [!DNL Experience Manager] Assets.

>[!IMPORTANT]
>
>U kunt metagegevens slechts in één richting toewijzen: van [!DNL Workfront] tot [!DNL Experience Manager] . Metagegevens voor documenten die zijn gekoppeld aan [!DNL Workfront] vanuit [!DNL Experience Manager] kunnen niet worden overgebracht naar [!DNL Workfront] .

### Metagegevensvelden configureren

Voordat u metagegevensvelden gaat toewijzen, moet u metagegevensvelden zowel in Workfront als in Experience Manager Assets configureren.

U kunt als volgt metagegevensvelden configureren:

1. Vorm een meta-gegevensschema in [!DNL Experience Manager Assets] zoals die in [&#x200B; wordt verklaard vormt activa meta-gegevensafbeelding tussen Adobe  [!DNL Workfront]  en  [!DNL Experience Manager Assets] &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


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

Voor meer informatie over markeringen in Experience Manager Assets, met inbegrip van hoe te om markeringen tot stand te brengen en te beheren, zie [&#x200B; het Beheer Markeringen &#x200B;](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags).

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
1. Klik [!UICONTROL Save] of beweging op de [&#x200B; sectie van de Werkschema&#39;s van de Opstelling &#x200B;](#set-up-workflows-optional) in dit artikel.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Workflows instellen (optioneel)

Een werkstroom is een reeks acties die Workfront verbinden met Adobe Experience Manager as a Cloud Service. Als Workfront-beheerder kunt u workflows configureren in Workfront en deze vervolgens toewijzen aan projectsjablonen.

Wanneer een Project wordt gecreeerd gebruikend een Malplaatje van het Project waaraan een werkschema wordt toegewezen, worden de acties die in het werkschema worden bepaald teweeggebracht.

Workflows worden ingeschakeld en geconfigureerd voor de Adobe Experience Manager als geheel. Deze werkschema&#39;s kunnen dan op projectmalplaatjes worden toegepast. Zij kunnen op het malplaatjeniveau, of op het projectniveau worden aangepast of worden aangepast wanneer een project van dat malplaatje wordt gecreeerd.

De volgende workflows zijn beschikbaar in de Adobe Experience Manager-integratie:

* [Gekoppelde Adobe Experience Manager-mappen maken](#create-adobe-experience-manager-linked-folders)
* [Elementen publiceren die naar Adobe Experience Manager Assets worden verzonden](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Gekoppelde Adobe Experience Manager-mappen maken

U kunt maximaal 100 gekoppelde mappen per mappenstructuur maken.

1. Schakel **[!UICONTROL Create Linked folder]** in.
1. Voer een naam in voor de gekoppelde map die u maakt.
1. (Voorwaardelijk) laat de **optie Standaard van de omslagboom** toe als u deze verbonden omslag de standaardomslag voor projecten wilt zijn die met malplaatjes worden gecreeerd die deze integratie gebruiken. U kunt een of meer standaardmappen selecteren.
1. Kies een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.
1. (Voorwaardelijk) Ga als volgt te werk om een mapstructuur (geneste mappen) aan deze integratie toe te voegen:

   1. Klik **toevoegen omslag** pictogram ![&#x200B; omslag &#x200B;](assets/add-folder-aem.png) toevoegt.
   1. Op het **het type van Naam** gebied, selecteer hoe u de omslag wilt noemen:

      * **Naam**: Type in een naam voor de omslag.
      * **gegevens van Objecten**: Selecteer de bron voor de omslagnaam, zoals de naam van het Project.

      >[!NOTE]
      >
      >* Mapnamen moeten uit minder dan 100 tekens bestaan.
      >* De volgende tekens worden uit mapnamen verwijderd:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Om een genestelde omslag aan de omslagboom toe te voegen, klik het drie-punt menu naast de omslag u een genestelde omslag binnen wilt creëren en **selecteren voegt Omslag** toe. Vul de velden in zoals wordt beschreven in Stap de vorige stap.
   1. Om een omslag aan Workfront te verbinden, selecteer de omslag en klik **maak verbonden omslag**   pictogram ![&#x200B; omslag van de Verbinding &#x200B;](assets/link-folder.png).
   1. (Facultatief) om een omslag uit te geven, selecteer de omslag en klik **uitgeven het pictogram van de Omslag** ![&#x200B; pictogram geeft pictogram &#x200B;](assets/edit-icon.png) uit.
   1. (Facultatief) om een omslag te schrappen, de omslag te selecteren en de **omslag van de Schrapping** pictogram ![&#x200B; omslag van de Schrapping &#x200B;](assets/delete-folder.png) te klikken.
1. (Voorwaardelijk) om een andere omslagboom toe te voegen, **+ voeg omslagboom** toe en volg de stappen in Stap 5.

1. Klik **[!UICONTROL Save]**, of beweging op [&#x200B; publiceer activa die naar de sectie van Adobe Experience Manager Assets &#x200B;](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) in dit artikel worden verzonden.


>[!NOTE]
>
>* De Inheemse Integratie van Workfront AEM kan **niet meer dan 100 omslagen per project per integratie** tot stand brengen, ongeacht hoeveel omslagbomen inbegrepen zijn.
>   * Voorbeeld: integratie met 4 mapstructuren in één project kan tot 100 mappen maken, niet 400.
>* De eerste map in elke mappenstructuur wordt automatisch gemarkeerd als gekoppeld aan Workfront. Als u deze map niet wilt koppelen, kunt u deze ontkoppelen.
>* Als er geen mapstructuur is opgegeven, wordt de hoofdmap de gekoppelde map.




### Elementen publiceren die naar Adobe Experience Manager Assets worden verzonden

1. Schakel **[!UICONTROL Publish assets automatically]** in.
1. Schakel het vakje naast de locatie in waar u de elementen wilt publiceren die naar Adobe Experience Manager-elementen zijn verzonden. U kunt een van beide of beide opties inschakelen.
1. (Voorwaardelijk) Als u de optie Brand Portal hebt ingeschakeld, selecteert u de Brand Portal waar u elementen wilt publiceren.
1. Klik **[!UICONTROL Save]** of beweging op de [&#x200B; Opstelling verbonden omslagen (Facultatieve) &#x200B;](#set-up-linked-folders-optional) sectie in dit artikel.

## Gekoppelde mappen instellen (optioneel)

U kunt gebruikers toestaan om mappen te maken die gekoppeld zijn aan [!DNL Experience Manager] terwijl ze zich in een [!DNL Workfront] -project bevinden. Wanneer een map is gekoppeld, worden alle aan de map toegevoegde middelen automatisch weergegeven in zowel [!DNL Workfront] als [!DNL Experience Manager] . Wanneer een element voor het eerst in [!DNL Workfront] aan de gekoppelde map wordt toegevoegd, worden de metagegevens van het element doorgegeven aan [!DNL Experience Manager Assets] .

In de onderstaande stappen geeft u aan waar u de gekoppelde mappen wilt maken. Elke integratie kan slechts één locatie voor alle gekoppelde mappen hebben.

Gekoppelde mappen instellen:

1. Schakel **[!UICONTROL Enable Linked folder]** in.
1. Kies een mappad om aan te geven waar u alle gekoppelde mappen aan deze integratie wilt koppelen.

   >[!NOTE]
   >
   >Gebruikers moeten in [!DNL Adobe Experience Manager Assets] schrijftoegang hebben tot de opgegeven map om een gekoppelde map te maken.

1. Klik op **[!UICONTROL Save]**.
