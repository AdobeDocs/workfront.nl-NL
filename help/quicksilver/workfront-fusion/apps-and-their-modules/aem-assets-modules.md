---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets-modules
description: Met de  [!DNL Adobe Experience Manager Assets]  schakelaar voor  [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets]  rekening, creeer, upload, en werk activa bij, en kopieer of verplaats omslagen en activa.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1308'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] modules

Met de [!DNL Adobe Experience Manager Assets] -connector voor [!DNL Adobe Workfront Fusion] kunt u een scenario starten op basis van gebeurtenissen in uw [!DNL Adobe Experience Manager Assets] -account, elementen maken, uploaden en bijwerken en mappen en elementen kopiëren of verplaatsen.

Voor een inleiding aan de schakelaar van Adobe Experience Manager Assets, zie:

* [ Adobe Experience Manager Assets ](https://video.tv.adobe.com/v/3427034/){target=_blank}

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige licentievereiste: geen [!DNL Workfront Fusion] licentievereiste.</p>
   <p>of</p>
   <p>Vereiste voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u het [!UICONTROL Select] - of [!UICONTROL Prime] [!DNL Adobe Workfront] -abonnement hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

* U moet een [!DNL Adobe Experience Manager Assets] account hebben om deze modules te kunnen gebruiken.
* U moet de [!UICONTROL Server-to-server] -stroom instellen in de [!DNL Adobe Developer console] .

  Voor instructies bij vestiging [!UICONTROL Server-to-server] stroom in [!DNL Adobe Developer console], zie [ Genererend de Tokens van de Toegang voor de Kant APIs van de Server ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Verbinden [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

Verbinding maken voor uw [!DNL Adobe Experience Manager Assets] -modules:

1. Klik op [!UICONTROL Add] naast het vak [!UICONTROL Connection] .

2. Selecteer het type verbinding dat u maakt:

   * **[!DNL AEM Assets as a Cloud Service]**

     Voor deze configuratie is informatie van de [!DNL Adobe Admin Console] vereist.

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Voor deze configuratie zijn een gebruikersnaam en wachtwoord vereist.

3. Vul de velden in voor het type verbinding dat u maakt.

   Voor [!DNL AEM Assets as a Cloud Service], zie [ de verbinding voor  [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service) vormen.

   Voor [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]), zie [ de verbinding voor [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic) vormen.

4. Klik op **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.


### De verbinding configureren voor [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>De informatie voor deze velden wordt gegenereerd als onderdeel van het instellen van de [!UICONTROL Server-to-server] -stroom op de [!DNL Adobe Developer Console] . U kunt deze waarden vinden in het JSON-bestand met servicereferenties dat is gegenereerd als onderdeel van die instelling.
>
>Voor instructies bij vestiging [!UICONTROL Server-to-server] stroom op [!UICONTROL Adobe Developer Console], zie [ Genererend de Tokens van de Toegang voor de Kant APIs van de Server ](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Connection name]</td>
                  <td>
                      <p>Geef een naam op voor deze verbinding</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                  <td>Voer de URL voor de instantie [!DNL Adobe Experience Manager] in. Plaats geen schuine streep <code>/</code> aan het einde van de URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Voer de client-id in die in de setup van [!UICONTROL Server-to-server] wordt gegenereerd.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Voer het clientgeheim in dat in de [!UICONTROL Server-to-server] -instelling wordt gegenereerd.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Technical account ID]</td>
                  <td>Voer de id van de technische rekening in. Dit is het veld "[!UICONTROL id]" in het JSON-bestand met clientreferenties.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">Voer de id van uw organisatie in. Dit is het veld "[!UICONTROL org]" in het JSON-bestand met clientreferenties.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta Scopes]</td>
                  <td>Voer de meta-bereiken in die in de [!UICONTROL Server-to-server] -instelling worden gegenereerd.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Private key]</td>
                  <td>Voer de gegenereerde persoonlijke sleutel in om de [!UICONTROL Server-to-server] -instelling te verkrijgen. Als u de persoonlijke sleutel wilt uitnemen, klikt u op [!UICONTROL Extract] en voert u het bestand in dat u wilt uitpakken en het wachtwoord voor het bestand.</td>
              </tr>
          </tbody>
      </table>


### De verbinding configureren voor [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Connection name]</td>
                <td>
                    <p>Geef een naam op voor deze verbinding</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                <td>Voer de URL voor de instantie [!DNL Adobe Experience Manager] in. Plaats geen schuine streep <code>/</code> aan het einde van de URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Voer de gebruikersnaam in voor de [!DNL AEM Assets] -account die deze verbinding gebruikt.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Voer het wachtwoord in voor de [!DNL AEM Assets] -account die door deze verbinding wordt gebruikt.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] modules en hun velden

Wanneer u [!DNL Adobe Experience Manager Essentials] modules configureert, geeft [!DNL Workfront Fusion] de onderstaande velden weer. Daarnaast kunnen aanvullende [!DNL Adobe Experience Manager Essentials] -velden worden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Voor meer informatie, zie [ informatie van de Kaart van één module aan een andere in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Copy a folder or asset]

Deze actiemodule kopieert een map of middel naar een andere locatie in uw Adobe Experience Manager Assets-account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u een map of een element wilt kopiëren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>Selecteer of wijs de omslag of de activa toe die u wilt kopiëren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Selecteer of wijs het pad toe aan de locatie voor de nieuwe map of het nieuwe element.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of copied folder] / [!UICONTROL asset]</td> 
   <td>Voer een naam in voor de nieuwe map of het nieuwe middel. De mapnaam die wordt weergegeven in [!DNL Adobe Experience Manager Assets] is gelijk aan de oorspronkelijke naam. De hier ingevoerde naam wordt weergegeven in de URL van de nieuwe map of het nieuwe middel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy children]</td> 
   <td>Schakel deze optie in om submappen of elementen in de map te kopiëren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Schakel deze optie in om mappen of middelen op de doellocatie te overschrijven die dezelfde naam hebben als de map of het element dat wordt gekopieerd.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a record]

In deze actiemodule wordt een map of elementcommentaar gemaakt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object type]</td> 
   <td> <p>Selecteer of u een map of een opmerking over een element wilt maken.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Vul de volgende velden in:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Voer een naam in voor de map. Deze naam wordt weergegeven in het bestandspad. Spaties of andere tekens worden dus niet opgenomen. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Voer een titel voor de map in, die u kunt weergeven in plaats van de naam.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset comment]</p> <p>Vul de volgende velden in:</p> 
      <ul> 
       <li> <p>[!UICONTROL Asset selection]</p> <p>Selecteer of wijs identiteitskaart van de activa toe u een commentaar aan wilt toevoegen.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>Voer de tekst van de opmerking in.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a record]

Met deze actiemodule verwijdert u een map, element of uitvoering.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u een map, element of uitvoering wilt verwijderen.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Selecteer de map die u wilt verwijderen door de mappen in het bijbehorende pad te selecteren.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Selecteer het element door de mappen in het bijbehorende pad te selecteren en vervolgens het element dat u wilt verwijderen.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Selecteer de vertoning door de mappen in het bijbehorende pad te selecteren.</p> <p>Voer de naam van de vertoning in of wijs deze toe.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a folder listing]

Deze actiemodule wint een vertegenwoordiging van een bestaande omslag en van zijn kindentiteiten (omslagen of activa) terug.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Selecteer of wijs de omslag toe die u wilt terugwinnen. Als u submappen aan het pad wilt toevoegen, klikt u op het plusteken en selecteert u de submap.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make a custom API call]

Deze actiemodule maakt een aangepaste API-aanroep naar de [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Voer een pad in dat relatief is ten opzichte van de basis-URL van [!DNL Adobe Experience Manager] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref"> HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a> voor meer informatie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Voeg de kopteksten van het verzoek toe in de vorm van een standaard JSON-object.</p> <p>Bijvoorbeeld: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Voer de queryreeks voor de aanvraag in. Voor Elk sleutel/waardepaar klikt u op <b>[!UICONTROL Add item]</b> en voert u de [!UICONTROL Key] en [!UICONTROL Value] in.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:  <p>Wanneer u voorwaardelijke instructies gebruikt, zoals <code>if</code> in uw JSON, plaatst u de aanhalingstekens buiten de voorwaardelijke instructie.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Move a folder or asset]

Met deze actiemodule verplaatst u het element of de map op het opgegeven pad naar een nieuwe locatie.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u een map of element wilt verplaatsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>Selecteer of wijs de map of middelen toe die u wilt verplaatsen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Selecteer of wijs het pad toe aan de locatie waarnaar u de map of het element wilt verplaatsen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of moved folder] / [!UICONTROL asset]</td> 
   <td>Voer een nieuwe naam in voor de verplaatste map of het verplaatste middel. De mapnaam die wordt weergegeven in [!DNL Adobe Experience Manager Assets] is gelijk aan de oorspronkelijke naam. De hier ingevoerde naam wordt weergegeven in de URL van de verplaatste map of het verplaatste middel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Schakel deze optie in om mappen of middelen op de doellocatie te overschrijven die dezelfde naam hebben als de map of het element dat wordt gekopieerd.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a record]

Deze actiemodule werkt een bestaande record bij.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Selecteer of u metagegevens van elementen of een elementuitvoering wilt verwijderen.</p> 
    <ul> 
     <li> <p>[!UICONTROL Asset metadata]</p> 
      <ul> 
       <li> <p>Selecteer het element waarvoor u metagegevens wilt bijwerken.</p> </li> 
       <li> <p>Voer de nieuwe titel van het element in.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset rendition]</p> 
      <ul> 
       <li> <p>Selecteer het element waarvoor u de vertoning wilt bijwerken.</p> </li> 
       <li> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Upload an asset]

Deze actiemodule uploadt een middel naar uw [!DNL Adobe Experience Manager Assets] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Zie <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref"> Verbinding maken [!DNL Adobe Experience Manager Assets] met [!DNL Workfront Fusion]</a> in dit artikel voor instructies over het verbinden van uw [!DNL Adobe Experience Manager Assets] -account met [!DNL Workfront Fusion] .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination]</td> 
   <td> <p>Selecteer de map waarin u middelen wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Voer de naam en gegevens van het bronbestand in of wijs deze toe.</td> 
  </tr> 
 </tbody> 
</table>
