---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Adobe Experience Manager Assets-integratie
description: U kunt uw werk verbinden met de volgende Integraties van Adobe Experience Manager Assets.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# Configureer de [!UICONTROL Experience Manager Assets as a Cloud Service] integratie

U kunt uw werk met uw inhoud verbinden in [!DNL Experience Manager Assets]&#x200B;:

* Elementen en metagegevens verschuiven vanuit [!DNL Adobe Workfront] tot [!DNL Experience Manager Assets]&#x200B;
* Elementen koppelen van [!DNL Experience Manager Assets] aan uw projecten en taken in [!DNL Workfront&#x200B;]
* Gebruiksgevallen voor versioning vereenvoudigen
* Mappen maken die zijn gekoppeld aan [!DNL Experience Manager Assets]
* Metagegevens bijhouden voor elementen en mappen
* Projectmetagegevens synchroniseren tussen [!DNL Workfront] en [!DNL Experience Manager Assets]


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

1. Een metagegevensschema configureren in [!DNL Experience Manager Assets] zoals uiteengezet in [Elementmetagegevenstoewijzing tussen Adobe configureren [!DNL Workfront] en [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
1. Aangepaste formuliervelden configureren in Workfront. [!DNL Workfront] beschikt over veel ingebouwde aangepaste velden die u kunt gebruiken. U kunt echter ook uw eigen aangepaste velden maken, zoals wordt uitgelegd in [Een aangepast formulier maken of bewerken](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Activa

Metagegevens worden toegewezen wanneer een element wordt verschoven van [!DNL Workfront] voor het eerst. Documenten met de ingebouwde of aangepaste velden worden automatisch toegewezen aan de opgegeven velden wanneer een element voor het eerst wordt verzonden naar [!DNL Experience Manager Assets].

>[!NOTE]
>
>Deze integratie ondersteunt geen aangepaste metagegevens van [!DNL Adobe Experience Manager].

Metagegevens toewijzen voor elementen:

1. Selecteren **[!UICONTROL Assets]** boven de tabel met metagegevens.
1. In de **[!UICONTROL [!DNL Workfront] field]** kiest u een ingebouwd of aangepast Workfront-veld.

   >[!NOTE]
   >
   >U kunt één kaart toewijzen [!DNL Workfront] veld naar meerdere [!UICONTROL Experience Manager Assets] velden. U kunt geen meerdere toewijzen [!DNL Workfront] velden naar één [!DNL Experience Manager Assets] veld.

1. In de [!DNL Experience Manager Assets] , doorzoeken in de vooraf ingevulde categorieën of ten minste twee letters invoeren in het zoekveld voor toegang tot extra categorieën.
1. Herhaal stap 2 en 3 zo nodig.
   ![metagegevensvelden](assets/asset-metadata.png)
1. Klikken [!UICONTROL Save] of ga naar de [Mappen](#folders) in dit artikel.

### Mappen

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
1. Klik op Opslaan of ga naar het dialoogvenster [Gekoppelde mappen instellen (optioneel)](#set-up-linked-folders-optional) in dit artikel.

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
