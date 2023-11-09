---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Proefdrukken genereren in [!DNL Workfront Proof]
description: Met Workfront Proof kunt u proefdrukken maken van documenten of websites en deze proefdrukken delen met anderen.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '2156'
ht-degree: 0%

---

# Proefdrukken genereren in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het standalone product [!DNL Workfront Proof]. Voor informatie over proefdrukken binnen [!DNL Adobe Workfront], zie [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] kunt u proefdrukken maken van documenten of websites en deze proefdrukken delen met anderen. In de volgende stappen worden de verschillende configuratieopties beschreven die beschikbaar zijn:

## Een proefdruk maken voor een document

1. Voer een van de volgende handelingen uit om een nieuwe proefdruk te maken en de [!UICONTROL New Proof] pagina:

   * Klik op groen **[!UICONTROL New proof]** in de linkerbovenhoek van een pagina.
   * In de **[!UICONTROL Dashboard]** in het gebied **[!UICONTROL Overview]** klikt u op de knop **[!UICONTROL New proof]** koppeling.

   * Verzenden via Dropzone (Enterprise-functie).
   * De **[!UICONTROL New Proof]** wordt weergegeven.

1. Als u een of meer documenten wilt proefdrukken, voegt u documenten toe die op een van de volgende manieren moeten worden gecontroleerd (herhaalt u dit proces om meerdere te controleren documenten toe te voegen):

   * Sleep een document van uw bestandssysteem naar het gebied voor slepen en neerzetten in het dialoogvenster **[!UICONTROL Add Files]** gebied.
   * Klik in het gebied voor slepen en neerzetten van het dialoogvenster **[!UICONTROL Add Files]** , bladert u naar het document dat u wilt uploaden en selecteert u het in het bestandssysteem op uw werkstation.

     ![proefdruk_document_upload.png](assets/proof-document-upload-350x64.png)

1. Als u een of meer websites wilt controleren, geeft u de URL op van de website die u wilt controleren in het dialoogvenster **[!UICONTROL Add Files]** gebied, dan drukken **[!UICONTROL Enter]**.

1. (Optioneel) Herhaal dit proces om meerdere websites aan een proefdruk toe te voegen.

   Ga voor meer informatie over het controleren van websites naar [Een proef voor een URL genereren](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Optioneel) Wijzig de bestandsnamen van geüploade bestanden:

   1. Plaats de muis boven de documentnaam die u wilt wijzigen in de documentlijst in het dialoogvenster **[!UICONTROL Add Files]** en klik vervolgens op de knop **[!UICONTROL Edit]** pictogram.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. In de **[!UICONTROL Proof name]** veld, geef een nieuwe naam op en klik vervolgens op **[!UICONTROL Done]**.

   1. (Optioneel) Als u bestanden wilt verwijderen die u wilt uploaden, plaatst u de muis boven het document dat u wilt verwijderen in de documentlijst in het dialoogvenster **[!UICONTROL Add Files]** en klik vervolgens op de knop **[!UICONTROL Delete]** pictogram.

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Optioneel) Schakel de optie in. **[!UICONTROL Combine all compatible files into single proof]**.

      **Wanneer deze optie is ingeschakeld:** Alle statische bestanden en websites zijn beschikbaar in één proefdruk en u kunt maximaal 50 bestanden tegelijk uploaden.

      >[!NOTE]
      >
      >Interactieve bestanden, zoals video&#39;s en interactieve websites, kunnen niet worden gecombineerd tot één proefdruk.

      **Wanneer deze optie is uitgeschakeld:** Alle documenten en websites worden gegenereerd als afzonderlijke proefdrukken en u kunt maximaal 20 bestanden tegelijk uploaden.

      Alle geüploade bestanden en websites combineren in één proefdruk:

      1. Schakel de optie in. **[!UICONTROL Combine all compatible files into single proof]**.
      1. In de **[!UICONTROL Proof name]** geeft u een nieuwe naam op voor de gecombineerde proefdruk.
      1. In de **[!UICONTROL Add Files]** , wijzigt u de volgorde van de opgenomen bestanden door een bestand naar de gewenste volgorde te slepen. De volgorde van de bestanden is de paginavolgorde van de gecombineerde proefdruk. Zie voor meer informatie over het maken van gecombineerde proefdrukken [Een proefdruk van meerdere pagina&#39;s maken](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Optioneel) Als u een geautomatiseerde workflow wilt gebruiken die meerdere fasen omvat, kunt u de opdracht **[!UICONTROL Workflow]** selecteert u een van de volgende opties:

   * **Eenvoudig:** Schakel deze optie in om gebruikers aan te wijzen die toegang moeten hebben tot de proefdruk direct nadat deze is gemaakt. U kunt de proefdruk delen met meerdere gebruikers.

     Zie &quot;Gebruikers aan een proef toevoegen&quot; in voor meer informatie over het delen van een proefdruk. [Een proefdruk delen binnen [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatisch:** Selecteer deze optie om de controle en goedkeuring van inhoud te beheren wanneer u complexe revisieprocessen hebt of als u inhoud ter controle regelmatig naar dezelfde groepen personen verzendt. Met de geautomatiseerde workflow wordt de proefdruk verplaatst van het werkgebied naar het werkgebied tot de definitieve goedkeuring. De relevante gebruikers worden op elk moment dat zij een goedkeuring moeten verlenen, op de hoogte gebracht.

     Voor meer informatie over het creëren van een Geautomatiseerde Workflow, zie [Stel een proefdruk in met een geautomatiseerde workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Geef op of u e-mailmeldingen en een aangepast bericht wilt verzenden naar de gebruikers die u in de vorige stap hebt geselecteerd:

   * **Ontvangers op de hoogte stellen van dit bewijs:** Selecteer deze optie om een e-mailbericht naar gebruikers te verzenden. Wanneer **[!UICONTROL Basic sharing]** is geselecteerd in het dialoogvenster **[!UICONTROL Workflow]** een e-mailmelding verzendt wanneer de proefdruk wordt gemaakt. Wanneer **[!UICONTROL Automated workflow]** is geselecteerd in het dialoogvenster **[!UICONTROL Workflow]** , wordt een e-mailmelding verzonden wanneer de proefdruk het werkgebied van de geautomatiseerde workflow bereikt waaraan de gebruiker is gekoppeld.

   * **Aangepast bericht toevoegen:** Selecteer deze optie om een aangepast bericht op te nemen in het bericht. U kunt een onderwerp en berichttekst opgeven. De berichttekst kan tekstopmaak bevatten, zoals vet, opsommingstekens en hyperlinks.

1. Selecteer een van de volgende proefdrukinstellingen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aanmelding vereisen - proefdruk kan alleen worden gedeeld met andere gebruikers</td> 
      <td> <p><strong>Aanmelding vereisen - proefdruk kan alleen worden gedeeld met andere gebruikers:</strong> Als deze optie is geselecteerd, alleen [!DNL Workfront Proof] gebruikers kunnen de proefdruk bekijken.</p> <p>Deze optie is standaard uitgeschakeld. Iedereen met de URL kan de proefdruk bekijken.</p> <p>Wanneer deze optie is geselecteerd:</p> 
       <ul> 
        <li>Gebruikers kunnen zich alleen aanmelden bij de proefdruk als ze aan de proefdruk zijn toegevoegd.</li> 
        <li>Abonnementen kunnen niet worden ingeschakeld.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Slechts één besluit vereist voor dit bewijs</td> 
      <td> <p>Wanneer deze optie is geselecteerd, wordt de evaluatie voltooid nadat een van de besluitvormers zijn besluit heeft genomen.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend</td> 
      <td>Gebruikers moeten hun gebruikersnaam en wachtwoord opgeven op het moment dat zij een beslissing nemen over een bewijs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bewijs vergrendelen wanneer alle vereiste beslissingen zijn genomen</td> 
      <td> <p><strong></strong> Als deze instelling is ingeschakeld, wordt de proefdrukstatus vergrendeld nadat alle beslissingen zijn genomen. De status wordt automatisch gewijzigd van ontgrendeld in vergrendeld wanneer de laatste fiatteur zijn beslissing neemt.</p> <p>Deze optie is standaard uitgeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Origineel bestand downloaden</td> 
      <td> <p><strong></strong> Als deze optie is geselecteerd, kunnen revisoren het originele bestand downloaden van waaruit de proefdruk is gemaakt.</p> <p>Wanneer deze optie is uitgeschakeld, is het pictogram Downloaden niet meer zichtbaar.<br>Deze optie is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proef delen via openbare URL of insluitcode</td> 
      <td>Als deze optie is geselecteerd, kan de proefdruk worden gedeeld via een openbare URL of insluitcode.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonneren op bewijs via openbare URL of insluitcode</td> 
      <td> <p>Als deze optie is geselecteerd, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich op de proefdruk abonneren. De persoon die zich op de proef abonneert, krijgt de rol en e-mail die u in de volgende montages bepaalt:</p> 
       <ul> 
        <li><strong>Abonnementsrol</strong>: De standaardproefdrukrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li> 
        <li><strong>Instellingen voor e-mailwaarschuwingen voor abonnees</strong>: De standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li> 
        <li> <p><strong>Toegang tot bewijs via e-mailkoppeling vereist voor</strong>: Configureer of de abonnee een e-mail ontvangt met een koppeling naar de proefdruk. U kunt <strong>Geen e-mail</strong> (E-mailkoppeling is niet vereist voor toegang tot de proefdruk), <strong>Alleen e-mail met verificatie</strong> (de abonnee ontvangt een koppeling naar de proef via e-mail zonder verificatie), of <strong>E-mails over validatie en proefdrukken</strong> (Abonnees ontvangen een koppeling naar de proefdruk via e-mail en moeten op de koppeling klikken om toegang te krijgen tot een proefdruk. Deze optie heeft tot doel ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft).</p> <p>Opmerking: als de proefdrukken de automatische werkstroom hebben gekoppeld, worden alle abonnementen per e-mail met bevestiging verzonden naar de eigenaar van het bewijs, zodat ze kunnen beslissen in welk stadium de persoon moet worden toegevoegd.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klik op **[!UICONTROL Create Proof]**.

   Workfront begint met het genereren van een proefdruk van de geselecteerde documenten of websites. Afhankelijk van de bestandsgrootte en het type varieert de vertraging bij het uploaden van een document. Wees geduld, want het duurt langer om grotere bestanden te genereren. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

   Klik op **[!UICONTROL Go to proof]** om het proefdrukprogramma te starten.

   ![Screen_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   Het document wordt weergegeven in het proefdrukprogramma.

   Gebruikers die geen proefdrukken op hun account hebben ingeschakeld, kunnen het document nog steeds bekijken en opmerkingen naar de proefdruk maken.

## Een proef voor een URL genereren {#generate-a-proof-for-a-url}

U kunt voor het eerst een proef voor een URL produceren. U kunt ook een nieuwe versie van een URL-proefdruk genereren waarvoor eerder een proefdruk is gegenereerd.

>[!NOTE]
>
>U kunt alleen een interactieve proefdruk voor een URL maken als uw [!DNL Workfront] milieu is geïntegreerd met een [!DNL Workfront Proof] Premium-account. Als u geen proef zoals besproken in deze sectie kunt gebruiken, contacteer uw systeembeheerder.

Een proef voor een URL produceren:

1. Voer een van de volgende handelingen uit om een nieuwe proefdruk te maken en de [!UICONTROL New Proof] pagina:

   * Klik op groen **[!UICONTROL New proof]** in de linkerbovenhoek van een pagina.
   * In de **[!UICONTROL Dashboard]** in het gebied **[!UICONTROL Overview]** klikt u op de knop **[!UICONTROL New proof]** koppeling.

   * Verzenden via Dropzone (Enterprise-functie).

1. (Voorwaardelijk) In de **[!UICONTROL New proof]** pagina die wordt weergegeven, om een nieuwe versie van een bestaande proefdruk te maken:

   1. Selecteer de proefdruk URL waar u een nieuwe versie wilt toevoegen.
   1. Klik op de knop **[!UICONTROL New Version]** boven aan de pagina.

      ![Screenshot_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Geef op de pagina Nieuwe proefdrukversie die wordt weergegeven de URL op van de website die u wilt controleren in het dialoogvenster **[!UICONTROL Add Files]** gebied, dan drukken **[!UICONTROL Enter]**.

1. (Optioneel) Herhaal dit proces om meerdere websites aan een proefdruk toe te voegen.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Klik op de website in de documentlijst in het dialoogvenster **[!UICONTROL Add Files]** gebied.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Geef een **[!UICONTROL Proof name]** voor het bewijs.

   Standaard is de proefdruknaam dezelfde als de URL van de site.

1. Selecteren **[!UICONTROL Handle site contents]** opties:

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
      <td> <p>Hiermee maakt u een proefdruk waarmee revisoren door de site kunnen navigeren, HTML5-afbeeldingen, Flash-elementen enzovoort kunnen bekijken.</p> <p>Als u een interactief bewijs wilt maken, moet de website worden gehost met een beveiligd protocol (https). Bovendien kunnen websites die niet in een iframe kunnen worden ingesloten, niet worden gegenereerd als een interactieve proefdruk (beperkingen voor het insluiten van iframes worden bepaald door de website die u probeert in te sluiten).</p> <p>Nadat de eerste proefdruk is gemaakt, kan deze instelling niet worden gewijzigd wanneer u volgende versies maakt.</p> <p>Zie voor meer informatie over interactieve proefdrukken <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Een proefdruk maken voor interactieve inhoud</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schermresolutie</td> 
      <td> <p>(Deze optie is niet beschikbaar voor interactieve proefdrukken.) U kunt de resolutie aanpassen waarin uw inhoud wordt weergegeven, of u kunt meerdere resoluties selecteren.</p> <p>Hierdoor kunnen gebruikers de proefdruk controleren om te zien hoe inhoud op verschillende apparaten, zoals verschillende formaten telefoons, tablets en monitoren, wordt weergegeven.</p> <p>Als u meerdere resoluties selecteert, wordt voor elke resolutie die u selecteert een afzonderlijke proefdruk gemaakt.</p> <p>Wanneer gebruikers opmerkingen plaatsen over de proefdruk, wordt de huidige schermresolutie automatisch weergegeven in de opmerking om ervoor te zorgen dat andere gebruikers weten met welke resolutie de opmerking wordt geassocieerd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zoeken naar subpagina's</td> 
      <td>(Deze optie is niet beschikbaar voor interactieve proefdrukken.) Selecteer deze optie om door pagina's van de website te navigeren. U kunt de website tot 2 niveaus diep van de hoofdpagina uitbreiden. Plaats de muis boven een pagina om de URL van de pagina weer te geven. Selecteer alleen de pagina's waarvan u een proefdruk wilt maken. Elke pagina die u selecteert, wordt standaard gemaakt als een afzonderlijke proefdruk of schakelt u de optie <strong>Combineren tot één proefdruk</strong> gebruiken om alle geselecteerde pagina's te combineren tot één proefdruk.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optioneel) Configureer eventuele geavanceerde opties voor proefdrukken, zoals het delen van de proefdruk, het toevoegen van een geautomatiseerde workflow of het instellen van toegangs- en abonnementsinstellingen. Raadpleeg de volgende artikelen voor meer informatie over deze opties:

   * [Een proefdruk delen binnen [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Stel een proefdruk in met een geautomatiseerde workflow in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Toegang- en abonnementsinstellingen configureren voor een proefdruk](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klik op **[!UICONTROL Done]**.

   Als u een nieuwe versie toevoegt aan een bestaande URL-proefdruk, blijven de opties die op de oorspronkelijke proefdruk of vorige versie zijn geconfigureerd, behouden in deze versie. Als u een nieuwe versie toevoegt aan een bestaande URL-proefdruk, blijven de opties die op de oorspronkelijke proefdruk of op de vorige versie zijn geconfigureerd, behouden in deze versie.

1. Klik op **[!UICONTROL Create Proof]**.

## Een proefdruk maken voor interactieve inhoud {#generate-a-proof-for-interactive-content}

Voor het gebruik van deze functie is een Pro Workfront-abonnement of hoger vereist. Zie voor meer informatie over de verschillende beschikbare plannen [Workfront-plannen](https://www.workfront.com/plans).

Zie voor meer informatie over interactieve inhoud [Overzicht van proefdrukken van interactieve inhoud](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Interactieve inhoud toevoegen als een URL](#add-interactive-content-as-a-url)
* [Interactieve inhoud toevoegen als ZIP-bestand](#add-interactive-content-as-a-zip-file)

### Interactieve inhoud toevoegen als een URL {#add-interactive-content-as-a-url}

Zie voor informatie over het toevoegen van een interactieve URL-proefdruk  [Een proef voor een URL genereren](#generate-a-proof-for-a-url).

### Interactieve inhoud toevoegen als ZIP-bestand {#add-interactive-content-as-a-zip-file}

1. Bereid uw inhoud voor door een ZIP-gebundeld bestand te maken.

   Voor informatie over .zip gebundelde dossierspecificaties, zie [Informatie over het voorbereiden van interactieve inhoud in een ZIP-bestand voor proefdrukken](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) in het artikel [Overzicht van proefdrukken van interactieve inhoud](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Voer een van de volgende handelingen uit om een nieuwe proefdruk te maken en de [!UICONTROL New Proof] pagina:

   * Klik op groen **[!UICONTROL New proof]** in de linkerbovenhoek van een pagina.
   * In de **[!UICONTROL Dashboard]** in het gebied **[!UICONTROL Overview]** klikt u op de knop **[!UICONTROL New proof]** koppeling.

   * Verzenden via Dropzone (Enterprise-functie).

1. In de **[!UICONTROL New proof]** pagina die wordt weergegeven, sleept u de interactieve ZIP-bundel naar de **[!UICONTROL Add files]** gebied.

1. (Optioneel) Configureer eventuele geavanceerde opties voor proefdrukken, zoals het delen van de proefdruk, het toevoegen van een geautomatiseerde workflow of het instellen van toegangs- en abonnementsinstellingen. Raadpleeg de volgende artikelen voor meer informatie over deze opties:

   * [Een proefdruk delen binnen [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * in het artikel
   * [Toegang- en abonnementsinstellingen configureren voor een proefdruk](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Klik op **[!UICONTROL Create Proof]**.

   Workfront begint een bewijs van de ZIP-bundel te genereren. Afhankelijk van de bundelgrootte varieert de vertragingstijd bij het uploaden van een document. Het genereren van grotere bestanden duurt langer. U kunt van de pagina weg navigeren en Workfront blijft uw bestand genereren. De maximale grootte voor het uploaden van bestanden is 4 GB.

   Nadat de proefdruk is gegenereerd, kunt u op de knop **[!UICONTROL Go to proof]** die de proefdruk lijkt te openen.
