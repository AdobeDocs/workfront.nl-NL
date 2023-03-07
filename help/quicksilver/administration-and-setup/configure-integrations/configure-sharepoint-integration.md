---
title: Configureer de [!DNL SharePoint] integratie
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: U kunt [!DNL Workfront] with [!DNL SharePoint] Online, die gebruikers de capaciteit verstrekken om aan te navigeren, te verbinden, en toe te voegen [!DNL SharePoint] documenten in Workfront. De opgegeven functionaliteit is vergelijkbaar met die van andere [!DNL Workfront] integratie, zoals Google Drive, Box en Dropbox.
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 15aa025c9a35e30867f942047ec1989fdd6834e5
workflow-type: tm+mt
source-wordcount: '2353'
ht-degree: 0%

---

# De veroudering configureren [!DNL SharePoint] integratie

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>De nieuwe [!DNL SharePoint] de integratie werd vrijgegeven voor de productie met de release van 22.3 (juli 2022). Hoewel uw gebruikers nog steeds toegang hebben tot documenten die via de verouderde [!DNL SharePoint] de nieuwe [!DNL SharePoint] integratie om documenten uit SharePoint te koppelen.
>
>* Voor de nieuwe SharePoint-integratie is geen configuratie door een beheerder vereist en deze kan door individuele gebruikers worden ingesteld. Voor een vloeiende overgang naar de nieuwe SharePoint-integratie moet een Workfront-beheerder echter kleine wijzigingen aanbrengen in het gedeelte Workfront Setup.
   >
   >    Zie voor meer informatie en instructies [De verouderde SharePoint-integratie configureren voor permanente toegang tot documenten](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) in dit artikel.
>    
>* We raden gebruikers aan documenten te koppelen die momenteel via de verouderde versie zijn gekoppeld [!DNL SharePoint] integratie door de nieuwe integratie .
   >    
   >    Voor instructies over het koppelen van documenten raadpleegt u [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


U kunt [!DNL Workfront] with [!DNL SharePoint Online], zodat gebruikers kunnen navigeren naar, koppelen en toevoegen [!DNL SharePoint] documenten in Workfront. De opgegeven functionaliteit is vergelijkbaar met die van andere [!DNL Workfront] integratie, zoals [!DNL Google Drive], [!DNL Box], en [!DNL Dropbox].

Deze integratie is alleen compatibel met [!DNL SharePoint Online]. Instanties op locatie van [!DNL SharePoint] worden niet ondersteund.

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder. Voor informatie over [!DNL Workfront] beheerders, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Vereisten

U moet over de benodigde toegang of machtigingen beschikken in [!DNL SharePoint] om uw organisatie te wijzigen of te vormen [!DNL SharePoint].

## Documenten koppelen via de nieuwe SharePoint-integratie

Individuele gebruikers kunnen documenten koppelen via de nieuwe [!DNL SharePoint] integratie. Voor de integratie is geen beheerdersconfiguratie vereist. In plaats daarvan meldt de gebruiker zich aan bij hun [!DNL Microsoft] account bij koppelen van een document, waardoor de integratie toegang heeft tot documenten die beschikbaar zijn in de [!DNL SharePoint].

De eerste keer dat een gebruiker verbinding maakt met de [!DNL Workfront] [!DNL SharePoint] integratie in hun [!DNL SharePoint] -account, kunnen ze alle machtigingen zien die [!DNL Workfront] gebruik bij interactie met hun [!UICONTROL SharePoint] account. Leesmachtigingen toestaan [!DNL Workfront] om bestanden te bekijken en te openen op [!DNL SharePoint]en schrijfmachtigingen geeft de gebruiker de mogelijkheid bestanden te uploaden naar [!DNL SharePoint].

![Sharepoint-machtigingen](assets/sharepoint-permissions.png)

Voor instructies voor het koppelen van documenten via de nieuwe [!DNL SharePoint] integratie, zie [Een extern document koppelen aan [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] integratie kan verbinding maken met één [!DNL SharePoint] -instantie. Daarom kan een gebruiker een integratie instellen voor één [!DNL SharePoint], maar kan geen integratie instellen op een tweede [!DNL SharePoint], zelfs als ze over machtigingen beschikken voor en documenten hebben op de tweede [!DNL SharePoint].
>
>* Een gebruiker heeft toegang tot dezelfde sites, verzamelingen, mappen, submappen en bestanden via de [!DNL Workfront] [!DNL SharePoint] integratie zoals zij in hun [!DNL SharePoint] account.


## De verouderde SharePoint-integratie configureren voor permanente toegang tot documenten

Om ervoor te zorgen dat uw gebruikers toegang blijven houden tot documenten die zijn gekoppeld aan Workfront via de verouderde SharePoint-integratie, moet u de toegang tot de verouderde SharePoint-integratie opnieuw configureren en de SharePoint Client Secret up-to-date houden.

* [Toegang tot de nalatenschap opnieuw configureren [!DNL SharePoint] integratie](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [Vorm het Geheim van de Cliënt voor verdere toegang tot de erfenis [!DNL SharePoint] integratie](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### Toegang tot de nalatenschap opnieuw configureren [!DNL SharePoint] integratie

Om ervoor te zorgen dat u toegang krijgt tot documenten die via de verouderde [!DNL SharePoint] Voer de volgende procedure uit, zonder dat uw gebruikers nieuwe documenten via die integratie kunnen koppelen.

>[!NOTE]
>
> * De nalatenschap [!DNL SharePoint] integratie is gelabeld &quot;[!DNL SharePoint].&quot;
> * De nieuwe [!DNL SharePoint] integratie is gelabeld &quot;[!UICONTROL [!DNL SharePoint] (Graph API)].&quot;


1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Setup]** ![Instellen](../get-started-wf-administration/assets/gear-icon-settings.png).
1. Selecteren **[!UICONTROL Documents]** in de linkernavigatie selecteert u vervolgens **[!UICONTROL Cloud Providers]**.
1. Zorg ervoor dat de **[!DNL SharePoint]** en **[!UICONTROL [!DNL SharePoint] (Graph API)]** beide opties zijn ingeschakeld.
1. Klik op **[!UICONTROL Save]**.
1. Selecteren **[!UICONTROL Documents]** in de linkernavigatie selecteert u vervolgens **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Selecteer het vinkje links in de lijst voor alle bestaande integratie en selecteer vervolgens **[!UICONTROL Disable]**.


### Vorm het Geheim van de Cliënt voor verdere toegang tot de erfenis [!DNL SharePoint] integratie

Uw [!DNL SharePoint] Clientgeheim verloopt één keer per jaar. Om ervoor te zorgen dat de documenten in uw verouderde [!DNL SharePoint] integratie, moet u zijn [!DNL SharePoint] Clientgeheim bijgewerkt.

>[!IMPORTANT]
>
> Omdat [!DNL SharePoint] Clientgeheimen worden verwerkt door [!DNL Microsoft], de functies en procedures van de clientgeheim kunnen worden gewijzigd op basis van updates van [!DNL SharePoint] gemaakt door [!DNL Microsoft]. Controleer altijd de [!DNL Microsoft] documentatie voor de meest recente informatie over procedures en kenmerken in [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. Een nieuw clientgeheim genereren zoals beschreven in [Een verlopen clientgeheim vervangen in een [!DNL SharePoint] Add-in](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. Kopieer dit clientgeheim naar een beveiligde locatie.
1. Aanmelden [!DNL Workfront] als beheerder.
1. Klik in Workfront op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klik op de knop [!DNL SharePoint] integratie die u wilt bijwerken, en klik dan **[!UICONTROL Edit]**.
1. Voer het nieuwe clientgeheim in de **[!UICONTROL Client Secret]** veld.
1. Klik op **[!UICONTROL Save]**.



## Instructies voor het opzetten van de verouderde SharePoint-integratie

>[!IMPORTANT]
>
>Deze integratie is afgekeurd. De instructies hier zijn alleen ter informatie en worden in de nabije toekomst verwijderd.


Workfront maakt verbinding met [!DNL SharePoint] Online met OAuth 2.0, een standaard die door de meeste op het web gebaseerde integraties wordt gebruikt voor de verificatie en autorisatie van gebruikers.

Om OAuth te vormen, moet u tot een [!DNL SharePoint] site en een site-app binnen [!DNL SharePoint]. Dit proces wordt beschreven in de volgende secties.

Voor meer informatie over OAuth, zie [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>Om het gemakkelijk te maken om informatie tussen te kopiëren en te kleven [!DNL Workfront] en [!DNL SharePoint] in deze stappen, adviseren wij het houden van beide toepassingen open in afzonderlijke lusjes.

* [Een [!DNL SharePoint] site](#create-and-configure-a-sharepoint-site)
* [Schrijfmachtigingen verlenen aan de site-app](#grant-write-permissions-to-the-site-app)
* [Een [!DNL Workfront] [!DNL SharePoint] integratiefunctie](#create-a-workfront-sharepoint-integration-instance)
* [Voltooi uw integratie](#complete-your-integration)
* [Documenten toevoegen](#add-documents)

### Een [!DNL SharePoint] site  {#create-and-configure-a-sharepoint-site}

Om [!DNL Workfront] om te verifiëren met [!DNL SharePoint], [!DNL Workfront] kan een master site gebruiken waar gebruikers beschikken over [!UICONTROL Full Control] machtigingsniveau of specifieke beheermachtigingen. Deze master site fungeert als een verificatiepunt voor [!DNL Workfront].

Om een [!DNL SharePoint] Site:

1. (Optioneel) Als u de hoofdsite van uw organisatie niet wilt gebruiken, kunt u een master site maken in [!DNL SharePoint].

   Ga voor instructies naar [Een site maken](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) in de [!DNL Microsoft] Documentatie.

   * Selecteer **[!UICONTROL Team Site]** als u de site maakt.

1. (Voorwaardelijk) Als u in stap 1 een site hebt gemaakt, gaat u naar de site die u zojuist hebt gemaakt.

   of

   Als u in stap 1 geen site hebt gemaakt, gaat u naar de hoofdsite van uw organisatie.

1. Toevoegen `/_layouts/15/appregnew.aspx` aan het einde van de URL in de zoekbalk boven in het browservenster.
1. Configureer de volgende velden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client ID]</p> </td> 
      <td> <p>Klikken <strong>[!UICONTROL Generate]</strong> om een client-id te genereren. Kopieer deze id naar een veilige locatie. U gebruikt het later wanneer u de [!DNL SharePoint] integratie in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client Secret]</p> </td> 
      <td> <p>Klikken <strong>[!UICONTROL Generate]</strong> om een clientgeheim te genereren. Kopieer dit geheim naar een veilige locatie. U gebruikt het later wanneer u de [!DNL SharePoint] integratie in [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Titel</p> </td> 
      <td> <p>Voer een titel in, zoals [!DNL Workfront] Site-app. Gebruikers zien deze titel bij het toevoegen van documenten.</p> </td> 
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

1. Klik op **[!UICONTROL Create]**
1. Doorgaan naar [Schrijfmachtigingen verlenen aan de site-app](#grant-write-permissions-to-the-site-app).

### Schrijfmachtigingen verlenen aan de site-app  {#grant-write-permissions-to-the-site-app}

Op dit moment hebt u een Site-app gemaakt en deze geregistreerd binnen [!DNL Workfront]. Deze site-app wordt ook wel APP-principal genoemd in [!DNL SharePoint]. Het zit in je huurder. Nieuwe site-apps hebben niet automatisch toegang tot siteverzamelingen in de huurder. De toestemmingen moeten uitdrukkelijk, voor elke plaatsinzameling worden verleend. De stappen hieronder zullen u tonen hoe te om toestemming te verlenen schrijven aan nieuwe Plaats App een plaatsinzameling. Herhaal deze stappen voor elk van de plaatsinzamelingen u onder toevoegde [!UICONTROL Visible Site Collections] in de bovenstaande stappen.

Deze site-app moet [!UICONTROL Write] toestemming aan om het even welke plaatsinzamelingen die de gebruikers moeten toegang hebben door [!DNL Workfront].

1. &#39;/_layouts/15/appinv.aspx&#39; toevoegen aan de URL in [!DNL Sharepoint].

   **Voorbeeld:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. De volgende velden configureren

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL App ID]</td> 
      <td> <p>Client-id toevoegen waarin u hebt gemaakt <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Een [!DNL SharePoint] site </a>en klik op <strong>[!UICONTROL Lookup]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Client] / [!UICONTROL App Domain] / [!UICONTROL Redirect URL]</p> </td> 
      <td> <p>Deze worden automatisch gevuld wanneer u klikt [!UICONTROL Lookup].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Permission Request XML]</td> 
      <td> <p>Kopieer de volgende XML naar de [!UICONTROL Permission Request XML] veld. Zorg ervoor dat deze exact wordt toegevoegd zoals wordt weergegeven zonder extra spaties enz. om fouten te voorkomen.</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. Klik op **[!UICONTROL Create]**.
1. Klik in het dialoogvenster dat wordt weergegeven op **[!UICONTROL Trust it]**.
1. Controleer of de site-app toegang heeft tot de siteverzameling door op de knop **[!UICONTROL Site collection app permissions]** koppelen in [!UICONTROL Site Settings].
1. Herhaal bovenstaande stappen voor de resterende plaatsinzamelingen, dan ga met verder [Een [!DNL Workfront] [!DNL SharePoint] integratiefunctie](#create-a-workfront-sharepoint-integration-instance).

### Een [!DNL Workfront] [!DNL SharePoint] integratiefunctie {#create-a-workfront-sharepoint-integration-instance}

Wanneer u een site-app hebt gemaakt in [!DNL SharePoint]kunt u nu gegevens van de site-app kopiëren naar [!DNL Workfront]. De site-app is een appprincipal en fungeert als de conduit via welke OAuth-verzoeken worden gedaan om toegang te krijgen tot documenten in siteverzamelingen.

1. Aanmelden [!DNL Workfront] als beheerder.
1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **[!UICONTROL Documents]** > **[!UICONTROL [!DNL SharePoint] Integration]**.
1. Klik op **[!UICONTROL Add [!DNL SharePoint]]**.
1. Configureer de volgende velden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
      <td> <p>Voer een naam in voor de [!DNL SharePoint] integratie. Gebruikers zien deze naam wanneer ze op [!UICONTROL Add] &gt; [!UICONTROL From] "naam van de integratie". </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] Hostinstantie]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] Toegangsdomein]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>Dit verwijst naar de Master site die gebruikers gebruiken om te verifiëren. Het is waarschijnlijk hetzelfde domein als het [!UICONTROL [!DNL SharePoint] Hostinstantie].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>Belangrijk</b> Siteverzamelingen worden alleen in de Oudere versie gebruikt [!DNL SharePoint] Integratie.
       <ul> 
        <li> <p><b>Als u de hoofdsite van uw organisatie gebruikt</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Als u een master site en subsites gebruikt:</b> </p> <p><b>BELANGRIJK</b>: [!DNL Microsoft SharePoint] beveelt niet langer het gebruik van subsites aan.</p> <p>Voer de URL-stam in voor de siteverzameling die u in de bovenstaande sectie hebt gemaakt.</p> <p>Dit is de sectie van URL na .com.</p> <p>Voorbeeld: voor de URL <code>https://mycompany.sharepoint.com/sites/mysite</code>de stam <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Client-id]</td> 
      <td>Voer de client-id in die u hebt gegenereerd in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Een [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] Clientgeheim]</td> 
      <td>Voer het clientgeheim in dat u hebt gegenereerd in <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">Een [!DNL SharePoint] site </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Visible Site Collections]</td> 
      <td> <b>Belangrijk</b> Siteverzamelingen worden alleen in de Oudere versie gebruikt [!DNL SharePoint] integratie.
       <ul> 
        <li> <p><b> Als u de hoofdsite van uw organisatie gebruikt</b><b>:</b> </p> <p>Enter <code>/</code></p> </li> 
        <li> <p><b>Als u een master site en subsites gebruikt:</b> </p> <p><b>BELANGRIJK</b>: [!DNL Microsoft SharePoint] beveelt niet langer het gebruik van subsites aan.</p> <p>Voor elke subsite die u aan uw [!DNL SharePoint] , voert u de stam van de subsite in.</p> <p>Voorbeeld: voor de URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>de stam <code>/sites/mysite/mysubsite</code>.</p> <p><b>OPMERKING</b>:   <p>Als u alleen uw configuratie wilt testen (geen subsites), voert u de stam van de master site in. </p> <p>Voorbeeld: voor de URL <code> https://mycompany.sharepoint.com/sites/mysite</code>de stam <code>/sites/mysite</code>.</p> <p>Wanneer u de configuratie hebt getest zoals beschreven in <a href="#complete-your-integration" class="MCXref xref">Voltooi uw integratie</a>, moet u de master site verwijderen en de subsites invoeren.</p> 
          <ol> 
           <li value="1">Klik op de knop <strong>[!UICONTROL Main Menu]</strong> pictogram <img src="assets/main-menu-icon.png"> in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op <strong>[!UICONTROL Setup]</strong> <img src="assets/gear-icon-settings.png">.<li><p>Klik in het linkerdeelvenster op <strong>[!UICONTROL Documents]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] Integratie]</strong>.</p></li><li><p>Klik op de knop [!DNL SharePoint] de integratie u plaatst, dan klik uitgeven.</p></li><li><p>De stam voor de master site verwijderen uit de [!UICONTROL Visible Site Collections] veld.</p></li><li><p>Voor elke subsite die u aan uw [!DNL SharePoint] , voert u de stam van de subsite in.</p></li><p>Voorbeeld: voor de URL<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>de stam <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Save]**
1. Doorgaan naar [Voltooi uw integratie](#complete-your-integration).

### Voltooi uw integratie {#complete-your-integration}

De basisconfiguratie is bijna volledig.

1. Klik in Workfront op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Documents]** ![](assets/document-icon.png).
1. Klik op **[!UICONTROL Add new]**.
1. Klikken **[!UICONTROL From]`<title of your [!DNL SharePoint] site>`** in de vervolgkeuzelijst.

   Er wordt een dialoogvenster weergegeven waarin u wordt uitgenodigd deze site te vertrouwen.

   >[!NOTE]
   >
   >Als dit dialoogvenster niet wordt weergegeven, kunt u [!DNL SharePoint] integratie is niet correct gevormd.

1. Klik op **[!UICONTROL Trust it]**.

### Documenten toevoegen {#add-documents}

U kunt nu documenten toevoegen vanuit uw [!DNL SharePoint] site.

Zie voor instructies [Een extern document koppelen aan [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>Als de gebruiker die een map heeft gekoppeld, geen toegang meer heeft tot de externe toepassing, [!DNL Workfront] heeft geen toegang meer tot de inhoud van de map. Dit kan bijvoorbeeld gebeuren als de gebruiker die oorspronkelijk de map had gekoppeld het bedrijf verlaat. Een gebruiker met toegang tot de map moet de map opnieuw koppelen om ervoor te zorgen dat hij of zij toegang kan blijven krijgen.

## Problemen oplossen

* [Probleem: Gebruikers ondervinden bij het gebruik van de [!DNL SharePoint] integratie.](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [Probleem: Als [!DNL Workfront] -gebruiker, kan ik geen nieuwe [!DNL SharePoint] -instantie. Als ik probeer te doen, zie ik een fout.](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [Probleem: Wanneer wordt geprobeerd te bladeren [!DNL SharePoint] bestanden in [!DNL Workfront], ik zie geen van mijn plaatsinzamelingen of al mijn plaatsinzamelingen.](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [Probleem: Ik heb geen toegang tot eerder gekoppelde mappen en documenten in [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### Probleem: Gebruikers ondervinden bij het gebruik van de [!DNL SharePoint] integratie. {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

Oplossingen:

De gebruikers moeten een lid van een groep zijn die aangewezen toestemmingen aan de [!DNL SharePoint] site.

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

Voor instructies over het creëren van en het uitgeven van toestemmingenniveaus, zie [machtigingsniveaus maken en bewerken](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) in de documentatie van Microsoft.

### Probleem: Als [!DNL Workfront] -gebruiker, kan ik geen nieuwe [!DNL SharePoint] -instantie. Als ik probeer te doen, zie ik een fout. {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

Oplossingen:

Dit kan worden veroorzaakt door een aantal dingen, die van of [!DNL Workfront] of [!DNL SharePoint]s configuratie. Controleren of:

* Client ID, Client Secret, return URL en andere configuratievelden worden correct toegewezen tussen de [!DNL Workfront] [!DNL SharePoint] Integratie-instantie en de [!DNL SharePoint] Site-app.
* De gebruiker heeft [!UICONTROL Full Control] toestemming aan de Inzameling van de Plaats die voor authentificatie wordt gebruikt.
* De Site-app staat onder [!UICONTROL Site App Permissions] voor de [!UICONTROL Site Collection] gebruikt voor verificatie.

### Probleem: Wanneer wordt geprobeerd te bladeren [!DNL SharePoint] bestanden in [!DNL Workfront], ik zie geen van mijn plaatsinzamelingen of al mijn plaatsinzamelingen. {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

Oplossingen:

Om een plaatsinzameling in te zien [!DNL Workfront]moet aan de volgende voorwaarden worden voldaan:

* De plaatsinzameling moet in worden geregistreerd [!DNL Workfront] [!DNL SharePoint] Integratie-instantie.

   Om dit te verifiëren in [!DNL Workfront]:

   1. Ga naar [!UICONTROL Setup] > [!UICONTROL Documents] > [!UICONTROL [!DNL SharePoint] Integration].
   1. Bewerk de [!DNL SharePoint] Informatie over integratieinstanties.
   1. Controleren of de siteverzameling onder staat staat [!UICONTROL Visible Site Collections].

* De gebruiker moet meningstoegang tot de plaatsinzameling in hebben [!DNL SharePoint].
* Om dit te verifiëren in [!DNL SharePoint], ga naar [!DNL SharePoint]en open de siteverzameling > [!UICONTROL Settings] > [!UICONTROL Site permissions].
* De [!DNL SharePoint] Site App moet toegang hebben tot de siteverzameling.

   Om dit te verifiëren in [!DNL SharePoint]:

   1. Ga naar de siteverzameling > [!UICONTROL Settings] > [!UICONTROL Site app permissions].
   1. Zorg ervoor dat de [!UICONTROL Site App] gebruikt door [!DNL Workfront] wordt hier weergegeven.
   1. (Voorwaardelijk) als App van de Plaats niet vermeld is, voeg aan de plaatsinzameling toe gebruikend _layouts/15/appinv.aspx.

      Voor informatie over het toevoegen van de plaatsinzameling, zie het verlenen schrijft Toestemmingen aan App van de Plaats.

### Probleem: Ik heb geen toegang tot eerder gekoppelde mappen en documenten in [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

Oplossing:

Als de gebruiker die een koppeling heeft gemaakt [!DNL SharePoint] map kan niet meer worden geverifieerd, [!DNL Workfront] heeft geen toegang meer tot de inhoud van de map. Dit kan bijvoorbeeld gebeuren als de gebruiker die oorspronkelijk de map had gekoppeld het bedrijf verlaat.

Een gebruiker met toegang tot de map moet de map opnieuw koppelen om ervoor te zorgen dat hij of zij toegang kan blijven krijgen.

Voor informatie over het koppelen van mappen van externe providers raadpleegt u [Documenten van externe toepassingen koppelen](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### Probleem: Ik zie een fout &quot;404 niet gevonden&quot; bij het toevoegen van een document van [!DNL Sharepoint]

#### Oplossing:

Deze fout zou kunnen voorkomen als één van de plaatsen in worden gevormd [!UICONTROL Visible Site Collections] list is verwijderd in Sharepoint. Controleer de [!UICONTROL Visible Site Collections] lijst, en verwijder om het even welke plaatsen die in SharePoint zijn geschrapt.
