---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Documenten van externe toepassingen koppelen
description: U kunt documenten en mappen vanuit externe bronnen koppelen aan Adobe Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: bec625b70b39fec9f9a6d4f7b48023702de43675
workflow-type: tm+mt
source-wordcount: '2563'
ht-degree: 0%

---

# Documenten van externe toepassingen koppelen

<!-- Audited: 01/2024 -->

U kunt documenten en mappen vanuit de volgende bronnen koppelen aan Adobe Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bestaande leveranciers van clouddocumenten van derden</td> 
   <td>Dit zijn onder andere: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>U kunt proefdrukken die oorspronkelijk zijn gemaakt met de Workfront-proefdrukken, beschikbaar maken in Workfront. Voor de huidige licenties is een Pro Workfront Plan of hoger vereist om deze functie te kunnen gebruiken. Voor de nieuwe vergunningen, omvatten alle plannen deze eigenschap. Zie voor meer informatie over de verschillende beschikbare plannen <a href="https://www.workfront.com/plans">Workfront-plannen</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>U kunt documenten vanuit Experience Manager Assets Essentials koppelen aan Workfront. Zie voor meer informatie <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">WORKFRONT DAM </td> 
   <td>Hiervoor is een extra aankoop vereist. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere documentproviders (via aangepaste documentintegratie)</td> 
   <td> <p class="workfront_plans">Voor de huidige licenties is een Pro Workfront Plan of hoger vereist om deze functie te kunnen gebruiken. Voor de nieuwe vergunningen, omvatten alle plannen deze eigenschap. Zie voor meer informatie over de verschillende beschikbare plannen <a href="https://www.workfront.com/plans">Workfront-plannen</a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Voordat u documenten of mappen koppelt, moet uw Workfront-beheerder deze functionaliteit inschakelen voor elke documentprovider of voor een aangepaste documentintegratie, zoals beschreven in [Documentintegratie configureren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Documenten die zijn gekoppeld aan een externe cloud, kunt u op dezelfde manier controleren en goedkeuren als documenten die rechtstreeks naar Workfront zijn geüpload.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td>
   <td> <p> Alle</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td>
   <td><p>Nieuw: Medewerker of hoger</p>
    <p>of</p>
    <p>Huidig: Verzoek of hoger</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Documentopslag

Documenten die vanuit een externe toepassing aan Workfront zijn gekoppeld, worden opgeslagen bij de externe cloud provider, niet in Workfront.

De volgende uitzonderingen zijn van toepassing:

* Als deze service de documentservice biedt, worden miniaturen en voorvertoningsafbeeldingen mogelijk opgeslagen op Workfront-servers.
* Wanneer u proef in Workfront gebruikt, wordt het document gekopieerd en toegevoegd aan de proefdrukservers.

## Een document van een externe toepassing koppelen aan Workfront

U kunt bestaande documenten koppelen aan een externe cloud provider. Dit geldt ook voor gedeelde documenten.

### Vereisten {#prerequisites}

Voordat u documenten of mappen koppelt, moet uw Workfront-beheerder deze functionaliteit inschakelen voor elke documentprovider of voor een aangepaste documentintegratie, zoals beschreven in [Documentintegratie configureren](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Een extern document koppelen aan Workfront {#link-an-external-document-to-workfront}

U kunt documenten vanuit een externe toepassing, zoals Google en Microsoft OneDrive, koppelen naar Workfront.

>[!IMPORTANT]
>
>Dropbox slaat documenten op op basis van het bestandspad. Hierdoor wordt een bestand dat is gekoppeld vanuit Dropbox, verplaatst, hernoemd of verwijderd, in Workfront ontoegankelijk.

1. Ga naar de **Documenten** in Workfront waar u het document wilt plaatsen.
1. Klikken **Nieuwe toevoegen** en klikt u op de externe documentprovider waar u documenten wilt koppelen aan Workfront.

   Als u bijvoorbeeld documenten van Dropbox wilt koppelen, klikt u op **Van Dropbox**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. (Voorwaardelijk) Als u wordt ertoe aangezet om in de externe dienst te registreren, typ uw login geloofsbrieven voor de dienst in het vakje dat verschijnt dan klik **Aanmelden**.
1. (Voorwaardelijk) Als u wordt gevraagd de externe toepassing te autoriseren, klikt u op de knop **Autoriseren** knop.

   Je hoeft dit maar één keer te doen.

1. In het zoekvak van het dialoogvenster **Externe bestanden en mappen koppelen** vak dat wordt weergegeven, typt u de naam van het item waarnaar u wilt zoeken en drukt u vervolgens op **Enter** om alle resultaten van de externe toepassing te zien, ongeacht in welke map ze zijn opgeslagen.

   of

   Blader naar de documenten die u wilt koppelen en selecteer deze.

   Hoewel u meerdere documenten kunt selecteren, worden alleen documenten die in de huidige weergave zijn geselecteerd, gekoppeld. Als u bijvoorbeeld een document selecteert en vervolgens naar een map gaat, wordt het oorspronkelijk geselecteerde document niet gekoppeld.

1. (Voorwaardelijk) Als u een Workfront DAM-klant bent, klikt u op **Miniatuur** om bestanden als miniatuurafbeeldingen weer te geven.

   >[!NOTE]
   >
   >Workfront DAM-klanten kunnen miniaturen weergeven wanneer ze documenten van Workfront DAM koppelen. Miniaturen kunnen ook worden weergegeven voor Workfront DAM-klanten voor andere services, zoals Dropbox en Box. Het weergeven van miniaturen voor andere services dan Workfront DAM in Workfront wordt echter niet ondersteund en er worden nooit miniaturen weergegeven wanneer u documenten koppelt van SharePoint of Google Drive.

1. Klikken **Koppeling**.

   In Workfront wordt het pictogram van de cloudprovider naast de documenten weergegeven.

   >[!NOTE]
   >
   >Voor documenten die zijn gekoppeld aan een vak, wordt de koppeling naar het document in het vak pas weergegeven als u de pagina vernieuwt.

### Een nieuwe versie van een gekoppeld document toevoegen {#add-a-new-version-of-a-linked-document}

U kunt vanuit een externe toepassing een nieuwe versie toevoegen van een document dat is gekoppeld aan Workfront.

1. Ga naar de **Documenten** Selecteer het gekoppelde document.

   >[!IMPORTANT]
   >
   >Het document moet zich buiten een gekoppelde map bevinden om een nieuwe versie te kunnen maken.

1. Klikken **Nieuwe toevoegen** > **Versie** en klikt u op de externe documentprovider.

   Als u bijvoorbeeld een nieuwe versie van een document vanuit Dropbox wilt koppelen, klikt u op **Van Dropbox**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. (Voorwaardelijk) Als u wordt ertoe aangezet om in de externe dienst te registreren, typ uw login geloofsbrieven voor de dienst in het vakje dat verschijnt dan klik **Aanmelden**.
1. (Voorwaardelijk) Als u wordt gevraagd de externe toepassing te autoriseren, klikt u op **Autoriseren**.

   Je hoeft dit maar één keer te doen.

1. In het zoekvak van het dialoogvenster **Externe bestanden en mappen koppelen** vak dat wordt weergegeven, typt u de naam van het item waarnaar u wilt zoeken en drukt u vervolgens op **Enter** om alle resultaten van de externe toepassing te zien, ongeacht in welke map ze zijn opgeslagen.

   of

   Blader naar de documenten die u wilt koppelen en selecteer deze.

   U kunt meerdere documenten selecteren, maar alleen documenten die in de huidige weergave zijn geselecteerd, worden gekoppeld. Als u bijvoorbeeld een document selecteert en vervolgens naar een map gaat, wordt het oorspronkelijk geselecteerde document niet gekoppeld.

1. (Voorwaardelijk) Als u een Workfront DAM-klant bent, klikt u op **Miniatuur** om bestanden als miniatuurafbeeldingen weer te geven.

   >[!NOTE]
   >
   >Workfront DAM-klanten kunnen miniaturen weergeven wanneer ze documenten van Workfront DAM koppelen. Miniaturen kunnen ook worden weergegeven voor Workfront DAM-klanten voor andere services, zoals Dropbox en Box. Het weergeven van miniaturen voor andere services dan Workfront DAM in Workfront wordt echter niet ondersteund en er worden nooit miniaturen weergegeven wanneer u documenten koppelt van SharePoint of Google Drive.

1. Klikken **Koppeling**.

   In Workfront verschijnt het pictogram van de cloudprovider naast de documenten om aan te geven dat deze zijn gekoppeld aan de externe cloudprovider.

   >[!NOTE]
   >
   >Voor documenten die zijn gekoppeld aan een vak, wordt de koppeling naar het document in het vak pas weergegeven als u de pagina vernieuwt.

Voor informatie over het toevoegen van een nieuwe versie van een document dat u vanuit uw bestandssysteem naar Workfront hebt geüpload, raadpleegt u [Documenten toevoegen aan Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) in [Documenten vanuit uw bestandssysteem toevoegen aan Adobe Workfront](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Workfront Proefdocumenten koppelen {#link-workfront-proof-documents}

U kunt proefdrukken koppelen aan Workfront die oorspronkelijk in Workfront Proof bestond. Als u een proefdruk van Workfront Proof koppelt, zijn alle opmerkingen en andere metagegevens die bij de proefdruk horen, beschikbaar in Workfront.

U kunt alleen proefdrukken koppelen waarvoor u toegang tot Weergave hebt in Workfront Proof.

1. Ga naar de **Documenten** in Workfront waar u het document wilt plaatsen.
1. Klikken **Nieuwe toevoegen** en klik vervolgens op **Proef van Workfront**.

   >[!NOTE]
   >
   >De opties in dit menu kunnen variëren afhankelijk van welke externe providers in uw omgeving zijn geconfigureerd.

1. In de **Proefdrukken van Workfront koppelen** Voer in het vak dat wordt weergegeven de naam in van de proefdruk die u in Workfront wilt aanbieden.

   De lijst wordt gefilterd terwijl u typt.

1. Selecteer maximaal 10 proefdrukken voor koppeling.

   Een grijze proefdruk is niet beschikbaar voor koppeling, omdat de proefdruk al is gekoppeld aan een document in Workfront.

1. Klikken **Koppeling**.

   De meest recente versie van de proefdruk is gekoppeld aan Workfront. Als u de proefdruk opent, zijn alle versies beschikbaar in de proefdrukviewer.

### Een Google-document maken vanuit Workfront {#create-a-google-document-from-within-workfront}

U kunt een nieuw Google-document maken vanuit Workfront. U kunt geen nieuwe documenten maken vanuit Workfront voor andere cloudproviders.

1. Ga naar de **Documenten** in Workfront waar u het document wilt plaatsen.
1. Klikken **Nieuwe toevoegen** > **Google-bestand** Selecteer vervolgens het type Google-document dat u wilt maken.
1. Als de **Google Drive-account toevoegen** wordt weergegeven, klikt u op **Google Drive autoriseren**.

   Een Google-document wordt toegevoegd aan de **Documenten** tab.

   >[!NOTE]
   >
   > Mijn Drive en Gedeeld met mij geven twee verschillende resultaten. Als u geen bestand kunt vinden in Mijn station, checkt u de map Gedeeld met mij in.

## Een document uploaden en koppelen van Workfront naar een externe cloud provider

U kunt een document van Workfront uploaden en koppelen aan een externe cloud provider. Hiermee wordt de opslag van het document verplaatst van Workfront naar de externe cloudprovider. Wanneer het document wordt gewijzigd in de externe toepassing, wordt het automatisch bijgewerkt in Workfront.

Gebruikers zonder Workfront-toegang kunnen het document in de externe toepassing zien als zij toegang hebben tot de toepassing.

1. Selecteer een document dat in Workfront is geüpload.
1. Klikken **Meer** >**Verzenden naar** selecteert u vervolgens de cloudprovider die u het gekoppelde document wilt opslaan.

   U kunt ook het menu Meer gebruiken ![](assets/more-icon.png) op de pagina Documentdetails om dit te doen.

1. Selecteer de map in de toepassing van de provider waarin u het document wilt opslaan.

   Dit kan elke map in de toepassing van de provider zijn, inclusief een gedeelde map.

1. Klikken **Opslaan**.

   Het logo van de externe provider wordt naast de documentnaam weergegeven om aan te geven dat het document nu is gekoppeld aan Workfront en is opgeslagen door de externe cloud provider.

   ![doc_with_google_drive_link_highlight__1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Mappen koppelen

Wanneer u een map koppelt tussen Workfront en een externe cloud provider, worden de map en alle inhoud ervan gekoppeld. Als gebruikers zonder Workfront-toegang bestanden toevoegen, verwijderen en wijzigen uit de externe documenttoepassing, worden de wijzigingen gesynchroniseerd met Workfront.

### Rechten voor maptoegang {#folder-access-rights}

Bij het synchroniseren van de mapinhoud van een externe documenttoepassing gebruikt Workfront de referenties van de gebruiker die oorspronkelijk de map had gekoppeld. Dit resulteert in de volgende gebruikerservaring:

* Als gebruikers geen toegang hebben tot bestanden en mappen in de externe toepassing, maar wel toegang hebben om de gekoppelde map via Workfront weer te geven, kunnen ze alleen de namen van de bestanden en mappen in Workfront bekijken, niet de inhoud ervan.
* Wanneer iemand toegang krijgt tot inhoud in een gekoppelde map in Workfront (zoals een submap in een gekoppelde map) die door een andere gebruiker aan Workfront is gekoppeld, wordt de inhoud gesynchroniseerd met Workfront met behulp van de Workfront-aanmeldingsgegevens van de gebruiker die de map oorspronkelijk heeft gekoppeld, niet met de gegevens van de gebruiker die de inhoud benadert.

>[!IMPORTANT]
>
>* Als de gebruiker die de map oorspronkelijk heeft gekoppeld, uit het Workfront-systeem wordt verwijderd, kunnen gebruikers geen inhoud meer openen in de gekoppelde map via Workfront. In dit geval moet de map opnieuw worden gekoppeld door een actieve Workfront-gebruiker die rechten heeft op de map in de externe toepassing.
>* Als de gebruiker die een map heeft gekoppeld, geen toegang meer heeft tot de externe toepassing, heeft Workfront geen toegang meer tot de inhoud van de map. Dit kan bijvoorbeeld gebeuren als de gebruiker die oorspronkelijk de map had gekoppeld het bedrijf verlaat. Een gebruiker met toegang tot de map moet de map opnieuw koppelen om ervoor te zorgen dat hij of zij toegang kan blijven krijgen.

### Een of meer externe mappen koppelen {#link-one-or-more-external-folders}

1. Ga naar het gebied in Workfront waar u de map wilt, en klik vervolgens op  **Documenten** ![](assets/document-icon.png) in het linkerdeelvenster.

1. Klikken **Nieuwe toevoegen** en klikt u vervolgens op de externe documentprovider vanwaar u een map wilt koppelen aan Workfront.
1. (Voorwaardelijk) Als u de externe service nog niet hebt geautoriseerd, geeft u uw aanmeldingsgegevens voor de externe provider op en klikt u op **Aanmelden**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. In de **Externe bestanden en mappen koppelen** Blader naar de mappen die u wilt koppelen en selecteer deze.

   of

   Typ de naam van de map waarnaar u wilt zoeken en druk op **Enter**.

   U kunt meerdere mappen selecteren, maar alleen de mappen die in de huidige weergave zijn geselecteerd, worden gekoppeld. Als u bijvoorbeeld een map selecteert en vervolgens naar een map gaat, wordt de oorspronkelijk geselecteerde map niet gekoppeld.

   >[!NOTE]
   >
   >Wanneer u mappen koppelt vanaf Google Drive, kunt u alleen mappen koppelen die zich op uw persoonlijke schijf (Mijn schijf) en op de teamschijf bevinden. U kunt geen mappen van het gebied Gedeeld met mij koppelen.

1. Klikken **Koppeling**.

   In Workfront wordt het logo van de cloudprovider naast de map weergegeven om aan te geven dat het is gekoppeld aan de externe cloudprovider.

1. (Optioneel) Als u de naam van de map wilt wijzigen zodat de mapnaam in Workfront afwijkt van de mapnaam in de externe documenttoepassing, selecteert u de map in het dialoogvenster **Mappen** klikt u op het menu Meer ![](assets/more-icon.png)  die naast de mapnaam wordt weergegeven, klikt u op **Naam wijzigen**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

Hierdoor wordt de naam van de map in de externe toepassing niet gewijzigd.

### Submappen toevoegen aan een gekoppelde map  {#add-subfolders-to-a-linked-folder}

U kunt een nieuwe map maken in een bestaande gekoppelde map. U kunt ook een andere map naar een bestaande gekoppelde map slepen.

1. Als u een nieuwe map in een bestaande gekoppelde map wilt maken, gaat u naar de bestaande map en maakt u de nieuwe map zoals beschreven in [Documentmappen maken](../../documents/organizing-documents/create-documents-folder.md).

   of

   Als u een bestaande map naar een bestaande gekoppelde map wilt slepen, gaat u naar het gebied Documenten waar u de submap wilt plaatsen en sleept u deze naar de gekoppelde map.

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >De volgende beperkingen zijn van toepassing wanneer u een bestaande Workfront-map naar een gekoppelde map sleept:
   >
   >* De map die u sleept, kan nog niet worden gekoppeld en kan geen inhoud bevatten die al is gekoppeld.
   >* De map (inclusief de inhoud) die u sleept, mag niet groter zijn dan 50 MB.

## Een document toevoegen aan een gekoppelde map

Als u via Workfront een document aan een gekoppelde map toevoegt, wordt dit automatisch toegevoegd als een gekoppeld document.

1. Selecteer de gekoppelde map waarin u het document wilt plaatsen en klik op **Nieuw toevoegen > Document** Blader vervolgens naar het document en voeg het toe aan de map.

   of

   In de **Documenten** in het gewenste gebied voor het document sleept u het document naar een gekoppelde map.

   Er wordt automatisch een nieuwe versie van het document gemaakt in de externe toepassing en gekoppeld aan Workfront.

>[!NOTE]
>
> * De documentopties zijn niet beschikbaar wanneer het document wordt verplaatst.
>
> * Nadat een document naar Experience Manager Assets is verplaatst, is het niet meer zichtbaar in de documentlijst in Workfront.
>
> * Handelingen of bewerkingen die u tijdens het verplaatsen op een document aanbrengt, worden niet in het document in Experience Manager Assets weergegeven en gaan daarom verloren.

## Een gekoppeld document of een gekoppelde map verwijderen

Wanneer u een gekoppeld document of een gekoppelde map uit de externe toepassing verwijdert, blijft het document of de map in het Workfront-systeem totdat u het document of de map ook uit Workfront verwijdert.

1. Selecteer het gekoppelde document of de gekoppelde map en klik op **Verwijderen**.
1. Klik in het bevestigingsvak dat wordt weergegeven op **Ja, ontkoppelen**.

   Het document is losgekoppeld van de Workfront-site. Dit wordt niet beïnvloed in de externe toepassing.

## Naam van gekoppelde documenten en mappen wijzigen

Wanneer u de naam van een gekoppeld document of een gekoppelde map wijzigt, is de wijziging alleen zichtbaar in de toepassing waarin u de naam hebt gewijzigd. Als u bijvoorbeeld de naam van een gekoppeld document wijzigt in Workfront, is de nieuwe naam alleen zichtbaar in Workfront.

Als u wilt dat de naam overeenkomt in Workfront en in de externe toepassing, moet u de naam op beide plaatsen wijzigen.

>[!IMPORTANT]
>
>Wijzig de naam van een document in Workfront dat is gekoppeld aan een Dropbox niet. Hierdoor is het bestand in Workfront niet toegankelijk. Wijzig in plaats daarvan de naam van het bestand in Dropbox en synchroniseer het bestand opnieuw.
