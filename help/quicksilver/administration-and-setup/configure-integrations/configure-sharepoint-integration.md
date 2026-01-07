---
title: Vorm de  [!DNL SharePoint]  Integratie
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: U kunt  [!DNL Workfront]  met  [!DNL SharePoint]  Online integreren, die gebruikers van de capaciteit voorzien om aan te navigeren, te verbinden, en  [!DNL SharePoint]  documenten binnen Workfront toe te voegen. De verstrekte functionaliteit is gelijkaardig aan dat van andere  [!DNL Workfront]  documentintegratie.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1671'
ht-degree: 0%

---

# De integratie met [!DNL SharePoint] configureren

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>De nieuwe [!DNL SharePoint] -integratie is vrijgegeven voor productie met de release van 22.3 (juli 2022).
>
>* Hoewel uw gebruikers nog steeds toegang hebben tot documenten die via de verouderde [!DNL SharePoint] integratie zijn gekoppeld, kunnen ze er geen documenten doorheen koppelen. ze moeten de nieuwe [!DNL SharePoint] -integratie gebruiken om documenten uit SharePoint te koppelen.
>
>* Als u geen bestaande SharePoint-integratie hebt geconfigureerd, kunt u deze niet toevoegen. U moet de nieuwe SharePoint-integratie gebruiken om documenten aan SharePoint te koppelen.
>
>* Voor de nieuwe SharePoint-integratie is mogelijk geen configuratie van een beheerder vereist en deze kan door individuele gebruikers worden ingesteld. Voor een vloeiende overgang naar de nieuwe SharePoint-integratie moet een Workfront-beheerder echter kleine wijzigingen aanbrengen in het gedeelte Workfront Setup.
>
>    Voor informatie en instructies, zie [ de integratie van erfenisSharePoint voor voortdurende toegang tot documenten ](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in dit artikel vormen.
>    
>* We raden gebruikers aan documenten te koppelen die momenteel via de verouderde [!DNL SharePoint] -integratie aan elkaar zijn gekoppeld.
>    
>    Voor instructies bij het verbinden van documenten, zie [ documenten van de Verbinding van externe toepassingen ](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

U kunt [!DNL Workfront] integreren met [!DNL SharePoint Online] , zodat gebruikers in Workfront kunnen navigeren naar documenten van het type [!DNL SharePoint] , deze kunnen koppelen en toevoegen. De geleverde functionaliteit is vergelijkbaar met die van andere [!DNL Workfront] -integraties, zoals [!DNL Google Drive] , [!DNL Box] en [!DNL Dropbox] .

Deze integratie is alleen compatibel met [!DNL SharePoint Online] . Op-premise instanties van [!DNL SharePoint] worden niet ondersteund.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een Workfront-beheerder zijn. </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet over de benodigde toegangsrechten of machtigingen in [!DNL SharePoint] beschikken om uw [!DNL SharePoint] -integratie te wijzigen of te configureren.

## Documenten koppelen via de nieuwe SharePoint-integratie

Individuele gebruikers kunnen documenten koppelen via de nieuwe [!DNL SharePoint] -integratie. Voor de integratie is geen beheerdersconfiguratie vereist. In plaats daarvan meldt de gebruiker zich bij het koppelen van een document aan zijn [!DNL Microsoft] -account. Hierdoor heeft de integratie toegang tot documenten die beschikbaar zijn in het [!DNL SharePoint] -bestand van de gebruiker.

De eerste keer dat een gebruiker de [!DNL Workfront] [!DNL SharePoint] -integratie verbindt met zijn [!DNL SharePoint] -account, ziet en accepteert hij alle machtigingen die [!DNL Workfront] gebruikt bij interactie met zijn [!UICONTROL SharePoint] -account, of kan hij of zij rechten aanvragen bij zijn of haar Microsoft-beheerder. Met leesmachtigingen kan [!DNL Workfront] bestanden weergeven en openen op [!DNL SharePoint] en met schrijfmachtigingen kan de gebruiker bestanden uploaden naar [!DNL SharePoint] .

![ toestemmingen van SharePoint ](assets/sharepoint-permissions.png)

Voor instructies bij het verbinden van documenten door de nieuwe [!DNL SharePoint] integratie, zie [ Verbinding een extern document aan  [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* Afhankelijk van de Microsoft-configuratie van de organisatie kunnen gebruikers de pagina &quot;Goedkeuring vereist&quot; zien in plaats van de pagina &quot;Machtigingen aangevraagd&quot;. In dit geval kunnen de gebruikers deze pagina gebruiken om aan te vragen dat de beheerder van Microsoft van de organisatie toestemmingen aan de integratie van SharePoint verleent.
>
>* Een [!DNL SharePoint] -integratie kan verbinding maken met één [!DNL SharePoint] -instantie. Daarom kan een gebruiker een integratie instellen voor één [!DNL SharePoint] , maar niet voor een tweede [!DNL SharePoint] , zelfs als deze rechten en documenten voor de tweede [!DNL SharePoint] heeft.
>
>* Een gebruiker heeft via de [!DNL Workfront] [!DNL SharePoint] -integratie toegang tot dezelfde sites, verzamelingen, mappen, submappen en bestanden als in zijn [!DNL SharePoint] -account.

### Documenten van SharePoint koppelen

Voor instructies bij het verbinden van documenten van SharePoint door de nieuwe [!DNL SharePoint] integratie, zie [ Verbinding een extern document aan  [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Documenten naar SharePoint verzenden

Een document naar SharePoint verzenden:

1. Klik **verzenden naar** pictogram ![ verzenden naar ](assets/send-to-icon.png) en selecteren SharePoint (Grafiek API).
1. (Optioneel) Zoek in de zoekbalk naar de site of map waarnaar u het document wilt verzenden.
1. Selecteer de site of map in de lijst.

   * De plaatsen zijn duidelijk met ![ pictogram van de Plaats ](assets/site-icon.png).

   * De omslagen zijn duidelijk met ![ pictogram van de Omslag ](assets/folder-icon.png).

   * Bestanden zijn niet gemarkeerd met een pictogram.

1. Klik **sparen**.


## Informatie over beveiliging, toegang en autorisatie voor de [!DNL SharePoint] -integratie

### Verificatie en autorisatie

[!DNL Workfront] gebruikt OAuth2 om een toegangstoken terug te winnen en een vernieuwingstoken. Dit toegangstoken wordt gebruikt voor autorisatie met alle [!DNL SharePoint] gebieden.

### Toegang en machtigingen

De eerste keer dat een gebruiker een document toevoegt aan [!DNL Workfront] vanuit [!DNL SharePoint] , wordt de gebruiker doorgestuurd naar de aangevraagde pagina met machtigingen, waar hij of zij rechten kan verlenen voor de integratie met SharePoint.

>[!NOTE]
>
>Afhankelijk van de Microsoft-configuratie van de organisatie kunnen gebruikers de pagina &quot;Goedkeuring vereist&quot; zien in plaats van de pagina &quot;Machtigingen aangevraagd&quot;. In dit geval kunnen de gebruikers deze pagina gebruiken om aan te vragen dat de beheerder van Microsoft van de organisatie toestemmingen aan de integratie van SharePoint verleent.

De volgende machtigingen worden aangevraagd:

| Toegang | Reden |
|---|---|
| Volledige toegang tot uw bestanden | Hiermee krijgt [!DNL Workfront] toegang tot de bestanden van een gebruiker om elementen te koppelen. Wanneer documenten van [!DNL Workfront] naar [!DNL SharePoint] worden verzonden, vereist [!DNL Workfront] toegang om het element te maken. |
| Items in alle siteverzamelingen lezen | Hiermee staat u [!DNL Workfront] toe om elementen te lezen die gebruikersnavigatie mogelijk maken. |
| Items in alle siteverzamelingen bewerken of verwijderen | Hiermee staat u [!DNL Workfront] toe elementen te maken in sites en siteverzamelingen. Verwijderen wordt alleen gebruikt bij opschonen nadat de koppelingen zijn verbroken. |
| Toegang behouden tot gegevens die u toegang hebt verleend aan | Hiermee staat u [!DNL Workfront] toe een vernieuwingstoken te genereren. |
| Aanmelden en gebruikersprofiel lezen | Staat [!DNL Workfront] toe om het toegangstoken te gebruiken om van naam van de gebruiker, door de OAuth2 login stroom te handelen. |

* Deze toegang wordt verleend door de gebruiker de eerste keer zij de integratie gebruiken, en kan op elk ogenblik worden ingetrokken.
* De toestemmingen die voor deze integratie worden gevraagd zijn **gemachtigde** toestemmingen.
* [!DNL Workfront] vraagt om de minimale toegang die vereist is om bewerkingen in de integratie uit te voeren.
* De toegang tot het weergeven, bewerken of verwijderen van een [!DNL Adobe Workfront] -document dat is gekoppeld aan [!DNL SharePoint] , is gebaseerd op de toegang van de gebruiker in [!DNL Workfront] . Voor elke navigatie, download of bewerking van een [!DNL SharePoint] -bestand of -map is echter toegang tot [!DNL SharePoint] vereist. De toegang tot deze handelingen wordt beheerd door [!DNL SharePoint] .
* Gebruikers kunnen miniaturen en voorvertoningen weergeven van afbeeldingen die zijn opgehaald uit [!DNL SharePoint] . Ook kunnen ze bestands- en mapnamen weergeven in [!DNL SharePoint] zonder zich aan te melden bij [!DNL SharePoint] .
* De toegangstoken van een gebruiker wordt slechts gebruikt wanneer de gebruiker off-line is en een andere gebruiker de inhoud van een omslag bekijkt die met [!DNL Workfront] wordt verbonden. Het toegangstoken wordt gebruikt om te ontdekken of om het even welke documenten in de omslag zijn toegevoegd, verwijderd, of uitgegeven.

### Beveiliging

Alle communicatie tussen [!DNL Workfront] en [!DNL SharePoint] vindt plaats via HTTPS, waarmee de informatie wordt versleuteld.

[!DNL Workfront] slaat, kopieert of dupliceert geen gegevens van [!DNL SharePoint] op. De enige uitzondering hierop is dat in [!DNL Workfront] miniaturen worden opgeslagen vanuit [!DNL SharePoint] om deze weer te geven in de lijstweergave en in Voorvertoning.

Als een element voor het eerst naar [!DNL Workfront] is geüpload en vervolgens naar [!DNL SharePoint] wordt verzonden, behoudt [!DNL Workfront] de gegevens voor het eerste bestand omdat gebruikers een vorige versie van een [!DNL Workfront] -document kunnen downloaden. Als een document is gemaakt in [!DNL SharePoint] , slaat [!DNL Workfront] die bestandsgegevens niet op.

## De verouderde [!DNL SharePoint] integratie configureren voor continue toegang tot documenten

Om ervoor te zorgen dat uw gebruikers via de verouderde [!DNL SharePoint] -integratie voortdurend toegang hebben tot documenten die aan Workfront zijn gekoppeld, moet u de toegang tot de verouderde [!DNL SharePoint] -integratie opnieuw configureren en de SharePoint Client Secret up-to-date houden.

* [Herzie toegang tot de erfenis  [!DNL SharePoint]  integratie](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Vorm het Geheim van de Cliënt voor voortdurende toegang tot de erfenis  [!DNL SharePoint]  integratie](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Toegang tot de verouderde [!DNL SharePoint] integratie opnieuw configureren

Door de verouderde [!DNL SharePoint] integratie opnieuw te configureren, hebben gebruikers toegang tot documenten die via de verouderde [!DNL SharePoint] -integratie zijn gekoppeld, terwijl ze er zeker van zijn dat uw gebruikers geen nieuwe documenten via die integratie kunnen koppelen.

>[!NOTE]
>
> * De oudere [!DNL SharePoint] integratie wordt geëtiketteerd &quot;[!DNL SharePoint]&quot;.
> * De nieuwe [!DNL SharePoint] integratie wordt geëtiketteerd &quot;[!UICONTROL [!DNL SharePoint] (Graph API)]&quot;.

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Selecteer **[!UICONTROL Documents]** in de linkernavigatie en selecteer vervolgens **[!UICONTROL Cloud Providers]** .
1. Zorg ervoor dat de optie **[!DNL SharePoint]** en **[!UICONTROL [!DNL SharePoint] (Graph API)]** beide zijn ingeschakeld.
1. Klik op **[!UICONTROL Save]**.
1. Selecteer **[!UICONTROL Documents]** in de linkernavigatie en selecteer vervolgens **[!UICONTROL [!DNL SharePoint] Integration]** .
1. Selecteer links van de lijst het vinkje voor alle bestaande integratie en selecteer vervolgens **[!UICONTROL Disable]** .



### Configureer het clientgeheim voor continue toegang tot de oudere [!DNL SharePoint] -integratie

Uw [!DNL SharePoint] clientgeheim verloopt één keer per jaar. Om ervoor te zorgen dat u toegang kunt blijven houden tot de documenten in uw verouderde [!DNL SharePoint] integratie, moet u de [!DNL SharePoint] Client Secret up-to-date houden.

>[!IMPORTANT]
>
> Omdat [!DNL SharePoint] Client Secrets wordt afgehandeld door [!DNL Microsoft] , kunnen de functies en procedures van Client Secret veranderen op basis van updates van [!DNL SharePoint] die door [!DNL Microsoft] zijn gemaakt. Raadpleeg altijd de documentatie bij [!DNL Microsoft] voor de meest recente informatie over procedures en functies in [!DNL SharePoint] .

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Produceer een nieuw cliëntgeheim zoals die in [ wordt beschreven Vervang een het verlopen cliëntgeheim in a  [!DNL SharePoint]  toe:voegen-binnen ](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Kopieer dit clientgeheim naar een beveiligde locatie.
1. Meld u aan bij [!DNL Workfront] als beheerder.
1. In Workfront, klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Setup]** ![ pictogram van de Opstelling ](/help/_includes/assets/gear-icon-setup.png).
1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]** .
1. Klik op de [!DNL SharePoint] -integratie die u wilt bijwerken en klik vervolgens op **[!UICONTROL Edit]** .
1. Bepaal de plaats van de **sectie van Info van de Verbinding** van het het uitgeven venster, dan ga het nieuwe Geheim van de Cliënt in het **[!UICONTROL SharePoint Client Secret]** gebied in.
1. Klik op **[!UICONTROL Save]**.

<!--

## Instructions for setting up the legacy SharePoint integration

>[!IMPORTANT]
>
>This integration has been deprecated. The instructions here are for information only and will be removed in the near future.


Workfront connects to [!DNL SharePoint] Online using OAuth 2.0, a standard used by most web-based integrations for the authentication and authorization of users.

To configure OAuth, you need to create a [!DNL SharePoint] site and a Site App within [!DNL SharePoint]. This process is described in the following sections.

For more information about OAuth, see [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>To make it easy to copy and paste information between [!DNL Workfront] and [!DNL SharePoint] in these steps, we recommend keeping both applications open in separate tabs.

* [Create and configure a [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site) 
* [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app) 
* [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance) 
* [Complete your integration](#complete-your-integration) 
* [Add documents](#add-documents)

### Create and configure a [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

In order for [!DNL Workfront] to authenticate with [!DNL SharePoint], [!DNL Workfront] ca use a master site where users have the [!UICONTROL Full Control] permission level or specific Manage permissions. This master site acts as an Authentication Entry Point for [!DNL Workfront].

To create and configure a [!DNL SharePoint] Site:

1. (Optional) If you do not want to use your organization's root site, you can create a master site in [!DNL SharePoint].

   For instructions, visit [Create a site](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in the [!DNL Microsoft] Documentation.

   * Select the **[!UICONTROL Team Site]** option when creating the site.

1. (Conditional) If you created a site in step 1, go to the site you just created.

   Or

   If you did not create a site in step 1, go to your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client ID. Copy this ID to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Click <strong>[!UICONTROL Generate]</strong> to generate a Client Secret. Copy this Secret to a secure location. You will use it later when you set up the [!DNL SharePoint] integration in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Title</p> </td> 
      <td> <p>Enter a title, such as [!DNL Workfront] Site App. Users see this title when adding documents..</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Redirect URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**
1. Continue to [Grant write permissions to the site app](#grant-write-permissions-to-the-site-app).

### Grant write permissions to the site app  {#grant-write-permissions-to-the-site-app}

At this point, you have successfully created a Site App and registered it within [!DNL Workfront]. This site app is also known as an app principal in [!DNL SharePoint]. It resides within your tenant. New site apps do not automatically have access to site collections within the tenant. Permissions must be granted explicitly, for each site collection. The steps below will show you how to grant Write permission to the new Site App a site collection. Repeat these steps for each of the site collections you added under [!UICONTROL Visible Site Collections] in the steps above.

This site app must have [!UICONTROL Write] permission to any site collections that users need to access through [!DNL Workfront].

1. Add '/_layouts/15/appinv.aspx' to the URL in [!DNL Sharepoint].

   **Example:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. Configure the following fields

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Add the Client ID that you created in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>and click <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>These automatically fill when you click [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Copy the following XML to the [!UICONTROL Permission Request XML] field. Make sure that it is added exactly as shown without additional spaces etc. in order to avoid errors.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre><code><span style="color: #63a35c; ">&lt;AppPermissionRequests&gt;</span><br><span style="color: #63a35c; ">&lt;AppPermissionRequest <span style="color: #795da3; ">Scope</span><span style="color: #df5000; ">="http://sharepoint/content/sitecollection/web"</span> <span style="color: #795da3; ">Right</span><span style="color: #df5000; ">="Write"</span>/&gt;</span><br><span style="color: #63a35c; ">&lt;/AppPermissionRequests&gt;</span></code></pre> 
      </div> 
      </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**. 
1. In the dialog that appears, click **[!UICONTROL Trust it]**.
1. Verify that the site app has access to the site collection by clicking the **[!UICONTROL Site collection app permissions]** link in [!UICONTROL Site Settings].
1. Repeat the steps above for the remaining site collections, then continue with [Create a [!DNL Workfront] [!DNL SharePoint] integration instance](#create-a-workfront-sharepoint-integration-instance).

### Create a [!DNL Workfront] [!DNL SharePoint] integration instance {#create-a-workfront-sharepoint-integration-instance}

When you have created a site app in [!DNL SharePoint], you can now copy information from the site app into [!DNL Workfront]. The site app is an app principal and acts as the conduit through which OAuth requests are made to access documents within site collections.

1. Log into [!DNL Workfront] as an administrator.
1. Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![Gear settings icon](assets/gear-icon-settings.png).

1. In the left panel, click **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Click **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Enter a name for the [!DNL SharePoint] integration. Users see this name when they click [!UICONTROL Add] &gt; [!UICONTROL From] 'name of integration'. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Host Instance]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Access Domain]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>This refers to the Master Site that users will use to authenticate through. It is likely the same domain as the [!UICONTROL [!DNL SharePoint] Host Instance].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] Integration.
       <ul> 
        <li> <p><b>If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>Enter the URL stem for the site collection that you created in the section above.</p> <p>This is the section of the URL after .com.</p> <p>Example: for the URL <code>https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client ID]</td> 
      <td>Enter the Client ID that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client Secret]</td> 
      <td>Enter the Client Secret that you generated in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Create and configure a [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Important</b> Site collections are used only in the Legacy [!DNL SharePoint] integration.
       <ul> 
        <li> <p><b> If you are using your organization's root site</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>If you are using a master site and subsites:</b> </p> <p><b>IMPORTANT</b>: [!DNL Microsoft SharePoint] no longer recommends the use of subsites.</p> <p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p> <p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p> <p><b>NOTE</b>:   <p>If you want to test your configuration only (no subsites), enter the stem of the master site. </p> <p>Example: for the URL <code> https://mycompany.sharepoint.com/sites/mysite</code>, the stem would be <code>/sites/mysite</code>.</p> <p>When you have tested your configuration as described in <a href="#complete-your-integration" class="MCXref xref">Complete your integration</a>, you must remove the master site and enter the subsites.</p> 
          <ol> 
           <li value="1">Click the <strong>[!UICONTROL Main Menu]</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of [!DNL Adobe Workfront], then click <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>In the left panel, click <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integration]</strong>.</p></li><li><p>Click the [!DNL SharePoint] integration you are setting up, then click Edit.</p></li><li><p>Delete the stem for the master site from the [!UICONTROL Visible Site Collections] field.</p></li><li><p>For each subsite you want to add to your [!DNL SharePoint] integration, enter the stem of the subsite.</p></li><p>Example: for the URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>, the stem would be <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Save]**
1. Continue to [Complete your integration](#complete-your-integration).

### Complete your integration {#complete-your-integration}

The basic configuration is almost complete.

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![Document icon](assets/document-icon.png).
1. Click **[!UICONTROL Add new]**.
1. Click **[!UICONTROL From] `<title of your [!DNL SharePoint] site>`** in the dropdown.

   A dialog that invites you to Trust this site appears.

   >[!NOTE]
   >
   >If this dialog does not appear, your [!DNL SharePoint] integration is not configured correctly.

1. Click **[!UICONTROL Trust it]**.

### Add documents {#add-documents}

You can now add documents from your [!DNL SharePoint] site.

For instructions, see [Link an external document to [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>If the user who linked a folder no longer has access to the external application, [!DNL Workfront] can no longer access the contents of the folder. This may happen, for example, if the user who originally linked the folder leaves the company. To ensure continued access, a user with access to the folder must re-link the folder.
> 

-->

## Problemen oplossen

* [ Probleem: De gebruikers ervaren op authentificatie-gebaseerde fouten wanneer het gebruiken van de  [!DNL SharePoint]  integratie.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [ Probleem: Wanneer het proberen om  [!DNL SharePoint]  dossiers in  [!DNL Workfront] te doorbladeren, zie ik geen of alle van mijn plaatsinzamelingen.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Probleem: ik heb geen toegang tot eerder verbonden omslagen en documenten in  [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Probleem: gebruikers ervaren op verificatie gebaseerde fouten bij het gebruik van de [!DNL SharePoint] -integratie. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Oplossingen:

Gebruikers moeten over de juiste machtigingen voor de [!DNL SharePoint] -site beschikken.

Gebruikers met [!UICONTROL Full Control] toegang hebben alle benodigde machtigingen voor uw [!DNL SharePoint] -integratie. Als u geen Volledige toegang van de Controle aan uw gebruikers wilt verlenen, moet u de volgende toestemmingen verlenen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Design]</p> </td> 
   <td> <p>Kan weergeven, toevoegen, bijwerken, verwijderen, goedkeuren en aanpassen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Edit]</p> </td> 
   <td> <p>Kan lijsten toevoegen, bewerken en verwijderen; kan lijstitems en documenten weergeven, toevoegen, bijwerken en verwijderen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>Kan lijstitems en documenten weergeven, toevoegen, bijwerken en verwijderen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL View only]</p> </td> 
   <td> <p>Pagina's, lijstitems en documenten kunnen worden weergegeven (documenttypen met bestandshandlers aan de serverzijde kunnen wel in de browser worden weergegeven, maar niet worden gedownload)</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor instructies bij het creëren van en het uitgeven van toestemmingsniveaus, zie [ hoe te tot toestemmingsniveaus ](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) in de documentatie van Microsoft leiden en uitgeven.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Probleem: wanneer ik probeer door [!DNL SharePoint] bestanden te bladeren in [!DNL Workfront] , zie ik geen of alle verzamelingen van mijn sites. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Oplossingen:

Als u een siteverzameling wilt weergeven in [!DNL Workfront] , moet aan de volgende voorwaarden worden voldaan:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* De gebruiker moet weergavetoegang hebben tot de siteverzameling in [!DNL SharePoint] .

  Controleer de machtigingen van de siteverzameling in SharePoint om dit in [!DNL SharePoint] te verifiëren.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Probleem: ik heb geen toegang tot eerder gekoppelde mappen en documenten in [!DNL SharePoint] . {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Oplossing:

Als de gebruiker die een map [!DNL SharePoint] heeft gekoppeld, niet langer kan worden geverifieerd, heeft [!DNL Workfront] geen toegang meer tot de inhoud van de map. Dit kan bijvoorbeeld gebeuren als de gebruiker die oorspronkelijk de map had gekoppeld het bedrijf verlaat.

Een gebruiker met toegang tot de map moet de map opnieuw koppelen om ervoor te zorgen dat hij of zij toegang kan blijven krijgen.

Voor informatie bij het verbinden van omslagen van externe leveranciers, zie [ documenten van de Verbinding van externe toepassingen ](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->
