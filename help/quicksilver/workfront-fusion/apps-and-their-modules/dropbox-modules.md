---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Dropbox
description: In een [!DNL Adobe Workfront Fusion] scenario's, kunt u werkschema's automatiseren die Dropbox gebruiken, evenals het verbinden met veelvoudige derdetoepassingen en de diensten. Dit staat u toe om activiteiten zoals controle, het zoeken, het terugwinnen van, het een lijst maken van, het creëren van, en het uitgeven van dossiers en omslagen in uw Dropbox te automatiseren.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
source-git-commit: 86be8b6e1c21f3fd5f5b66afa3bf930d6bafbd63
workflow-type: tm+mt
source-wordcount: '2842'
ht-degree: 0%

---

# [!DNL Dropbox] modules

In een [!DNL Adobe Workfront Fusion] scenario, kunt u werkschema&#39;s automatiseren die gebruiken [!UICONTROL Dropbox] of [!DNL Dropbox Business], en sluit deze aan op meerdere toepassingen en services van derden. Hierdoor kunt u activiteiten zoals het controleren, zoeken, ophalen, weergeven, maken en bewerken van bestanden en mappen in uw [!UICONTROL Dropbox].

Als u instructies bij het creëren van een scenario nodig hebt, zie [Een scenario maken in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Voor informatie over modules, zie [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Huidige vergunningsvereiste: Neen [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereiste: als u beschikt over [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Vereisten voor verouderd product: uw organisatie moet het product kopen [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

* Te gebruiken [!DNL Dropbox] modules, moet u een [!DNL Dropbox] account.

>[!IMPORTANT]
>
>Dropbox moet toepassingen met meer dan 50 gebruikers goedkeuren.
>
>Voor meer informatie, zoek naar &quot;Goedkeuring van de Productie&quot;in de Dropbox ontwikkelaarsgids.


## Verbinding maken met [!DNL Dropbox]

Als u een verbinding wilt maken voor uw [!DNL Dropbox] modules:

1. Klikken **[!UICONTROL Add]** naast het vak Verbinding.

1. Vul de volgende velden in:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Voer een naam in voor deze verbinding.</p>
        </td>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Selecteer of deze verbinding voor een productie of een non-productie milieu is.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Selecteer of u verbinding maakt met een serviceaccount of een persoonlijke account.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Voer uw [!UICONTROL Dropbox] [!UICONTROL Client ID]. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Voer uw [!DNL Dropbox] [!UICONTROL Client Secret]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Account Type]</td>
        <td>Selecteer of u met een persoonlijke rekening van de Dropbox of een bedrijfsrekening (de Zaken van de Dropbox) verbindt.</td>
        </tr>
      </tbody>
    </table>

1. Klikken **[!UICONTROL Continue]** om de verbinding op te slaan en terug te keren naar de module.## [!DNL Dropbox] modules en hun velden

## [!DNL Dropbox] modules en hun velden

Wanneer u [!DNL Dropbox] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!DNL Dropbox] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggermodules](#trigger-modules)
* [Modules voor ophalen [!DNL Dropbox] bestanden en mappen](#modules-for-getting-dropbox-files-and-folders)
* [Modules voor maken en bewerken [!DNL Dropbox] bestanden en mappen](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Overige modules](#other-modules)

### Triggermodules

#### [!UICONTROL Watch Files]

Deze triggertypemodule retourneert bestandsgegevens wanneer het bestand in een opgegeven map wordt gewijzigd.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map die u wilt controleren op wijzigingen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch also subfolders]</td> 
   <td> <p> Schakel deze optie in om ook de submappen in de geselecteerde map te controleren op gewijzigde bestanden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit] </td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules voor ophalen [!DNL Dropbox] bestanden en mappen

* [[!UICONTROL Search Files/Folders]](#search-filesfolders)
* [[!UICONTROL Download a File]](#download-a-file)
* [[!UICONTROL Get a Folder Metadata]](#get-a-folder-metadata)
* [[!UICONTROL List All Files/Subfolders in a Folder]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL List File Revisions]](#list-file-revisions)

#### [!UICONTROL Search Files/Folders]

Deze zoekmodule zoekt naar records in een object in [!DNL Dropbox] die overeenkomen met de zoekquery die u opgeeft.

U kunt deze informatie in verdere modules in het scenario in kaart brengen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Voer de zoekterm in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de map die u wilt doorzoeken. Deze module zoekt het volledige [!DNL Dropbox] als u geen map selecteert.</p> </td> 
  </tr> 
  <tr> 
   <td>Bestandsstatus</td> 
   <td> <p> Selecteer de bestandsstatus om de zoekopdracht te beperken tot de geselecteerde bestandsstatus.</p> </td> 
  </tr> 
  <tr> 
   <td>Bestandscategorieën</td> 
   <td> <p> Selecteer de bestandscategorieën om de zoekopdracht te beperken tot de geselecteerde categorieën.</p> </td> 
  </tr> 
  <tr> 
   <td>Bestandsextensies</td> 
   <td> <p> Kies de bestandsextensies waarnaar u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>Limiet </td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a File]

Deze actiemodule downloadt een bestand uit een map.

U geeft het bestand en de locatie op.

De module retourneert de id van het bestand en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

>[!NOTE]
>
>Deze module is nuttig om dossiers aan verdere modules te verstrekken.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>Wijze waarop bestanden worden geselecteerd</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of het bestand handmatig wilt selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Bestandspad / Bestand</p> </td> 
   <td> <p style="font-weight: bold;">Bestandspad</p> <p>Typ of wijs het doelpad naar het bestand toe.</p> <p style="font-weight: bold;">Bestand</p> <p>Selecteer het bestand in het menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Folder Metadata]

In deze actiemodule worden de gegevens van de gedeelde map opgehaald.

U geeft de id van de map op.

De module retourneert de id van de map en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>Gedeelde map-id</td> 
   <td> <p> Voer de id in van de map waarover u gegevens wilt ophalen of wijs deze toe.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List All Files/Subfolders in a Folder]

In deze actiemodule worden bestanden of mappen in een bepaalde map weergegeven.

U geeft de id van de map op.

De module retourneert de id&#39;s van de bestanden of mappen en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>Lijst </td> 
   <td> <p>Selecteer of u bestanden of mappen wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>Alleen downloadbare bestanden tonen</td> 
   <td> <p> Schakel deze optie in als u alleen downloadbare bestanden wilt retourneren. Sommige bestandstypen, zoals Google Docs, kunnen niet worden gedownload.</p> </td> 
  </tr> 
  <tr> 
   <td>Map </td> 
   <td> <p>Voer de map in waarvan u bestanden of mappen wilt ophalen of wijs de map toe.</p> </td> 
  </tr> 
  <tr> 
   <td>Limiet </td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt een lijst maken.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List File Revisions]

Deze actiemodule haalt alle bestandsrevisies (een versiegeschiedenis) van een bepaald bestand op.\
U geeft de id van het bestand op.

De module retourneert alle standaardvelden die aan de record zijn gekoppeld, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>Wijze waarop bestanden worden geselecteerd</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of het bestand handmatig wilt selecteren.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Bestandspad / Bestand</p> </td> 
   <td> <p style="font-weight: bold;">Bestandspad</p> <p>Typ of wijs het doelpad naar het bestand toe.</p> <p style="font-weight: bold;">Bestand</p> <p>Selecteer het bestand in het menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limiet</p> </td> 
   <td> <p>Ga of kaart het maximumaantal verslagen in u de module tijdens elke cyclus van de scenariouitvoering wilt een lijst maken.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules voor maken en bewerken [!DNL Dropbox] bestanden en mappen

* [[!UICONTROL Upload] een bestand](#upload-a-file)
* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Create/Overwrite a Text File]](#createoverwrite-a-text-file)
* [[!UICONTROL Create/Update a Share Link]](#createupdate-a-share-link)
* [[!UICONTROL Restore a File]](#restore-a-file)
* [[!UICONTROL Move a File/Folder]](#move-a-filefolder)
* [[!UICONTROL Rename a File/Folder]](#rename-a-filefolder)
* [[!UICONTROL Delete a File/Folder]](#delete-a-filefolder)

#### [!UICONTROL Upload a File]

Deze actiemodule uploadt een bestand naar een map.

U geeft informatie op zoals de locatie van het bestand, het bestand dat u wilt uploaden en een optionele nieuwe naam voor het bestand.

De module retourneert de id van het bestand en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td> <p> Selecteer de map van uw [!DNL Dropbox] U wilt het bestand uploaden naar.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Voer het bestand in dat u aan het bestand wilt toevoegen of wijs het bestand toe [!DNL Dropbox] hierboven geselecteerde map.</p> <p style="font-weight: bold;">[!UICONTROL File name]</p> <p>Voer de bestandsnaam in of wijs deze toe, inclusief de bestandsextensie.</p> <p style="font-weight: bold;">[!UICONTROL File data]</p> <p>Voer de bestandsgegevens in of wijs deze toe (van vorige modules zoals [!UICONTROL Google Drive] &gt;[!UICONTROL Get a File)].</p> <p>Opmerking: de maximale grootte van het geüploade bestand is 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing file]</td> 
   <td> <p> Schakel deze optie in om het bestaande bestand te vervangen door het nieuwe bestand. Als deze optie niet is ingeschakeld, wordt de naam van het geüploade bestand gewijzigd.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Folder]

Deze actiemodule maakt een nieuwe map.

U geeft het pad en een naam voor de map op.

De module retourneert de id van de map en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name] </td> 
   <td> <p>Voer de naam voor de nieuwe map in.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Voer het pad in of wijs het toe op de plaats waar u een nieuwe map wilt maken.</p> <p>Opmerking:   <p>Als u een [!DNL Dropbox Business] account (met teamspaties), moet u de slash verwijderen <code>/</code>, of klik niet op <strong>[!UICONTROL Click here] om map te kiezen</strong> om een teammap in de hoofdmap te maken.</p> <p>Als de schuine streep niet wordt verwijderd, treedt een fout op <code>[409] path/malformed_path/..</code> wordt geretourneerd.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auto rename]</td> 
   <td> <p> Schakel deze optie in om de naam van de nieuwe map te wijzigen als er al een map met dezelfde naam bestaat op de doellocatie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Overwrite a Text File]

In deze actiemodule wordt een DOC-bestand gemaakt of wordt de inhoud van een bestaand bestand overschreven.

U geeft het bronbestand en de map op.

De module retourneert de id van de map en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select to]</td> 
   <td> <p> Selecteer of u een DOC-bestand wilt maken of overschrijven.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Selecteer de doellocatie waar u een bestand wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Voer het bestand in dat u aan het bestand wilt toevoegen of wijs het bestand toe [!DNL Dropbox] map.</p> <p style="font-weight: bold;">Bestandsnaam</p> <p>Voer de bestandsnaam in voor het nieuwe DOC-bestand (zonder extensie).</p> <p style="font-weight: bold;">Bestandsinhoud</p> <p>Voer de tekstinhoud van het DOC-bestand in.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Share Link]

In deze actiemodule wordt een openbare koppeling naar een bestand gemaakt.

U geeft het bestand en de informatie over de koppeling op.

De module retourneert de id van de koppeling en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of invoeren, of selecteer het bestand handmatig.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path / File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Typ of wijs het doelpad naar het bestand toe.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Selecteer het bestand in het menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Requested Visibility]</p> </td> 
   <td> <p>Selecteer of de verbinding openbaar, voor team, of wachtwoord beperkt is.</p> <p>Opmerking: [!UICONTROL Team only] en [!UICONTROL Access with password] opties zijn alleen beschikbaar voor gebruikers met [!DNL Dropbox Pro] of hoger.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Link's Expiration Date]</td> 
   <td> <p> Voer de datum en tijd in waarop de koppeling verloopt en niet meer toegankelijk is. Als dit veld leeg blijft, verloopt de koppeling niet. Voor een lijst met ondersteunde datum- en tijdnotaties raadpleegt u <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Afgedwongen typegebruik in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Opmerking: [!UICONTROL Team only] en [!UICONTROL Access with password] opties zijn alleen beschikbaar voor gebruikers met [!UICONTROL Dropbox Pro] of hogere versies.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Link's Access Level]</p> </td> 
   <td> <p>Stel de machtigingen voor de ontvanger van de koppeling in.</p> <p><strong>[!UICONTROL Viewer]</strong> Gebruikers die de koppeling gebruiken, kunnen de inhoud weergeven en opmerkingen plaatsen.</p> <p><strong>[!UICONTROL Editor]</strong> Gebruikers die de koppeling gebruiken, kunnen de inhoud bewerken, weergeven en opmerkingen plaatsen.</p> <p><strong>[!UICONTROL Max]</strong> Gebruikers die de koppeling gebruiken, ontvangen het maximale toegangsniveau waarop u de koppeling kunt instellen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restore a File]

In deze actiemodule wordt een vorige versie van een bestand hersteld.

U geeft het bestand en het nummer van de gewenste revisie op.

De module retourneert de id van de versie en alle bijbehorende velden, samen met eventuele aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of invoeren, of selecteer het bestand handmatig.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL File Path]</strong> </p> <p>Typ of wijs het doelpad naar het bestand toe.</p> <p><strong>[!UICONTROL File]</strong> </p> <p>Selecteer het bestand in het menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Ga of kaart het revisieaantal van de revisie in u wilt herstellen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File/Folder]

Deze actiemodule verplaatst een bestand of map naar een andere locatie.

U geeft het bestand of de map op en bepaalt hoe en waar u het bestand of de map wilt verplaatsen.

De module retourneert de id van het bestand of de map en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files] </td> 
   <td> <p>Selecteer of u het bestandspad wilt toewijzen of invoeren, of selecteer het bestand handmatig.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File/Folder Path] / [!UICONTROL File/Folder]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File/Folder Path]</p> <p>Voer het doelpad in of wijs dit toe aan het bestand of de map.</p> <p style="font-weight: bold;">[!UICONTROL File/Folder]</p> <p>Selecteer het bestand of de map in het menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Voer de doellocatie voor het bestand of de map in of wijs deze toe.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL New Name]</p> </td> 
   <td> <p>Voer de nieuwe naam voor het bestand of de map op de nieuwe locatie in.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Auto Rename]</p> </td> 
   <td> <p>Schakel deze optie in om ervoor te zorgen dat als er al een bestand of map met dezelfde naam bestaat, de module de naam van het nieuwe bestand of de nieuwe map wijzigt door ([!UICONTROL NUMBER]) na de bestands- of mapnaam. Anders wordt het bestand of de map op de doellocatie overschreven.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Allow ownership transfer]</p> </td> 
   <td> <p>Schakel deze optie in om verplaatsing door de eigenaar toe te staan, zelfs als dit zou leiden tot een eigendomsoverdracht voor de inhoud die wordt verplaatst.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rename a File/Folder]

In deze actiemodule wordt de naam van een bestand of map gewijzigd.

U geeft het bestand of de map en de nieuwe naam op.

De module retourneert de id van het bestand of de map en alle bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>Wijze waarop bestanden worden geselecteerd</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of invoeren, of selecteer het bestand handmatig.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Pad naar bestand/map/bestand/map</p> </td> 
   <td> <p style="font-weight: bold;">Pad naar bestand/map</p> <p>Voer het doelpad in of wijs dit toe aan het bestand of de map.</p> <p style="font-weight: bold;">Bestand/map</p> <p>Selecteer het bestand of de map in het menu.</p> </td> 
  </tr> 
  <tr> 
   <td>Naam wijzigen </td> 
   <td> <p>Voer de [!UICONTROL target name] voor het bestand, inclusief de bestandsextensie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File/Folder]

Met deze actiemodule verwijdert u een bestand of map.

U geeft het bestand of de map op.

De module retourneert de id van de record en de bijbehorende velden, samen met aangepaste velden en waarden die door de verbinding worden geopend. U kunt deze informatie in verdere modules in het scenario in kaart brengen.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Selecteer of u het bestandspad wilt toewijzen of invoeren, of selecteer het bestand handmatig.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Typ of wijs het doelpad naar het bestand toe.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Selecteer het bestand in het menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Overige modules

#### [!UICONTROL Make an API Call]

Deze actiemodule laat u een douane voor authentiek verklaarde vraag aan het maken [!DNL Dropbox] API. Op deze manier kunt u een automatisering van de gegevensstroom maken die niet door de ander kan worden uitgevoerd [!DNL Dropbox] modules.

Als u deze module configureert, worden de volgende velden weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw [!DNL Dropbox] account aan [!DNL Workfront Fusion], zie <a href="#create-a-connection-to-dropbox" class="MCXref xref">Verbinding maken met [!DNL Dropbox]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Een pad invoeren ten opzichte van een pad invoeren ten opzichte van <code>https://api.dropboxapi.com</code>. Bijvoorbeeld: <code>/2/files/list_folder</code></p> <p>Opmerking: raadpleeg de <a href="https://www.dropbox.com/developers/documentation/http/documentation">Dropbox API v2-documentatie</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Selecteer de HTTP- verzoekmethode u de API vraag moet vormen. Zie voor meer informatie <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-aanvraagmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>Voer de gewenste aanvraagheaders in. [!DNL Workfront Fusion] voegt automatisch machtigingsheaders toe.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p> Voer de queryreeks voor de aanvraag in.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Voeg de inhoud van de hoofdtekst voor de API-aanroep toe in de vorm van een standaard JSON-object.</p> <p>Opmerking:   <p>Bij het gebruik van voorwaardelijke instructies zoals <code>if</code> in uw JSON, plaats de aanhalingstekens buiten de voorwaardelijke verklaring.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Voorbeeld:** De volgende API-aanroep retourneert de eerste 10 bestanden van de [!DNL /Text files] in uw [!DNL Dropbox] account:
>
>URL: `/2/files/list_folder`
>
>Lichaam:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>De gelijken van het onderzoek kunnen in de Output van de module onder worden gevonden [!UICONTROL Bundle] > [!UICONTROL Body] > vermeldingen.
>
>In ons voorbeeld werden 10 tickets geretourneerd:

## Algemene problemen

* [Kan een bestand niet uploaden of bijwerken](#unable-to-upload-or-update-a-file)
* [Afbeeldingen waarnaar via een gedeelde koppeling wordt verwezen, worden niet gerenderd](#image-referenced-via-a-shared-link-does-not-render)

### Kan een bestand niet uploaden of bijwerken

Er zijn verschillende situaties wanneer het uploaden of bijwerken van een bestand mislukt:

* Het geüploade bestand is te groot en overschrijdt de maximaal toegestane bestandsgrootte voor uw [!DNL Dropbox] of u hebt al uw [!DNL Dropbox] opslagquotum van de account. U moet bestaande bestanden verwijderen uit uw [!DNL Dropbox] account of upgrade uw abonnement.
* De eerder geselecteerde map waarnaar het bestand wordt geüpload, bestaat niet meer. Het scenario stopt en u moet de doelmap opnieuw selecteren.

### Afbeeldingen waarnaar via een gedeelde koppeling wordt verwezen, worden niet gerenderd

De URL die door de [!UICONTROL Dropbox] >[!UICONTROL Create a shared link] niet rechtstreeks koppelen aan een afbeelding, maar aan een [!DNL Dropbox] pagina. Als u het downloaden van de afbeelding wilt forceren, vervangt u het navolgende `?dl=0` with `?dl=1`. Als u de afbeelding wilt renderen (bijvoorbeeld in een webbrowser of in Facebook Messenger), voegt u `&raw=1` naar de URL.

Als u de directe of onbewerkte koppeling naar uw afbeelding voor uw website of voor andere [!DNL Workfront Fusion] -modules, moet u de eerste gedeelde URL als volgt wijzigen:

Oorspronkelijke URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Vervangen `www` with `dl`.
1. Verwijderen `?dl=0`.

Uiteindelijke URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

Als u de URL automatisch wilt wijzigen, kunt u de opdracht `replace()` functie tweemaal:

* www door dl vervangen

  ![](assets/www-to-dl-350x32.png)

* En om ?dl=0 te verwijderen

  ![](assets/remove-dl0-350x33.png)

U kunt dit in één stap doen door de volgende functies te combineren:

![](assets/replace-both-350x47.png)

U kunt het ook kopiëren en in het veld plakken. Vervangen `1.url` met de URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
