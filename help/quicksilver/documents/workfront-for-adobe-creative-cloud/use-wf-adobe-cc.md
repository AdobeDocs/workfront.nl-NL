---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-adobe-creative-cloud
title: De extensie Workfront voor Illustrator en InDesign gebruiken
description: Met de extensie Workfront kunt u digitale inhoud die u opslaat en maakt in Adobe Illustrator en Adobe InDesign exporteren naar Workfront. Hierdoor wordt het reviseren en goedkeuren van documenten versneld.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: 40945eac-e8de-42af-b6ba-f3082c208e02
source-git-commit: 147a5b5d508e1ea01d18d981f9157439a643cf55
workflow-type: tm+mt
source-wordcount: '3056'
ht-degree: 0%

---

# De extensie Workfront voor Illustrator en InDesign gebruiken

>[!IMPORTANT]
>
>We vervangen de extensie Workfront voor Illustrator en InDesign door [bijgewerkte Creative Cloud-plug-ins](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-toc.md). Vanaf eind 2022 wordt deze extensie niet meer ondersteund en is deze ongewijzigd beschikbaar.


Met de extensie Workfront kunt u digitale inhoud die u opslaat en maakt in Adobe Illustrator en Adobe InDesign exporteren naar Workfront. Hierdoor wordt het reviseren en goedkeuren van documenten versneld.

De extensie Workfront wordt ondersteund voor Adobe Creative Cloud 2017 en hoger in de volgende toepassingen:

* InDesign
* Illustrator
* Photoshop

   >[!NOTE]
   >
   >We raden u aan de nieuwe [Adobe Workfront voor Photoshop](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-cc-install-ps.md) insteekmodule.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Pro of hoger</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>U moet een Adobe Creative Cloud-licentie hebben naast een Workfront-licentie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Bewerk de toegang tot het object waarmee u wilt communiceren.</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Aanmelden bij Workfront Extension vanuit Illustrator of InDesign {#log-in-to-workfront-extension-from-illustrator-or-indesign}

Wanneer u zich bij Workfront aanmeldt vanuit een van de ondersteunde Adobe-toepassingen, wordt u aangemeld bij alle ondersteunde Adobe-toepassingen.

1. Ga naar de toepassing van de Adobe waar u de uitbreiding van Workfront wilt gebruiken.

   Voor een lijst met ondersteunde indelingen voor elke ondersteunde toepassing raadpleegt u [Ondersteunde geëxporteerde bestandsindelingen](#supported-exported-file-formats) in dit artikel.

1. Klikken **Venster** > **Extensies** > Workfront.

1. (Optioneel) Sleep het Workfront-deelvenster naar de positie waar u het wilt weergeven in de Adobe-toepassing.
1. Volg de aanwijzingen om u aan te melden bij Workfront.

   >[!NOTE]
   >
   >* Workfront maakt verbinding met Adobe Creative Cloud met behulp van OAuth 2.0, een veilige standaard die door de meeste webgebaseerde integraties wordt gebruikt voor de verificatie en autorisatie van gebruikers.
   >* Wanneer u wordt gevraagd om het dialoogvenster [domein of host] van uw Workfront-account typt u deze notatie: *yourCompany&#39;sDomain.my.workfront.com*. Het domein van uw bedrijf is gewoonlijk de naam van uw bedrijf.


   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

## Een bestand uploaden naar een Workfront-project, -taak of -uitgave {#upload-a-file-to-a-workfront-project-task-or-issue}

U kunt een bestand uploaden vanaf uw computerbestandssysteem of een bestand dat momenteel in een Adobe Creative Cloud-toepassing is geopend, exporteren naar een Workfront-project, -taak of -uitgave. 

Houd rekening met het volgende wanneer u een bestand uploadt of exporteert uit Adobe Creative Cloud:

* Met het toegangsniveau kunt u documenten alleen uploaden naar Workfront. Zie voor meer informatie [Toegang tot documenten verlenen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).
* U moet over machtigingen beschikken om documenten te uploaden naar het gewenste item. Zie voor meer informatie [Overzicht van het delen van machtigingen voor objecten](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Het bestand wordt geüpload naar het gebied Documenten voor het Workfront-object dat u selecteert.
* U kunt een document niet exporteren naar het gebied Documenten in het hoofdmenu ![](assets/main-menu-icon.png) uit een Adobe Creative Cloud-toepassing.

In dit gedeelte wordt het volgende uitgelegd:

* [Een bestand uploaden](#upload-a-file)
* [Een bestand exporteren dat momenteel is geopend in Illustrator of InDesign](#export-a-file-currently-open-in-illustrator-or-indesign)
* [Een nieuwe versie van een bestand uploaden vanuit Illustrator of InDesign](#upload-a-new-version-of-a-file-from-illustrator-or-indesign)

### Een bestand uploaden {#upload-a-file}

U kunt uw bestanden uploaden naar een project, taak of uitgave zonder uw Adobe Creative Cloud-toepassing te verlaten.

1. Als de Workfront-extensie niet wordt weergegeven wanneer u de Adobe Creative Cloud-toepassing opent, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Klik op de naam van het project, de taak of de uitgave waarnaar u het bestand wilt uploaden.

   U kunt hier naar zoeken door de naam te typen in het dialoogvenster **Zoeken** en selecteren **Project**, **Taak**, of **Probleem** in het keuzemenu rechts van de **Zoeken** doos. Als de naam van het werkitem niet in de lijst wordt weergegeven, drukt u op **Enter** om te zoeken in alle Workfront-objecten die je kunt bekijken.

1. Klikken **Selecteren** in de rechterbenedenhoek van de extensie Workfront.
1. In de **Klik om opmaak te selecteren** klikt u op de indeling waarin u het bestand wilt opslaan in Workfront.

   Voor een lijst met ondersteunde indelingen voor elke ondersteunde toepassing raadpleegt u [Ondersteunde geëxporteerde bestandsindelingen](#supported-exported-file-formats) in dit artikel.

1. (Voorwaardelijk) Als het werkitem waarnaar u het bestand wilt uploaden documentmappen bevat, selecteert u een documentmap in het dialoogvenster **Klik om een documentmap te selecteren** veld, klik vervolgens op **Selecteren**.

1. Klikken **Een lokaal bestand uploaden**.
1. In de **Bestand openen** het bestand in uw bestandssysteem te zoeken en vervolgens op **Openen**.

1. (Optioneel) Typ een nieuwe naam voor het bestand. 

   ![](assets/rename-file-uploading.png)

1. Klikken **Uploaden**.

   In Workfront wordt het document nu vermeld in het gebied Documenten voor het project, de taak of de uitgave die u hebt opgegeven.  

1. (Optioneel) Klik op de naam van het document om de pagina Documentdetails te openen in Workfront.

   Workfront wordt geopend in een nieuw browsertabblad.

### Een bestand exporteren dat momenteel is geopend in Illustrator of InDesign {#export-a-file-currently-open-in-illustrator-or-indesign}

1. Open in een ondersteunde Adobe Creative Cloud-toepassing een bestand dat u naar Workfront wilt exporteren. 
1. Als de Workfront-extensie niet wordt weergegeven, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Klik op de naam van het project, de taak of de uitgave waarnaar u het bestand wilt exporteren.

   U kunt hier naar zoeken door de naam te typen in het dialoogvenster **Zoeken** en selecteren **Project**, **Taak**, of **Probleem** in het keuzemenu rechts van de **Zoeken** doos. Als de naam van het werkitem niet in de lijst wordt weergegeven, drukt u op **Enter** om te zoeken in alle Workfront-objecten die je kunt bekijken.

1. In de **Klik om opmaak te selecteren** klikt u op de indeling waarin u het bestand wilt opslaan in Workfront.

   Voor een lijst met ondersteunde indelingen voor elke ondersteunde toepassing raadpleegt u [Ondersteunde geëxporteerde bestandsindelingen](#supported-exported-file-formats) in dit artikel.

1. (Voorwaardelijk) Als het werkitem waarnaar u het bestand wilt uploaden documentmappen bevat, selecteert u een documentmap in het dialoogvenster **Klik om een documentmap te selecteren** veld, klik vervolgens op **Selecteren**.
1. (Optioneel) Als u de naam van het document wilt wijzigen, klikt u op de documentnaam en typt u een nieuwe naam.

   ![](assets/rename-doc-exporting.png)

1. Klikken **Exporteren**. 

   Er wordt een bericht weergegeven om te bevestigen dat het document is geëxporteerd naar Workfront.

   In Workfront wordt het document weergegeven in het gebied Documenten van het object dat u in Workfront hebt opgegeven.

1. (Optioneel) Klik op de naam van het document om het in Workfront te openen.

   ![adobe_document_with_name_highlight.PNG](assets/adobe-document-with-name-highlight-350x251.png)

   Workfront wordt geopend in een nieuw browsertabblad.

### Een nieuwe versie van een bestand uploaden vanuit Illustrator of InDesign {#upload-a-new-version-of-a-file-from-illustrator-or-indesign}

1. Als u een bestand waaraan u werkt in een ondersteunde Adobe-toepassing wilt exporteren als een nieuwe versie van een bestand in Workfront, opent u het bestand in de Adobe-toepassing. 
1. Als de Workfront-extensie niet wordt weergegeven, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Klik op de naam van het project, de taak of de uitgave waar het bestaande document wordt weergegeven.

   U kunt hier naar zoeken door de naam te typen in het dialoogvenster **Zoeken** en selecteren **Project**, **Taak**, of **Probleem** in het keuzemenu rechts van de **Zoeken** doos. Als de naam van het werkitem niet in de lijst wordt weergegeven, drukt u op **Enter** om te zoeken in alle Workfront-objecten die je kunt bekijken.

   Alle documenten die naar projecten, taken of uitgaven worden geüpload, worden in een lijst weergegeven, ongeacht of ze vanuit de Adobe-toepassing zijn geüpload.

1.  
1. In de **Klik om opmaak te selecteren** klikt u op de indeling waarin u het bestand wilt opslaan in Workfront.

   Dit is vereist als u een bestand exporteert dat is geopend in de Adobe-toepassing. Voor een lijst met ondersteunde indelingen voor elke ondersteunde toepassing raadpleegt u [Ondersteunde geëxporteerde bestandsindelingen](#supported-exported-file-formats) in dit artikel.

1. Als u een bestand exporteert dat u in de Adobe-toepassing hebt geopend, als een nieuwe versie van het Workfront-document dat u hebt geselecteerd, klikt u op **Exporteren**.

   of

   Als u een bestand van uw computerbestandssysteem wilt uploaden als een nieuwe versie van het Workfront-document dat u hebt geselecteerd, klikt u op **Een lokaal bestand uploaden**, zoekt u het bestand in het vak dat wordt weergegeven, klikt u op **Openen** en klik vervolgens op **Uploaden**.

1. (Optioneel) Klik op de naam van het document om de nieuwe versie weer te geven in Workfront. 

   >[!NOTE]
   >
   >De naam van het document in Workfront wordt standaard ingevuld en kan niet worden bewerkt. De naam van het bestand dat u uploadt of exporteert, wordt ook niet gewijzigd als een nieuwe versie.
   >
   >
   >![](assets/doc-name-cant-be-changed.png)

## Opmerkingen maken over een Workfront-document van Illustrator of InDesign {#comment-on-a-workfront-document-from-illustrator-or-indesign}

U kunt opmerkingen rechtstreeks toevoegen aan een Workfront-document in een Adobe-toepassing. In Workfront worden uw opmerkingen weergegeven in het gedeelte Updates van het document en in het gedeelte Updates van het Workfront-item waar het document is opgeslagen. 

1. Open een van de ondersteunde Adobe-toepassingen.
1. Als de Workfront-extensie niet wordt weergegeven, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Klik op het project, de taak of het probleem waarbij het bestaande document wordt weergegeven.

   U kunt hier naar zoeken door de naam te typen in het dialoogvenster **Zoeken** en selecteren **Project**, **Taak**, of **Probleem** in het keuzemenu rechts van de **Zoeken** doos. Als de naam van het werkitem niet in de lijst wordt weergegeven, drukt u op **Enter** om te zoeken in alle Workfront-objecten die je kunt bekijken.

1. Klik op de naam van het bestaande document en klik vervolgens op **Selecteren** in de rechterbenedenhoek van de extensie Workfront.
1. Klik op de knop **Opmerking** typt u de update in het vak dat wordt weergegeven.

1. (Optioneel) Als u andere Workfront-gebruikers of -teams wilt opnemen in de opmerking, typt u de naam van een gebruiker of een team in het deelvenster **Personen of teams op de hoogte stellen** klikt u op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.
1. (Optioneel) Selecteer **Goedkeuringsaanvraag indienen**.
1. Klikken **Bijwerken**.

   Er wordt een update gepost op het tabblad Updates van het document. Workfront-gebruikers die u in de opmerking opneemt, ontvangen een melding in de app en ontvangen, afhankelijk van de configuratie van Workfront, mogelijk ook een e-mailmelding.

   Ga voor meer informatie over berichten in Workfront naar [Meldingen in apps weergeven en beheren](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). 

   Voor meer informatie over het ontvangen van e-mailberichten raadpleegt u [Adobe Workfront-berichten](../../workfront-basics/using-notifications/wf-notifications.md).

## Illustrator of InDesign om goedkeuring van een document vragen

U kunt een Workfront-documentgoedkeuring rechtstreeks aanvragen bij een Adobe-toepassing.

U kunt de volgende entiteiten om goedkeuring van een document verzoeken:

* Een Workfront-gebruiker
* Een externe gebruiker zonder een Workfront-account

U kunt op de volgende manieren goedkeuring aanvragen voor een document van een Adobe-toepassing:

* Door een fiatteur aan het document te koppelen.
* Door opmerkingen toe te voegen aan een document, meldt u de persoon wanneer u een opmerking maakt. en ze als fiatteur aan het document koppelen.

   Voor informatie over het aanvragen van een goedkeuring bij het plaatsen van opmerkingen over een document raadpleegt u [Opmerkingen maken over een Workfront-document van Illustrator of InDesign](#comment-on-a-workfront-document-from-illustrator-or-indesign) in dit artikel.

Om een goedkeuring op een document van een Adobe- aanvraag te verzoeken:

1. Open een van de ondersteunde Adobe-toepassingen.
1. Als de Workfront-extensie niet wordt weergegeven, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Klik op het project, de taak of het probleem waarbij het bestaande document wordt weergegeven en klik vervolgens op de naam van het bestaande document.

   U kunt hier naar zoeken door de naam te typen in het dialoogvenster **Zoeken** en selecteren **Project**, **Taak**, of **Probleem** in het keuzemenu rechts van de **Zoeken** doos. Als de naam van het werkitem niet in de lijst wordt weergegeven, drukt u op **Enter** om te zoeken in alle Workfront-objecten die je kunt bekijken.

1. Klik op de naam van het bestaande document en klik vervolgens op **Selecteren** in de rechterbenedenhoek van de extensie Workfront.
1. Klik op de knop **Goedkeuring** tab.
1. Om een fiatteur toe te voegen, in **Een naamvak typen** Voer een van de volgende handelingen uit:

   * Typ de naam van een fiatteur en selecteer deze vervolgens wanneer deze in de lijst wordt weergegeven.

      ![](assets/adobe-cc-adding-a-doc-approver-350x189.png)

   * Typ het e-mailadres van een externe gebruiker.

1. Klikken **Goedkeuring aanvragen**.

   Workfront-gebruikers die u in de opmerking of als fiatteur toevoegt, ontvangen een melding in de app en ontvangen, afhankelijk van de configuratie van Workfront, mogelijk ook een e-mailbericht.\
   Externe gebruikers ontvangen een e-mailbericht van de locatie waar zij een beslissing over de goedkeuring kunnen nemen.

   Voor informatie over berichten in Workfront raadpleegt u [Meldingen in apps weergeven en beheren](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md). Voor informatie over het ontvangen van e-mailberichten raadpleegt u [Adobe Workfront-berichten](../../workfront-basics/using-notifications/wf-notifications.md).

## Een proefdruk van Illustrator of InDesign genereren {#generate-a-proof-from-illustrator-or-indesign}

Als uw organisatie automatische werkstroomsjablonen gebruikt, kunt u een proefdruk genereren voor een document dat u maakt in een Adobe-toepassing zonder de toepassing te verlaten. Voor informatie over het maken van proefdrukken raadpleegt u [Proefdrukken maken](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-proofs--in-wf.md). Voor informatie over Geautomatiseerde malplaatjes van het Werkschema, zie [Geautomatiseerde werkstroomsjablonen](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md#automate) in [Geautomatiseerd workflowoverzicht](../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

1. Open een van de ondersteunde Adobe-toepassingen.
1. Als de Workfront-extensie niet wordt weergegeven, klikt u op **Venster** > **Extensies** > Workfront.

   Een lijst van het werkpunten die aan u worden toegewezen toont als het project een huidige status is. Meld u aan bij Workfront als een lijst niet wordt weergegeven.

   Persoonlijke taken worden onder **Geen project**.

1. Als het document al naar Workfront is geüpload, selecteert u het project, de taak of geeft u een uitgave in de Workfront-extensie waar het document wordt weergegeven. Klik vervolgens op de naam van het document.

   of

   Een Adobe-document uploaden naar een Workfront-object, zoals wordt beschreven in de sectie [Een bestand uploaden naar een Workfront-project, -taak of -uitgave](#upload-a-file-to-a-workfront-project-task-or-issue) in dit artikel, klikt u op de naam van het document.

1. In de **Klik om opmaak te selecteren** klikt u op de indeling waarin u het bestand wilt opslaan in Workfront.

   Sommige indelingen zijn niet beschikbaar nadat u de proefdrukfunctionaliteit hebt ingeschakeld in de volgende stap. Zie voor meer informatie [Ondersteunde geëxporteerde bestandsindelingen](#supported-exported-file-formats) in dit artikel.

1. Klikken **Uploaden als een nieuwe proefdruk** om het mogelijk te maken.
1. Selecteer **Workflowsjabloon** u wilt dat personen het document reviseren.

   Uw Workfront-beheerder stelt de automatische workflowsjablonen in, zoals beschreven in . Zie de beheerder als u vragen hebt.

   1. Minstens één toevoegen **Nieuwe ontvanger** in elk stadium in het malplaatje van het Werkschema.

      U kunt beginnen een naam te typen en het selecteren wanneer u het in de drop-down lijst ziet die verschijnt.

   1. Geef de **Proefdrukrol** en frequentie van **E-mailwaarschuwingen** voor elke ontvanger die u toevoegt.

   1. (Optioneel) In het dialoogvenster **E-mailmelding** selecteert u of u een e-mailbericht met een optioneel aangepast bericht over de proefdruk wilt verzenden aan alle proefontvangers die u hebt toegevoegd.

1. Klikken **Proef maken**.

   U kunt de voortgang van het maken van proefdrukken bekijken. Er wordt een waarschuwing weergegeven wanneer het genereren is voltooid. U kunt de taak openen waar u de proefdruk hebt gemaakt en deze wordt daar weergegeven.

## Een nieuwe versie van een proefdruk uploaden zonder Illustrator of InDesign te verlaten

1. Klik op een bestaand document met een proefdruk en klik vervolgens op **Selecteren** in de rechterbenedenhoek.
1. Klikken **Uploaden als een nieuwe proefdrukversie** om het mogelijk te maken.
1. (Optioneel) Selecteer de optie **Workflowsjabloon** u wilt dat mensen de nieuwe versie bekijken.

   Als u geen andere sjabloon selecteert, blijft de sjabloon die voor de eerdere versie is geselecteerd, van kracht. Als u de sjabloon voor de eerdere versie hebt gewijzigd, zijn de wijzigingen ook van kracht voor de nieuwe versie.

   Uw Workfront-beheerder stelt de automatische workflowsjablonen in, zoals beschreven in . Zie de beheerder als u vragen hebt.

   1. Minstens één toevoegen **Nieuwe ontvanger** in elk stadium in het malplaatje van het Werkschema.

      U kunt beginnen een naam te typen en het selecteren wanneer u het in de drop-down lijst ziet die verschijnt.

   1. Geef de **Proefdrukrol** en frequentie van **E-mailwaarschuwingen** voor elke ontvanger die u toevoegt.
   1. (Optioneel) In het dialoogvenster **E-mailmelding** selecteert u of u een e-mailbericht met een optioneel aangepast bericht over de proefdruk wilt verzenden aan alle proefontvangers die u hebt toegevoegd.

1. Klikken **Nieuwe proefdrukversie maken**.

   U kunt de voortgang van het maken van proefdrukken bekijken. Er wordt een waarschuwing weergegeven wanneer het genereren is voltooid. U kunt de taak openen waar u de proefdruk hebt gemaakt en deze wordt daar weergegeven.

## Afmelden bij Workfront-extensie

1. Klik in de toepassing Adobe op **Venster** > **Extensies** > Workfront.

1. Klik op de knop **Meer** menu ![](assets/more-menu.png) in de rechterbovenhoek van het deelvenster.

1. (Optioneel) Klik op **Feedback** om een korte enquête te openen en Workfront je feedback over Workfront for Adobe Creative Cloud te sturen. 
1. Klikken **Afmelden**.\
   Het aanmeldingsscherm wordt weergegeven. Voor informatie over het aanmelden raadpleegt u [Aanmelden bij Workfront Extension vanuit Illustrator of InDesign](#log-in-to-workfront-extension-from-illustrator-or-indesign) in dit artikel.

## Ondersteunde geëxporteerde bestandsindelingen {#supported-exported-file-formats}

* [Ondersteunde geëxporteerde bestandsindelingen voor Adobe InDesign](#supported-exported-file-formats-for-adobe-indesign)
* [Ondersteunde geëxporteerde bestandsindelingen voor Adobe Illustrator](#supported-exported-file-formats-for-adobe-illustrator)

### Ondersteunde geëxporteerde bestandsindelingen voor Adobe InDesign  {#supported-exported-file-formats-for-adobe-indesign}

Workfront ondersteunt de volgende bestandsindelingen voor het exporteren van een bestand van InDesign naar Workfront:

* EPS - Encapsulated PostScript
* ePub - Vaste indeling van elektronische publicatie
* ePub - Opnieuw te publiceren elektronische publicatie &#42;
* HTML - HyperText Markup Language
* IDML - InDesign Markup Language &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PDF - Adobe Portable-documentbestand
* PNG - Portable Network Graphics
* SWF - Flash Player &#42;
* XML - Extensible Markup Language &#42;

&#42; Deze bestandsindeling is niet beschikbaar als **Een nieuwe proefdruk uploaden** is ingeschakeld (zie voor informatie over deze optie [Een proefdruk van Illustrator of InDesign genereren](#generate-a-proof-from-illustrator-or-indesign) in dit artikel). Als deze bestandsindeling al is geselecteerd voordat u deze inschakelt **Een nieuwe proefdruk uploaden** wordt de bestandsindeling gewijzigd in PDF. U kunt een andere indeling selecteren in de lijst.

### Ondersteunde geëxporteerde bestandsindelingen voor Adobe Illustrator  {#supported-exported-file-formats-for-adobe-illustrator}

Workfront ondersteunt de volgende bestandsindelingen voor het exporteren van een bestand van Illustrator naar Workfront:

* DWG - AutoCAD-tekening, AutoCAD-uitwisselingsbestand &#42;
* JPG, JPEG - Joint Photographic Experts Group
* PNG - Portable Network Graphics
* PSD - Photoshop-document
* SWF - Flash Player &#42;
* TIFF - Tagged Image File Format

&#42; Deze bestandsindeling is niet beschikbaar als **Een nieuwe proefdruk uploaden** is ingeschakeld (zie voor informatie over deze optie [Een proefdruk van Illustrator of InDesign genereren](#generate-a-proof-from-illustrator-or-indesign) in dit artikel). Als deze bestandsindeling al is geselecteerd voordat u deze inschakelt **Een nieuwe proefdruk uploaden** wijzigt het systeem de bestandsindeling in PNG. U kunt een andere indeling selecteren in de lijst.
