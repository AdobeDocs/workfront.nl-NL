---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Genereer proefdrukken in [!DNL Workfront Proof]
description: Met Workfront Proof kunt u proefdrukken maken van documenten of websites en deze proefdrukken met anderen delen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1818'
ht-degree: 0%

---

# Genereer proefdrukken in [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Dit artikel verwijst naar de functionaliteit in het standalone product [!DNL Workfront Proof]. Zie Proefdruk voor informatie over de proefdruk binnenin[!DNL Adobe Workfront][.](../../../review-and-approve-work/proofing/proofing.md)

Met [!DNL Workfront Proof] kunt u proefdrukken maken van documenten of websites en deze proefdrukken delen met anderen. In de volgende stappen worden de verschillende configuratieopties beschreven die beschikbaar zijn:

## Een proefdruk maken op basis van een document

1. Voer een van de volgende handelingen uit om de pagina **[!UICONTROL New Proof]** te openen:

   * Klik op de knop **[!UICONTROL New proof]** in de linkerbovenhoek van een pagina.
   * Verzenden via Dropzone (Enterprise-functie).

1. Als u een of meer documenten wilt proefdrukken, voegt u documenten toe die op een van de volgende manieren moeten worden gecontroleerd (herhaalt u dit proces om meerdere documenten toe te voegen):

   * Sleep een document van het bestandssysteem naar het gebied voor slepen en neerzetten in het **[!UICONTROL Add Files]** -gebied.
   * In het **[!UICONTROL Add Files]** gebied, klik **doorblader** verbinding om het document te vinden en te selecteren u van het dossiersysteem op uw werkstation wilt uploaden.

     ![ proof_document_upload.png ](assets/proof-document-upload-350x64.png)

1. Als u een website wilt controleren, voert u de URL van de website in het gebied **[!UICONTROL Add Files]** in en drukt u op **[!UICONTROL Enter]** . Herhaal deze stap om meerdere websites aan een proefdruk toe te voegen.

   Zie [Een proefdruk voor een URL](#generate-a-proof-for-a-url) genereren voor meer informatie over het controleren van websites.

   ![Bewijs website](assets/proof-website-350x65.png)

1. (Optioneel) Wijzig de bestandsnamen van geüploade bestanden:

   1. Plaats in de documentenlijst de muisaanwijzer op de documentnaam die u wilt wijzigen en klik vervolgens op het **[!UICONTROL Edit]** pictogram.

      ![ proof_edit.png ](assets/proof-edit-350x53.png)

   1. Geef in het veld **[!UICONTROL Proof name]** een nieuwe naam op en klik vervolgens op **[!UICONTROL Done]** .

   1. (Optioneel) Als u bestanden wilt verwijderen die u wilt uploaden, plaatst u de muisaanwijzer boven het document dat u wilt verwijderen in de documentlijst en klikt u op het pictogram **[!UICONTROL Delete]** .

      ![ proof_delete.png ](assets/proof-delete-350x53.png)

   1. (Optioneel) Schakel de optie **[!UICONTROL Combine all compatible files into single proof]** in.

      **wanneer deze optie wordt toegelaten:** Alle statische dossiers en websites zijn beschikbaar in één enkele proef, en u kunt tot 50 dossiers in een bepaalde tijd uploaden.

      >[!NOTE]
      >
      >Interactieve bestanden, zoals video&#39;s en interactieve websites, kunnen niet worden gecombineerd tot één proefdruk.

      **wanneer deze optie wordt onbruikbaar gemaakt:** Alle documenten en websites worden geproduceerd als individuele proeven, en u kunt tot 20 dossiers in een bepaald ogenblik uploaden.

      Alle geüploade bestanden en websites combineren in één proefdruk:

      1. Schakel de optie **[!UICONTROL Combine all compatible files into single proof]** in.
      1. Voer in het veld **[!UICONTROL Proof name]** een nieuwe naam in voor de gecombineerde proefdruk.
      1. Wijzig in het gebied **[!UICONTROL Add Files]** de volgorde van de opgenomen bestanden door een bestand in de gewenste volgorde te slepen. De volgorde van de bestanden is de paginavolgorde van de gecombineerde proefdruk. Voor meer informatie over het creëren van gecombineerde proeven, zie [ tot een multi-paginaproef ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) leiden.

1. (Optioneel) Als u een geautomatiseerde workflow wilt gebruiken die meerdere fasen omvat, selecteert u een van de volgende opties in de sectie **[!UICONTROL Workflow]** :

   * **Basis:** selecteer deze optie om gebruikers aan te wijzen die u toegang tot de proef onmiddellijk wilt hebben nadat het wordt gecreeerd. U kunt de proefdruk delen met meerdere gebruikers.

     Voor meer informatie over het delen van een proef, zie [ een proef binnen  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) delen.

   * **Geautomatiseerd:** selecteer deze optie om inhoudsoverzicht en goedkeuring te beheren wanneer u complexe overzichtsprocessen hebt, of als u inhoud voor overzicht naar de zelfde groepen regelmatig verzendt. Met een geautomatiseerde workflow wordt de proefdruk verplaatst van het werkgebied naar het werkgebied tot de definitieve goedkeuring. De betrokken gebruikers worden op elk moment op de hoogte gebracht dat zij een goedkeuring moeten verlenen.

     Voor meer informatie over het creëren van een Geautomatiseerd Werkschema, zie [ Opstelling een bewijs met een Geautomatiseerde Werkschema in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Geef op of u e-mailmeldingen en een aangepast bericht wilt verzenden naar de gebruikers die u in de vorige stap hebt geselecteerd:

   * **breng ontvangers op de hoogte over deze proef:** selecteer deze optie om een e-mailbericht naar gebruikers te verzenden. Wanneer **[!UICONTROL Basic sharing]** is geselecteerd in de **[!UICONTROL Workflow]** -sectie, wordt een e-mailmelding verzonden wanneer de proefdruk wordt gemaakt. Wanneer **[!UICONTROL Automated workflow]** is geselecteerd in de **[!UICONTROL Workflow]** -sectie, wordt een e-mailmelding verzonden wanneer de proefdruk het werkgebied van de geautomatiseerde workflow ingaat waaraan de gebruiker is gekoppeld.

   * **voeg douanebericht toe:** selecteer deze optie om een douanebericht in het bericht te omvatten. U kunt een onderwerp en berichttekst opgeven. De berichttekst kan tekstopmaak bevatten, zoals vet, opsommingstekens en hyperlinks.

1. Selecteer een van de volgende proefinstellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Inloggen vereist. Dit bewijs kan niet worden gedeeld met andere gebruikers</td> 
      <td> <p>Wanneer deze optie is geselecteerd:</p> 
       <ul> 
        <li>Gebruikers kunnen zich niet aanmelden bij de proefdruk om deze te bekijken, tenzij ze eraan zijn toegevoegd.</li> 
        <li>Abonnementen kunnen niet worden ingeschakeld.</li> 
       </ul> 
       <p>Deze optie is standaard uitgeschakeld.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend</td> 
      <td><p>Als deze optie is geselecteerd, moeten gebruikers hun gebruikersnaam en wachtwoord opgeven op het moment dat ze een beslissing nemen over een proefdruk.</p>
      <p>Deze optie is standaard uitgeschakeld.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bewijs vergrendelen wanneer alle vereiste beslissingen zijn genomen</td> 
      <td> <p>Als deze instelling is ingeschakeld, wordt de proefdrukstatus vergrendeld nadat alle beslissingen zijn genomen. De status wordt automatisch gewijzigd van ontgrendeld in vergrendeld wanneer de laatste fiatteur zijn beslissing neemt.</p> 
      <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Downloaden van het oorspronkelijke bestand toestaan</td> 
      <td> <p><strong></strong> Als deze optie is geselecteerd, kunnen revisoren het originele bestand downloaden van waaruit de proefdruk is gemaakt.</p> <p>Wanneer deze optie is uitgeschakeld, is het pictogram Downloaden niet meer zichtbaar.</p>
      <p>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Toestaan dat bewijs wordt gedeeld via openbare URL of insluitcode</td> 
      <td><p>Wanneer deze optie is geselecteerd, kan de proef worden gedeeld via een openbare URL of insluitcode.</p>
       <p>Deze optie is standaard ingeschakeld.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonneer op een proefversie via een openbare URL of insluitcode toestaan</td> 
      <td> <p>Als deze optie is geselecteerd, kunnen personen die niet aan de proefdruk zijn toegevoegd, zich abonneren op de proefdruk. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:</p> 
       <ul> 
        <li><strong> rol van de Abonnee </strong>: De standaardproefdrukrol die aan alle recensenten wordt toegewezen die aan de proef intekenen.</li> 
        <li><strong> e-mail waakzame montages voor abonnees </strong>: Het standaard e-mailalarm dat aan alle recensenten wordt toegewezen die aan de proef intekenen.</li> 
        <li> <p><strong> toegang van het Bewijs via e-mailverbinding die voor </strong> wordt vereist: Vorm of de abonnee een e-mail met een verbinding aan de proef ontvangt. U kunt <strong> Geen e-mail </strong> selecteren (de e-mailverbinding wordt niet vereist om tot de proef toegang te hebben), <strong> het bericht van het Bewijs slechts e-mail </strong> (de abonnee ontvangt een verbinding aan de proef via e-mail zonder enige controle), of <strong> Bevestiging en proefdrukbericht </strong> (de Abonnee ontvangt een verbinding aan de proef via e-mail en moet de verbinding klikken om tot een proef toegang te hebben. Het doel van deze optie is ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</p> <p>Opmerking: als voor de proefdrukken een geautomatiseerde workflow is bijgevoegd, worden bij alle abonnementen bevestigingse-mails naar de eigenaar van het bewijs gegenereerd, zodat deze kan bepalen in welk stadium de persoon moet worden toegevoegd.</p> </li> 
       </ul> 
        <p>Deze optie is standaard uitgeschakeld.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create Proof]**. Workfront genereert een proefdruk van de geselecteerde documenten of websites.

   De vertraging bij het uploaden van een document hangt af van de bestandsgrootte en het type. Het genereren van grotere bestanden duurt langer. U kunt vanaf de pagina navigeren terwijl Workfront uw bestand blijft genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

## Genereer een statische proef met een URL {#generate-a-proof-for-a-url}

U kunt een statische proef genereren met behulp van een website-URL.

>[!NOTE]
>
>U kunt alleen een interactieve proefdruk voor een URL genereren als uw [!DNL Workfront] omgeving is geïntegreerd met een [!DNL Workfront Proof] Premium-account. Neem contact op met de Workfront-beheerder als u geen proefdrukken kunt gebruiken zoals beschreven in deze sectie.

1. Voer een van de volgende handelingen uit om de pagina **[!UICONTROL New Proof]** te openen:

   * Klik op de knop **[!UICONTROL New proof]** in de linkerbovenhoek van een pagina.
   * Verzenden via Dropzone (Enterprise-functie).

1. In de **Nieuwe proef** pagina, ga URL van de website in u een proef van in het **[!UICONTROL Add Files]** gebied wilt tot stand brengen, dan druk **[!UICONTROL Enter]** of **[!UICONTROL Return]** op uw toetsenbord.

1. (Optioneel) Herhaal dit proces om meerdere websites aan de proefdruk toe te voegen.

   ![ proof_website.png ](assets/proof-website-350x65.png)

1. In het **[!UICONTROL Add Files]** gebied, klik **uitgeven** pictogram rechts van URL om de details van de websiteproef te openen.

   ![ proof_upload_website_modify.png ](assets/proof-upload-website-modify-350x185.png)

1. Voer een **[!UICONTROL Proof name]** in. Standaard is de proefdruknaam dezelfde als de URL van de site.

1. Selecteer een van de volgende **[!UICONTROL Handle site contents]** -opties:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Schermopname vastleggen</td> 
      <td>Maakt een proefdruk van een statische afbeelding van de voorpagina van de URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interactief</td> 
      <td> <p>Hiermee maakt u een proefdruk waarmee revisoren door de site kunnen navigeren, HTML5-afbeeldingen, Flash-elementen enzovoort kunnen bekijken.</p> <p>Als u een interactief proefdrukken wilt maken, moet de website worden gehost met een beveiligd protocol (https). Daarnaast kunnen websites die niet in een iframe kunnen worden ingesloten, niet worden gegenereerd als een interactieve proefdruk (beperkingen voor het insluiten van iframes worden bepaald door de website die u wilt insluiten).</p> <p>Nadat de eerste proefdruk is gemaakt, kan deze instelling niet worden gewijzigd wanneer u volgende versies maakt.</p> <p>Voor meer informatie over het interactieve proef, zie <a href="#generate-a-proof-for-interactive-content" class="MCXref xref"> een proef voor interactieve inhoud </a> produceren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schermresolutie</td> 
      <td> <p>(Deze optie is niet beschikbaar voor interactieve proefdrukken.) U kunt de resolutie aanpassen waarin uw inhoud wordt weergegeven, of u kunt meerdere resoluties selecteren.</p> <p>Hierdoor kunnen gebruikers de proefdruk controleren om te zien hoe inhoud op verschillende apparaten, zoals verschillende formaten telefoons, tablets en monitoren, wordt weergegeven.</p> <p>Als u meerdere resoluties selecteert, wordt voor elke resolutie die u selecteert een afzonderlijke proefdruk gemaakt.</p> <p>Wanneer gebruikers opmerkingen plaatsen over de proefdruk, wordt de huidige schermresolutie automatisch weergegeven in de opmerking om ervoor te zorgen dat andere gebruikers weten met welke resolutie de opmerking wordt geassocieerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zoeken naar subpagina's</td> 
      <td>(Deze optie is niet beschikbaar voor interactieve proefdrukken.) Selecteer deze optie om door pagina's van de website te navigeren. U kunt de website tot 2 niveaus diep van de hoofdpagina uitbreiden. Houd de muisaanwijzer boven een pagina om de URL van de pagina weer te geven en selecteer alleen de pagina's die u wilt controleren. Elke pagina die u selecteert, wordt standaard gemaakt als een afzonderlijke proefdruk. Alternatief, kunt u <strong> toelaten combineren alle compatibele dossiers in enige proefdruk </strong> optie.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Configureer eventuele geavanceerde opties voor proefdrukken, zoals het delen van de proefdruk, het toevoegen van een geautomatiseerde workflow of het instellen van toegangs- en abonnementsinstellingen. Raadpleeg de volgende artikelen voor meer informatie over deze opties:

   * [Een proefdruk delen binnen  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Opstelling een proef met een Geautomatiseerde Werkschema in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Toegang- en abonnementsinstellingen configureren voor een proefdruk](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klik op **[!UICONTROL Done]**.

1. Klik op **[!UICONTROL Create Proof]**.

## Een proefdruk maken voor interactieve inhoud {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Voor meer informatie over Interactieve inhoud, zie [ Interactieve inhoudsproeven overzicht ](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Interactieve inhoud toevoegen als een URL](#add-interactive-content-as-a-url)
* [Interactieve inhoud toevoegen als ZIP-bestand](#add-interactive-content-as-a-zip-file)

### Interactieve inhoud toevoegen als een URL {#add-interactive-content-as-a-url}

Voor informatie over hoe te om een interactieve proef toe te voegen URL, zie [ een proef voor een URL ](#generate-a-proof-for-a-url) produceren.

### Interactieve inhoud toevoegen als ZIP-bestand {#add-interactive-content-as-a-zip-file}

1. Bereid uw inhoud voor door een ZIP-gebundeld bestand te maken.

   Zie [Overzicht](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md) van interactieve inhoudsproeven voor informatie over .zip gebundelde bestandsspecificaties.

1. Voer een van de volgende handelingen uit om de **[!UICONTROL New Proof]** pagina te openen:

   * Klik op de **[!UICONTROL New proof]** knop in de linkerbovenhoek van een pagina.
   * Indienen via Dropzone (Enterprise-functie).

1. Sleep op de pagina **[!UICONTROL New proof]** de interactieve ZIP-bundel naar het **[!UICONTROL Add files]** -gebied.

1. (Optioneel) Configureer eventuele geavanceerde opties voor proefdrukken, zoals het delen van de proefdruk, het toevoegen van een geautomatiseerde workflow of het instellen van toegangs- en abonnementsinstellingen. Raadpleeg de volgende artikelen voor meer informatie over deze opties:

   * [Een proefdruk delen binnen  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Toegang- en abonnementsinstellingen configureren voor een proefdruk](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klik op **[!UICONTROL Create Proof]**. Workfront genereert een proefdruk van het ZIP-bestand.

   De vertraging bij het uploaden van een document hangt af van de grootte van het ZIP-bestand. U kunt vanaf de pagina navigeren terwijl Workfront uw bestand blijft genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.
