---
title: Vorm [!DNL SharePoint] integratie
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: U kunt [!DNL Workfront] with [!DNL SharePoint] Online, die gebruikers de capaciteit verstrekken om aan te navigeren, te verbinden, en toe te voegen [!DNL SharePoint] documenten in Workfront. De opgegeven functionaliteit is vergelijkbaar met die van andere [!DNL Workfront] documentintegratie.
author: Becky
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '1541'
ht-degree: 0%

---

# Vorm [!DNL SharePoint] integratie

<!--Audited: 12/2023-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>De nieuwe [!DNL SharePoint] de integratie werd vrijgegeven voor de productie met de release van 22.3 (juli 2022). Hoewel uw gebruikers nog steeds toegang hebben tot documenten die via de verouderde [!DNL SharePoint] integratie moeten zij de nieuwe [!DNL SharePoint] integratie om documenten uit SharePoint te koppelen.
>
>* De nieuwe integratie van SharePoint vereist geen configuratie door een beheerder, en kan opstelling door individuele gebruikers zijn. Voor een vloeiende overgang naar de nieuwe SharePoint-integratie moet een Workfront-beheerder echter kleine wijzigingen aanbrengen in het gedeelte Workfront Setup.
>
>    Zie voor meer informatie en instructies [De verouderde SharePoint-integratie configureren voor permanente toegang tot documenten](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in dit artikel.
>    
>* We raden gebruikers aan documenten te koppelen die momenteel via de verouderde versie zijn gekoppeld [!DNL SharePoint] integratie door de nieuwe integratie .
>    
>    Zie voor instructies over het koppelen van documenten [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

U kunt [!DNL Workfront] with [!DNL SharePoint Online], zodat gebruikers kunnen navigeren naar, koppelen en toevoegen [!DNL SharePoint] documenten in Workfront. De opgegeven functionaliteit is vergelijkbaar met die van andere [!DNL Workfront] integratie, zoals [!DNL Google Drive], [!DNL Box], en [!DNL Dropbox].

Deze integratie is alleen compatibel met [!DNL SharePoint Online]. Op locatie [!DNL SharePoint] worden niet ondersteund.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>Nieuw: Standaard <p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td>U moet een [!DNL Workfront] beheerder. </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Vereisten

U moet over de benodigde toegang of machtigingen beschikken in [!DNL SharePoint] om uw [!DNL SharePoint] integratie.

## Documenten koppelen via de nieuwe SharePoint-integratie

Individuele gebruikers kunnen documenten koppelen via de nieuwe [!DNL SharePoint] integratie. Voor de integratie is geen beheerdersconfiguratie vereist. In plaats daarvan meldt de gebruiker zich aan bij hun [!DNL Microsoft] account bij koppelen van een document, waardoor de integratie toegang heeft tot documenten die beschikbaar zijn in de [!DNL SharePoint].

De eerste keer dat een gebruiker verbinding maakt met de [!DNL Workfront] [!DNL SharePoint] integratie in hun [!DNL SharePoint] -account, kunnen ze alle machtigingen zien die [!DNL Workfront] gebruik bij interactie met hun [!UICONTROL SharePoint] account. Leesmachtigingen toestaan [!DNL Workfront] bestanden weergeven en openen op [!DNL SharePoint]en schrijfmachtigingen geeft de gebruiker de mogelijkheid bestanden te uploaden naar [!DNL SharePoint].

![Sharepoint-machtigingen](assets/sharepoint-permissions.png)

Voor instructies voor het koppelen van documenten via de nieuwe [!DNL SharePoint] integratie, zie [Een extern document koppelen aan [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] integratie kan verbinding maken met één [!DNL SharePoint] -instantie. Daarom kan een gebruiker een integratie instellen voor één [!DNL SharePoint], maar kan geen integratie instellen op een tweede [!DNL SharePoint], zelfs als ze over machtigingen beschikken voor en documenten hebben op de tweede [!DNL SharePoint].
>
>* Een gebruiker heeft toegang tot dezelfde sites, verzamelingen, mappen, submappen en bestanden via de [!DNL Workfront] [!DNL SharePoint] integratie zoals zij in hun [!DNL SharePoint] account.

### Documenten van SharePoint koppelen

Voor instructies voor het koppelen van documenten van SharePoint via de nieuwe [!DNL SharePoint] integratie, zie [Een extern document koppelen aan [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront).

### Documenten naar SharePoint verzenden

Een document naar SharePoint verzenden:

1. Klik op de knop **Verzenden naar** pictogram ![Verzenden naar](assets/send-to-icon.png) en selecteer SharePoint (Graph API).
1. (Optioneel) Zoek in de zoekbalk naar de site of map waarnaar u het document wilt verzenden.
1. Selecteer de site of map in de lijst.

   * Sites zijn gemarkeerd met ![Sitepictogram](assets/site-icon.png).

   * Mappen zijn gemarkeerd met ![Mappictogram](assets/folder-icon.png).

   * Bestanden zijn niet gemarkeerd met een pictogram.

1. Klikken **Opslaan**.


## Informatie over beveiliging, toegang en autorisatie voor de [!DNL SharePoint] integratie

### Verificatie en autorisatie

[!DNL Workfront] gebruikt OAuth2 om een toegangstoken terug te winnen en een te verfrissen teken. Dit toegangstoken wordt gebruikt voor vergunning met allen [!DNL SharePoint] gebieden.

### Toegang en machtigingen

De eerste keer dat een gebruiker een document toevoegt aan [!DNL Workfront] van [!DNL SharePoint], worden zij geleid aan het scherm dat om de volgende toestemmingen verzoekt:

| Toegang | Reden |
|---|---|
| Volledige toegang tot uw bestanden | Toestaan [!DNL Workfront] om de bestanden van een gebruiker te openen en elementen te koppelen. Wanneer documenten worden verzonden van [!DNL Workfront] tot [!DNL SharePoint], [!DNL Workfront] vereist toegang om het element te maken. |
| Items in alle siteverzamelingen lezen | Toestaan [!DNL Workfront] om elementen te lezen die gebruikersnavigatie mogelijk maken. |
| Items in alle siteverzamelingen bewerken of verwijderen | Toestaan [!DNL Workfront] om activa in plaatsen en plaatsinzamelingen te creëren. Verwijderen wordt alleen gebruikt bij opschonen nadat de koppelingen zijn verbroken. |
| Toegang behouden tot gegevens die u toegang hebt verleend aan | Toestaan [!DNL Workfront] om een vernieuwingstoken te produceren. |
| Aanmelden en gebruikersprofiel lezen | Toestaan [!DNL Workfront] om het toegangstoken te gebruiken om namens de gebruiker te handelen, door de OAuth2 login stroom. |

* Deze toegang wordt verleend door de gebruiker de eerste keer zij de integratie gebruiken, en kan op elk ogenblik worden ingetrokken.
* De voor deze integratie aangevraagde machtigingen zijn **gedelegeerd** machtigingen.
* [!DNL Workfront] vraagt om de minimumtoegang die wordt vereist om verrichtingen in de integratie uit te voeren.
* Toegang tot het weergeven, bewerken of verwijderen van [!DNL Adobe Workfront] document gekoppeld aan [!DNL SharePoint] is gebaseerd op de toegang van de gebruiker tot [!DNL Workfront]. Elke navigatie, download of bewerking van een [!DNL SharePoint] bestand of map vereist toegang tot [!DNL SharePoint]en de toegang tot deze acties wordt geregeld door [!DNL SharePoint].
* Gebruikers kunnen miniaturen en voorvertoningen weergeven die afkomstig zijn van [!DNL SharePoint]en kunt u bestands- en mapnamen zien in [!DNL SharePoint], zonder u aan te melden [!DNL SharePoint].
* De toegangstoken van een gebruiker wordt gebruikt slechts wanneer de gebruiker off-line is en een andere gebruiker de inhoud van een omslag bekijkt die met verbonden is [!DNL Workfront]. Het toegangstoken wordt gebruikt om te ontdekken of om het even welke documenten in de omslag zijn toegevoegd, verwijderd, of uitgegeven.

### Beveiliging

Alle communicatie tussen [!DNL Workfront] en [!DNL SharePoint] wordt uitgevoerd via HTTPS, waarmee de informatie wordt versleuteld.

[!DNL Workfront] gegevens niet opslaan, kopiëren of dupliceren van [!DNL SharePoint]. De enige uitzondering is dat: [!DNL Workfront] slaat miniaturen op van [!DNL SharePoint] in de lijstweergave en in Voorvertoning.

Als een element voor het eerst is geüpload naar [!DNL Workfront]en vervolgens verzonden naar [!DNL SharePoint], [!DNL Workfront] behoudt de gegevens voor het eerste bestand omdat gebruikers een vorige versie van een [!DNL Workfront] document. Als er een document is gemaakt in [!DNL SharePoint], [!DNL Workfront] slaat die bestandsgegevens niet op.

## De nalatenschap configureren [!DNL SharePoint] integratie voor verdere toegang tot documenten

Om ervoor te zorgen dat uw gebruikers via de veroudering toegang hebben tot documenten die aan Workfront zijn gekoppeld [!DNL SharePoint] integratie, moet u toegang tot de erfenis opnieuw vormen [!DNL SharePoint] en de SharePoint Client Secret up-to-date houden.

* [Toegang tot de nalatenschap opnieuw configureren [!DNL SharePoint] integratie](#reconfigure-access-to-the-legacy-sharepoint-integration)
* [Vorm het Geheim van de Cliënt voor verdere toegang tot de erfenis [!DNL SharePoint] integratie](#configure-the-client-secret-for-continued-access-to-the-legacy-sharepoint-integration)

### Toegang tot de nalatenschap opnieuw configureren [!DNL SharePoint] integratie

De nalatenschap opnieuw configureren [!DNL SharePoint] met integratie hebben uw gebruikers toegang tot documenten die via de verouderde [!DNL SharePoint] integratie, terwijl het ervoor zorgen dat uw gebruikers geen nieuwe documenten door die integratie kunnen verbinden.

>[!NOTE]
>
> * De nalatenschap [!DNL SharePoint] integratie is gelabeld &quot;[!DNL SharePoint].&quot;
> * De nieuwe [!DNL SharePoint] integratie is gelabeld &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Selecteren **[!UICONTROL Documents]** in de linkernavigatie selecteert u vervolgens **[!UICONTROL Cloud Providers]**.
1. Zorg ervoor dat de **[!DNL SharePoint]** en **[!UICONTROL [!DNL SharePoint] (Graph API)]** beide opties zijn ingeschakeld.
1. Klik op **[!UICONTROL Save]**.
1. Selecteren **[!UICONTROL Documents]** in de linkernavigatie selecteert u vervolgens **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Selecteer het vinkje links in de lijst voor alle bestaande integratie en selecteer vervolgens **[!UICONTROL Disable]**.
   ![](assets/disable-old-sharepoint.png)


### Vorm het Geheim van de Cliënt voor verdere toegang tot de erfenis [!DNL SharePoint] integratie

Uw [!DNL SharePoint] Clientgeheim verloopt één keer per jaar. Om ervoor te zorgen dat de documenten in uw verouderde [!DNL SharePoint] integratie, moet u zijn [!DNL SharePoint] Clientgeheim bijgewerkt.

>[!IMPORTANT]
>
> Omdat [!DNL SharePoint] Clientgeheimen worden verwerkt door [!DNL Microsoft], de functies en procedures van de clientgeheim kunnen worden gewijzigd op basis van updates van [!DNL SharePoint] gemaakt door [!DNL Microsoft]. Controleer altijd de [!DNL Microsoft] documentatie voor de meest recente informatie over procedures en kenmerken in [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Een nieuw clientgeheim genereren zoals beschreven in [Een verlopen clientgeheim vervangen in een [!DNL SharePoint] Add-in](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret).
1. Kopieer dit clientgeheim naar een beveiligde locatie.
1. Aanmelden [!DNL Workfront] als beheerder.
1. Klik in Workfront op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).
1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klik op de knop [!DNL SharePoint] integratie die u wilt bijwerken, en klik dan **[!UICONTROL Edit]**.
1. Zoek de **Verbindingsinfo** sectie van het het uitgeven venster, dan ga het nieuwe Geheim van de Cliënt in **[!UICONTROL SharePoint Client Secret]** veld.
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
1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

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

1. In Workfront, Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Documents]** ![](assets/document-icon.png).
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

* [Probleem: gebruikers ervaren op verificatie gebaseerde fouten bij het gebruik van de [!DNL SharePoint] integratie.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Probleem: tijdens het bladeren [!DNL SharePoint] bestanden in [!DNL Workfront], ik zie geen van mijn plaatsinzamelingen of al mijn plaatsinzamelingen.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Probleem: ik heb geen toegang tot eerder gekoppelde mappen en documenten in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Probleem: gebruikers ervaren op verificatie gebaseerde fouten bij het gebruik van de [!DNL SharePoint] integratie. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Oplossingen:

Gebruikers moeten over de juiste machtigingen beschikken om [!DNL SharePoint] site.

Gebruikers met [!UICONTROL Full Control] toegang heeft alle noodzakelijke toestemmingen voor uw [!DNL SharePoint] integratie. Als u geen Volledige toegang van de Controle aan uw gebruikers wilt verlenen, moet u de volgende toestemmingen verlenen:

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

Zie voor instructies over het maken en bewerken van machtigingsniveaus [machtigingsniveaus maken en bewerken](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) in de documentatie van Microsoft.

<!--

### Problem: As a [!DNL Workfront] user, I am unable to provision a new [!DNL SharePoint] instance. When I attempt to do I see an error. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Solutions:

This can be caused by a number of things, originating in either [!DNL Workfront] or [!DNL SharePoint]'s configuration. Verify that:

* The Client ID, Client Secret, return URL and other configuration fields are correctly mapped between the [!DNL Workfront] [!DNL SharePoint] Integration instance and the [!DNL SharePoint] Site App.
* The user has [!UICONTROL Full Control] permission to the Site Collection used for authentication.
* The Site App is listed under [!UICONTROL Site App Permissions] for the [!UICONTROL Site Collection] used for authentication.

-->

### Probleem: tijdens het bladeren [!DNL SharePoint] bestanden in [!DNL Workfront], ik zie geen van mijn plaatsinzamelingen of al mijn plaatsinzamelingen. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Oplossingen:

Om een plaatsinzameling in te zien [!DNL Workfront]moet aan de volgende voorwaarden worden voldaan:

<!--

* The site collection must be registered in the [!DNL Workfront] [!DNL SharePoint] Integration instance.

  To verify this in [!DNL Workfront]:

   1. Go to [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Edit the [!DNL SharePoint] Integration instance information.
   1. Verify that the site collection is listed under [!UICONTROL Visible Site Collections].
   -->

* De gebruiker moet meningstoegang tot de plaatsinzameling in hebben [!DNL SharePoint].

  Om dit te verifiëren in [!DNL SharePoint], controleert u de machtigingen van de siteverzameling in SharePoint.

<!--* The [!DNL SharePoint] Site App must have access to the site collection.

  To verify this in [!DNL SharePoint]:

   1. Go to the site collection > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Ensure that the [!UICONTROL Site App] used by [!DNL Workfront] is listed here.
   1. (Conditional) If the Site App is not listed, add to the site collection using _layouts/15/appinv.aspx.

      For information about adding the site collection, see Granting Write Permissions To The Site App.
      
-->

### Probleem: ik heb geen toegang tot eerder gekoppelde mappen en documenten in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Oplossing:

Als de gebruiker die een koppeling heeft gemaakt [!DNL SharePoint] map kan niet meer worden geverifieerd, [!DNL Workfront] heeft geen toegang meer tot de inhoud van de map. Dit kan bijvoorbeeld gebeuren als de gebruiker die oorspronkelijk de map had gekoppeld het bedrijf verlaat.

Een gebruiker met toegang tot de map moet de map opnieuw koppelen om ervoor te zorgen dat hij of zij toegang kan blijven krijgen.

Voor informatie over het koppelen van mappen van externe providers raadpleegt u [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

<!--

### Problem: I see a "404 not found" error when attempting to add a document from [!DNL Sharepoint]

#### Solution:

This error might occur if one of the sites configured in the [!UICONTROL Visible Site Collections] list has been deleted in Sharepoint. Check the [!UICONTROL Visible Site Collections] list, and remove any sites that have been deleted in Sharepoint.-->