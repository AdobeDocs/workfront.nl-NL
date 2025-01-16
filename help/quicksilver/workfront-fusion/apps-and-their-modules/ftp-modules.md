---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP-modules
description: De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie. Dit artikel is vervangen, maar bevat een koppeling naar het nieuwe artikel dat deze functionaliteit behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# FTP-modules

>[!IMPORTANT]
>
>De Adobe Workfront Fusion-documentatie is verplaatst naar een nieuwe locatie.
>
>De informatie in dit artikel is nu te vinden in het artikel:
>
>* [ modules van FTP ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/ftp-modules.html)
>
>Werk eventuele bladwijzers bij.
>
>Dit artikel wordt niet meer bijgewerkt en wordt in de nabije toekomst verwijderd.

Met FTP-modules kunt u bestandswijzigingen in een geselecteerde map controleren, nieuwe bestanden naar de gewenste map uploaden en bestaande bestanden die zich al in een map bevinden, wijzigen of verwijderen.

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
   <p>Huidige productvereiste: als u het abonnement [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] hebt, moet uw organisatie [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken. [!DNL Workfront Fusion] wordt opgenomen in het [!UICONTROL Ultimate] [!DNL Workfront] -abonnement.</p>
   <p>of</p>
   <p>Vereiste verouderd product: uw organisatie moet [!DNL Adobe Workfront Fusion] en [!DNL Adobe Workfront] aanschaffen om de in dit artikel beschreven functionaliteit te kunnen gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met de [!DNL Workfront] -beheerder als u wilt weten welk abonnement, licentietype of toegang u hebt.

Voor informatie over [!DNL Adobe Workfront Fusion] vergunningen, zie [[!DNL Adobe Workfront Fusion]  vergunningen ](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Om [ Fusion App ] met [!DNL Workfront Fusion] te gebruiken, moet u een rekening van FTP hebben.

## Verbinding maken in een FTP-module {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection name]</td> 
   <td> <p> Voer de naam in voor uw FTP-verbinding.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Voer de hostnaam van de FTP-server in. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Voer het poortnummer van de FTP-server in. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL User name] </td> 
   <td> <p>Voer de gebruikersnaam van uw FTP-account in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Password] </td> 
   <td> <p>Voer het wachtwoord voor uw FTP-account in.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Een beveiligde verbinding (TLS) gebruiken</p> </td> 
   <td> <p>Selecteer of u een veilige verbinding wilt gebruiken.</p> <p style="font-weight: bold;">[!UICONTROL No]</p> <p>De verbinding is niet beveiligd.</p> <p style="font-weight: bold;">[!UICONTROL Explicit encryption or Implicit encryption]</p> <p>De verbinding wordt beveiligd met SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Reject unauthorized certificates]</p> </td> 
   <td> <p>Schakel deze optie in om het FTP-servercertificaat te verifiëren. Als de verificatie mislukt, wordt er geen verbinding gemaakt. Om voor de verificatie te slagen, moet het certificaat aan een van de volgende criteria voldoen:</p> 
    <ul> 
     <li>worden ondertekend door aRoot <a href="https://en.wikipedia.org/wiki/Certificate_authority"> Instantie van het Certificaat </a></li> 
     <li>worden ondertekend door een Directe Instantie van het Certificaat (zie b.v. <a href="https://knowledge.digicert.com/solution/SO16297.html"> hoe de certificaatketens </a> voor verdere verklaring werken). In dit geval moeten alle tussentijdse certificaten op de FTP-server zijn geïnstalleerd.</li> 
     <li>Een zelfondertekend certificaat zijn dat wordt opgegeven in het veld [!UICONTROL Self-signed certificate] (zie hieronder)</li> </ul>

Als deze optie is uitgeschakeld, wordt het FTP-servercertificaat niet geverifieerd. Wij raden u ten zeerste aan de optie niet uit te schakelen, omdat hierdoor de verbinding onveilig wordt en een ernstig veiligheidsrisico ontstaat.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Self-signed certificate]</p> </td> 
   <td> <p>Klik op de knop <b>[!UICONTROL Extract]</b> om het dialoogvenster voor uploaden te openen.</p> <p>Upload het certificaat om het TLS te gebruiken met uw zelfondertekende certificaat. [!DNL Workfront Fusion] bewaart of bewaart geen gegevens u, zoals dossiers en wachtwoorden verstrekt. Bestand en wachtwoord worden alleen gebruikt om het certificaat te extraheren.</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP-modules en de bijbehorende velden

* [Triggers](#triggers)
* [Handelingen](#actions)

### Triggers

#### [!UICONTROL Watch files]

[!UICONTROL Watch files] is de enige triggermodule voor FTP. De inhoud van de geselecteerde map wordt gecontroleerd. De trigger wordt uitgevoerd wanneer een nieuw bestand in de opgegeven map wordt ingevoegd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Selecteer de map die u wilt controleren.</p> <p><b> Nota:</b> slechts één omslag per scenario wordt toegestaan. Submappen worden genegeerd.</p> <p><b> Uiteinde:</b> om spoor van veelvoudige omslagen te houden, creeer een onafhankelijk scenario voor elk van hen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files] </td> 
   <td> <p>Stel het maximale aantal resultaten in waarmee [!DNL Workfront Fusion] gedurende één cyclus werkt. Als de waarde te hoog is ingesteld, kan de verbinding aan de kant van de opgegeven service van derden (timeout) worden onderbroken. [!DNL Workfront Fusion] heeft hier geen invloed op. Wij adviseren dat u een lagere waarde plaatst en of een hogere waarde voor het maximumaantal cycli bepaalt of het scenario vaker in werking stelt.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

* [[!UICONTROL Change permissions]](#change-permissions)
* [[!UICONTROL Create a folder]](#create-a-folder)
* [[!UICONTROL Delete a file]](#delete-a-file)
* [[!UICONTROL Delete a folder]](#delete-a-folder)
* [[!UICONTROL Get a file]](#get-a-file)
* [[!UICONTROL List of files in a folder]](#list-of-files-in-a-folder)
* [[!UICONTROL Move a file or folder]](#move-a-file-or-folder)
* [[!UICONTROL Upload] een bestand](#upload-a-file)

#### [!UICONTROL Change permissions]

In deze handelingsmodule worden de machtigingsinstellingen van een bestand of map gewijzigd.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Change permission settings of]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Selecteer of u de instellingen voor een bestand of map wilt wijzigen.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL File path]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Voer het bestandspad in of wijs het toe aan de map of het bestand.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Permissions]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Stel de gewenste bestands- of mapmachtigingen in. Gebruik de parameters chmod. Bijvoorbeeld: <code>777 </code> of <code>-rwxrwxrwx</code> .</p>
               <p>Rechten moeten overeenkomen met het patroon <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code> .</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Create a folder]

Deze actiemodule maakt een nieuwe map.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Folder path]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Voer het bestandspad in of wijs het toe aan de nieuwe map.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL New folder name]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Voer een naam voor de nieuwe map in of wijs deze toe.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Delete a file]

Hiermee wordt een bestand uit de opgegeven map verwijderd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de FTP-map waaruit u een bestand wilt verwijderen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File name]</td> 
   <td> <p> Voer de bestandsnaam in, inclusief de bestandsnaamextensie. Voorbeeld: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a folder]

Deze actiemodule verwijdert de opgegeven map permanent.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Folder]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Selecteer de FTP-map waaruit u een bestand wilt verwijderen.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Get a file]

Hiermee wordt een bestand opgehaald van de FTP-server dat verder kan worden verwerkt, bijvoorbeeld geüpload naar de [!DNL Dropbox] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#creating-the-ftp-connection" class="MCXref xref"> Creërend de Verbinding van FTP </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File path]</td> 
   <td> <p> Voer het pad in van het bestand dat u wilt ophalen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List of files in a folder]

Hiermee worden bestands- en/of mapgegevens opgehaald.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#creating-the-ftp-connection" class="MCXref xref"> Creërend de Verbinding van FTP </a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de FTP-map waarin u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Selecteer of u informatie over bestanden of mappen of beide wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Voer de zoekterm in. Als er geen zoekterm is ingevoerd, worden alle bestanden en mappen uit de opgegeven map opgehaald.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
   <td> <p> Stel het maximumaantal opgehaalde bestanden in door deze module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a file or folder]

Deze actiemodule verplaatst een bestand of map naar een andere locatie.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Connection]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#Create" class="MCXref xref" >[!UICONTROL Create a connection] in een module van FTP </a> in dit artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Old file path]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Voer het pad in waaruit u het bestand wilt verplaatsen. Voorbeeld: <code>/folder1/document.txt</code> .</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL New file path]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Voer het pad in waarnaar u het bestand wilt verplaatsen. Voorbeeld: <code>/folder2/document.txt</code> .</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL Upload a file]

Uploadt een bestand naar de FTP-server.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td>Voor instructies bij het vestigen van een verbinding aan de rekening van FTP, zie <a href="#creating-the-ftp-connection" class="MCXref xref"> Creërend de Verbinding van FTP </a> in dit artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de FTP-map waarnaar u het bestand wilt uploaden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file] </td> 
   <td> <p>Selecteer een bronbestand uit een vorige module of wijs de naam en gegevens van het bronbestand toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Append to an already existing file]</td> 
   <td> <p>Als deze optie is ingeschakeld en het bestand al op de FTP-server staat, wordt de inhoud van het bestand aan het bestaande bestand toegevoegd. Als deze optie niet is ingeschakeld, wordt de inhoud van het bestand overschreven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Create folders if don't exist] </td> 
   <td> <p>Als deze optie is ingeschakeld en de map die u in het veld Map hebt ingevoerd, niet bestaat op de FTP-server, maakt de module de map</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemen oplossen {#troubleshooting}

Als u problemen ondervindt met de FTP-toepassing tijdens het maken van de verbinding of tijdens het uitvoeren van een module, probeert u een van de populaire FTP-clients te gebruiken en probeert u dezelfde actie uit te voeren (bijvoorbeeld het maken van een verbinding of het weergeven van bestanden in een map). met de FTP-client. Als u dezelfde problemen ook ondervindt met de FTP-client, is de reden mogelijk een verkeerde configuratie van de FTP-server.
