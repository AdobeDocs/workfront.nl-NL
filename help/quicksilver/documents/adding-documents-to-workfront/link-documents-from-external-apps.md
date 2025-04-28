---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Documenten van externe toepassingen koppelen
description: U kunt documenten en mappen vanuit externe bronnen koppelen aan Adobe Workfront.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '2620'
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
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront Proof </td> 
   <td>U kunt proefdrukken die oorspronkelijk in Workfront Proof zijn gemaakt, beschikbaar maken in Workfront. Voor de huidige licenties is een Pro Workfront Plan of hoger vereist om deze functie te kunnen gebruiken. Voor de nieuwe vergunningen, omvatten alle plannen deze eigenschap. Voor meer informatie over de diverse beschikbare plannen, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Abonnementen van Workfront </a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>U kunt documenten vanuit Experience Manager Assets Essentials koppelen aan Workfront. Zie <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials </a> voor meer informatie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">WORKFRONT DAM </td> 
   <td>Hiervoor is een extra aankoop vereist. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere documentproviders (via aangepaste documentintegratie)</td> 
   <td> <p class="workfront_plans">Voor de huidige licenties is een Pro Workfront Plan of hoger vereist om deze functie te kunnen gebruiken. Voor de nieuwe vergunningen, omvatten alle plannen deze eigenschap. Voor meer informatie over de diverse beschikbare plannen, zie <a href="https://business.adobe.com/products/workfront/pricing.html"> Abonnementen van Workfront </a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Alvorens u documenten of omslagen verbindt, moet uw beheerder van Workfront deze functionaliteit voor elke documentleverancier, of voor een integratie van het douanedocument toelaten, zoals die in [ wordt beschreven vormt documentintegraties ](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

Documenten die zijn gekoppeld aan een externe cloud, kunt u op dezelfde manier controleren en goedkeuren als documenten die rechtstreeks naar Workfront zijn geüpload.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Documentopslag

Documenten die vanuit een externe toepassing aan Workfront zijn gekoppeld, worden opgeslagen bij de externe cloud provider, niet in Workfront.

De volgende uitzonderingen zijn van toepassing:

* Als deze service de documentservice biedt, worden miniaturen en voorvertoningsafbeeldingen mogelijk opgeslagen op Workfront-servers.
* Wanneer u proef in Workfront gebruikt, wordt het document gekopieerd en toegevoegd aan de proefdrukservers.

## Een document van een externe toepassing koppelen aan Workfront

U kunt bestaande documenten koppelen aan een externe cloud provider. Dit geldt ook voor gedeelde documenten.

### Vereisten {#prerequisites}

Alvorens u documenten of omslagen verbindt, moet uw beheerder van Workfront deze functionaliteit voor elke documentleverancier, of voor een integratie van het douanedocument toelaten, zoals die in [ wordt beschreven vormt documentintegraties ](../../administration-and-setup/configure-integrations/configure-document-integrations.md).

### Een extern document koppelen aan Workfront {#link-an-external-document-to-workfront}

U kunt documenten vanuit een externe toepassing, zoals Google en Microsoft OneDrive, koppelen naar Workfront.

>[!IMPORTANT]
>
>Dropbox slaat documenten op op basis van het bestandspad. Hierdoor wordt een bestand dat is gekoppeld vanuit Dropbox verplaatst, hernoemd of verwijderd, in Workfront ontoegankelijk.

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt.
1. Klik **toevoegen Nieuw**, dan klik de externe documentleverancier waar u documenten aan Workfront wilt verbinden.

   Bijvoorbeeld, om documenten van Dropbox te verbinden, klik **van Dropbox**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. (Voorwaardelijk) als u wordt ertoe aangezet om in de externe dienst te registreren, typ uw login geloofsbrieven voor de dienst in de doos die verschijnt, dan klik **binnen Teken**.
1. (Voorwaardelijk) als u wordt ertoe aangezet om de externe toepassing te machtigen, klik **machtigt** knoop.

   Je hoeft dit maar één keer te doen.

1. In het onderzoeksvakje van de **Verbinding Externe Dossiers en Omslagen** doos die verschijnt, typ de naam van het punt u wilt zoeken, dan **binnengaan** om alle resultaten van de externe toepassing te zien, ongeacht welke omslag zij binnen worden opgeslagen.

   of

   Blader naar de documenten die u wilt koppelen en selecteer deze.

   Hoewel u meerdere documenten kunt selecteren, worden alleen documenten die in de huidige weergave zijn geselecteerd, gekoppeld. Als u bijvoorbeeld een document selecteert en vervolgens naar een map gaat, wordt het oorspronkelijk geselecteerde document niet gekoppeld.

1. (Voorwaardelijk) als u een klant van Workfront DAM bent, klik het **pictogram van de Duimnagel** om dossiers als duimnagelbeelden te tonen.

   >[!NOTE]
   >
   >Workfront DAM-klanten kunnen miniaturen weergeven wanneer ze documenten van Workfront DAM koppelen. Miniaturen kunnen ook worden weergegeven voor Workfront DAM-klanten voor andere services, zoals Dropbox en Box. Het weergeven van miniaturen voor andere services dan Workfront DAM in Workfront wordt echter niet ondersteund en er worden nooit miniaturen weergegeven wanneer u documenten koppelt van SharePoint of Google Drive.

1. Klik **Verbinding**.

   In Workfront wordt het pictogram van de cloudprovider naast de documenten weergegeven.

   >[!NOTE]
   >
   >* Als de download-URL waarmee het document wordt gekoppeld, meer dan 2048 tekens bevat, kan het bestand niet worden gekoppeld.
   >* Voor documenten die zijn gekoppeld aan een vak, wordt de koppeling naar het document in het vak pas weergegeven als u de pagina vernieuwt.

### Een nieuwe versie van een gekoppeld document toevoegen {#add-a-new-version-of-a-linked-document}

U kunt vanuit een externe toepassing een nieuwe versie toevoegen van een document dat is gekoppeld aan Workfront.

1. Ga naar het **gebied van Documenten** waar het document verbonden is, dan selecteer het verbonden document.

   >[!IMPORTANT]
   >
   >Het document moet zich buiten een gekoppelde map bevinden om een nieuwe versie te kunnen maken.

1. Klik **toevoegen Nieuw** > **Versie**, dan klik de externe documentleverancier.

   Bijvoorbeeld, om een nieuwe versie van een document van Dropbox te verbinden, klik **van Dropbox**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. (Voorwaardelijk) als u wordt ertoe aangezet om in de externe dienst te registreren, typ uw login geloofsbrieven voor de dienst in de doos die verschijnt, dan klik **binnen Teken**.
1. (Voorwaardelijk) als u wordt ertoe aangezet om de externe toepassing toe te staan, klik **machtigt**.

   Je hoeft dit maar één keer te doen.

1. In het onderzoeksvakje van de **Verbinding Externe Dossiers en Omslagen** doos die verschijnt, typ de naam van het punt u wilt zoeken, dan **binnengaan** om alle resultaten van de externe toepassing te zien, ongeacht welke omslag zij binnen worden opgeslagen.

   of

   Blader naar de documenten die u wilt koppelen en selecteer deze.

   U kunt meerdere documenten selecteren, maar alleen documenten die in de huidige weergave zijn geselecteerd, worden gekoppeld. Als u bijvoorbeeld een document selecteert en vervolgens naar een map gaat, wordt het oorspronkelijk geselecteerde document niet gekoppeld.

1. (Voorwaardelijk) als u een klant van Workfront DAM bent, klik het **pictogram van de Duimnagel** om dossiers als duimnagelbeelden te tonen.

   >[!NOTE]
   >
   >Workfront DAM-klanten kunnen miniaturen weergeven wanneer ze documenten van Workfront DAM koppelen. Miniaturen kunnen ook worden weergegeven voor Workfront DAM-klanten voor andere services, zoals Dropbox en Box. Het weergeven van miniaturen voor andere services dan Workfront DAM in Workfront wordt echter niet ondersteund en er worden nooit miniaturen weergegeven wanneer u documenten koppelt van SharePoint of Google Drive.

1. Klik **Verbinding**.

   In Workfront verschijnt het pictogram van de cloudprovider naast de documenten om aan te geven dat deze zijn gekoppeld aan de externe cloudprovider.

   >[!NOTE]
   >
   >Voor documenten die zijn gekoppeld aan een vak, wordt de koppeling naar het document in het vak pas weergegeven als u de pagina vernieuwt.

Voor informatie over het toevoegen van nieuwe versie van een document u aan Workfront van uw dossiersysteem hebt geupload, zie [ documenten aan Adobe Workfront ](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) in [ toevoegen documenten aan Adobe Workfront van uw dossiersysteem ](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Workfront Proof-documenten koppelen {#link-workfront-proof-documents}

U kunt proefdrukken koppelen aan Workfront die oorspronkelijk in Workfront Proof bestonden. Als u een proefdruk van Workfront Proof koppelt, zijn alle opmerkingen en andere metagegevens die bij de proefdruk horen, beschikbaar in Workfront.

U kunt alleen proefdrukken koppelen waarvoor u in Workfront Proof toegang tot Weergave hebt.

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt.
1. Klik **toevoegen Nieuw**, dan klik **van Workfront Proof**.

   >[!NOTE]
   >
   >De opties in dit menu kunnen variëren afhankelijk van welke externe providers in uw omgeving zijn geconfigureerd.

1. In de **proefdrukken van de Verbinding van Workfront Proof** doos die verschijnt, begin typend de naam van de proef u in Workfront beschikbaar wilt maken.

   De lijst wordt gefilterd terwijl u typt.

1. Selecteer maximaal 10 proefdrukken voor koppeling.

   Een grijze proefdruk is niet beschikbaar voor koppeling, omdat de proefdruk al is gekoppeld aan een document in Workfront.

1. Klik **Verbinding**.

   De meest recente versie van de proefdruk is gekoppeld aan Workfront. Als u de proefdruk opent, zijn alle versies beschikbaar in de proefdrukviewer.

### Een Google-document maken vanuit Workfront {#create-a-google-document-from-within-workfront}

U kunt een nieuw Google-document maken vanuit Workfront. U kunt geen nieuwe documenten maken vanuit Workfront voor andere cloudproviders.

1. Ga naar het **gebied van Documenten** in Workfront waar u het document wilt.
1. Klik **toevoegen Nieuw** > **het Dossier van Google**, dan selecteren het type van het document van Google u wilt creëren.
1. Als **de Rekening van de Aandrijving van Google** verschijnt, klik **autoriseer de Aandrijving van Google**.

   Een document van Google wordt toegevoegd aan de **Documenten** tabel.

   >[!NOTE]
   >
   > Mijn Drive en Gedeeld met mij geven twee verschillende resultaten. Als u geen bestand kunt vinden in Mijn station, checkt u de map Gedeeld met mij in.

## Een document uploaden en koppelen van Workfront naar een externe cloud provider

U kunt een document van Workfront uploaden en koppelen aan een externe cloud provider. Hiermee wordt de opslag van het document verplaatst van Workfront naar de externe cloudprovider. Wanneer het document wordt gewijzigd in de externe toepassing, wordt het automatisch bijgewerkt in Workfront.

>[!NOTE]
>
>Door een element naar een externe documentprovider te verzenden, maakt u een nieuwe versie van het element.

Gebruikers zonder Workfront-toegang kunnen het document in de externe toepassing zien als zij toegang hebben tot de toepassing.

1. Selecteer een document dat in Workfront is geüpload.
1. Klik **Meer** > **verzenden naar**, dan selecteer de wolkenleverancier die u het verbonden document wilt opslaan.

   U kunt het Meer menu ![ Meer menu ](assets/more-icon.png) op de pagina van de Details van het Document ook gebruiken om dit te doen.

1. Selecteer de map in de toepassing van de provider waarin u het document wilt opslaan.

   Dit kan elke map in de toepassing van de provider zijn, inclusief een gedeelde map.

1. Klik **sparen**.

   Het logo van de externe provider wordt naast de documentnaam weergegeven om aan te geven dat het document nu is gekoppeld aan Workfront en is opgeslagen door de externe cloud provider.

   ![ doc_with_google_drive_link_highlight__1_.png ](assets/doc-with-google-drive-link-highlight--1--350x66.png)

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

1. Ga naar het gebied in Workfront waar u de omslag wilt, dan klik **![ het pictogram van Documenten ](assets/document-icon.png) in het linkerpaneel van Documenten**.

1. Klik **toevoegen Nieuw**, dan klik de externe documentleverancier waarvan u een omslag aan Workfront wilt verbinden.
1. (Voorwaardelijk) als u de externe dienst nog niet hebt geautoriseerd, specificeer uw login geloofsbrieven voor de externe leverancier, dan klik binnen **Teken**.

   Externe providers die u al hebt geautoriseerd, worden boven aan de lijst weergegeven.

1. In het **vakje van de Verbinding Externe Dossiers en Omslagen** dat verschijnt, doorblader aan en selecteer de omslagen u wilt verbinden.

   of

   Typ de naam van de omslag u wilt zoeken, dan **ingaan** drukken.

   U kunt meerdere mappen selecteren, maar alleen de mappen die in de huidige weergave zijn geselecteerd, worden gekoppeld. Als u bijvoorbeeld een map selecteert en vervolgens naar een map gaat, wordt de oorspronkelijk geselecteerde map niet gekoppeld.

   >[!NOTE]
   >
   >Wanneer u mappen koppelt vanaf Google Drive, kunt u alleen mappen koppelen die zich op uw persoonlijke schijf (Mijn schijf) en op de teamschijf bevinden. U kunt geen mappen van het gebied Gedeeld met mij koppelen.

1. Klik **Verbinding**.

   In Workfront wordt het logo van de cloudprovider naast de map weergegeven om aan te geven dat het is gekoppeld aan de externe cloudprovider.

1. (Facultatief) om de omslag anders te noemen zodat de omslagnaam in Workfront van de omslagnaam in de externe documenttoepassing verschillend is, selecteer de omslag in de **sectie 0} Omslagen {, klik het Meer menu ![ Meer ](assets/more-icon.png) dat naast de omslagnaam toont, dan** anders noemt **klikt.**

   ![ noem omslag anders ](assets/documents-folderlink-rename-nwe-350x154.png)

Hierdoor wordt de naam van de map in de externe toepassing niet gewijzigd.

### Submappen toevoegen aan een gekoppelde map  {#add-subfolders-to-a-linked-folder}

U kunt een nieuwe map maken in een bestaande gekoppelde map. U kunt ook een andere map naar een bestaande gekoppelde map slepen.

1. Om een nieuwe omslag binnen een bestaande verbonden omslag tot stand te brengen, ga naar de bestaande omslag, dan creeer de nieuwe omslag zoals die in [ wordt beschreven creeer documentomslagen ](../../documents/organizing-documents/create-documents-folder.md).

   of

   Als u een bestaande map naar een bestaande gekoppelde map wilt slepen, gaat u naar het gebied Documenten waar u de submap wilt plaatsen en sleept u deze naar de gekoppelde map.

   ![ Belemmering in verbonden omslag ](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >De volgende beperkingen zijn van toepassing wanneer u een bestaande Workfront-map naar een gekoppelde map sleept:
   >
   >* De map die u sleept, kan nog niet worden gekoppeld en kan geen inhoud bevatten die al is gekoppeld.
   >* De map (inclusief de inhoud) die u sleept, mag niet groter zijn dan 50 MB.

## Een document toevoegen aan een gekoppelde map

Als u via Workfront een document aan een gekoppelde map toevoegt, wordt dit automatisch toegevoegd als een gekoppeld document.

1. Selecteer de verbonden omslag waar u het document wilt, **toevoegen Nieuw > Document**, dan doorbladeren aan het document en het toevoegen aan de omslag.

   of

   In het **gebied van Documenten** waar u het document wilt, sleep het document in een verbonden omslag.

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

1. Selecteer het verbonden document of de omslag, dan klik **Schrapping**.
1. In het bevestigingsvakje dat verschijnt, klik ja **, ontkoppel het**.

   Het document is losgekoppeld van de Workfront-site. Dit wordt niet beïnvloed in de externe toepassing.

## Naam van gekoppelde documenten en mappen wijzigen

Wanneer u de naam van een gekoppeld document of een gekoppelde map wijzigt, is de wijziging alleen zichtbaar in de toepassing waarin u de naam hebt gewijzigd. Als u bijvoorbeeld de naam van een gekoppeld document wijzigt in Workfront, is de nieuwe naam alleen zichtbaar in Workfront.

Als u wilt dat de naam overeenkomt in Workfront en in de externe toepassing, moet u de naam op beide plaatsen wijzigen.

>[!IMPORTANT]
>
>Wijzig de naam van een document in Workfront dat is gekoppeld aan Dropbox niet. Hierdoor is het bestand in Workfront niet toegankelijk. Wijzig in plaats daarvan de naam van het bestand in Dropbox en synchroniseer het bestand opnieuw.
