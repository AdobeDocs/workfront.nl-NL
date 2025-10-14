---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Veelgestelde vragen - proefdrukken en bestanden maken en delen
description: Een proefdruk is een statisch, audio- of videobestand dat in de conceptviewer beschikbaar is voor revisie. Revisoren die aan een bewijs zijn toegevoegd, beschikken over een set gereedschappen om opmerkingen en beslissingen over de proefdruk te maken.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1342'
ht-degree: 0%

---

# Veelgestelde vragen - proefdrukken en bestanden maken en delen

>[!IMPORTANT]
>
>Dit artikel verwijst naar functionaliteit in het zelfstandige product [!DNL Workfront Proof] . Voor informatie bij het proef binnen [!DNL Adobe Workfront], zie [&#x200B; het Bewijzen &#x200B;](../../../review-and-approve-work/proofing/proofing.md).

## Wat is een bewijs?

### Antwoord

Een proefdruk is een statisch, audio- of videobestand dat in de conceptviewer beschikbaar is voor revisie. Revisoren die aan een bewijs zijn toegevoegd, beschikken over een set gereedschappen om opmerkingen en beslissingen over de proefdruk te maken.

## Welke bestandstypen worden ondersteund?

### Antwoord

U kunt proefdrukken maken op basis van statische bestanden, audiobestanden en videobestanden. U kunt geen bestanden uploaden die groter zijn dan 4 GB. [!DNL Workfront] steunt meer dan 150 dossiertypes (zie [&#x200B; Ondersteunde het proef dossiertypes en het overzicht van groottegrenzen &#x200B;](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) voor een volledige lijst).

## Wat is het verschil tussen een bewijs en een dossier?

### Antwoord

Wanneer u een bestand uploadt naar [!DNL Workfront Proof] , slaat het systeem het bestand op in uw [!DNL Workfront Proof] -account. Wanneer u het deelt, verzendt [!DNL Workfront Proof] een e-mail aan uw ontvangers een verbinding die zij kunnen klikken om het dossier te downloaden. U kunt elk gewenst bestandstype delen.

Wanneer u een proefdruk maakt op basis van een bestand dat u hebt geüpload naar [!DNL Workfront Proof] , kunt u het bestand ter controle beschikbaar stellen in de conceptviewer. Revisoren ontvangen een e-mail met een koppeling naar de proefdruk. Wanneer ze de proefdruk openen, zien ze de proefdruk en kunnen ze opmerkingen toevoegen en besluiten nemen. U kunt proeven tot stand brengen gebruikend dossiers van de lijst van gesteunde dossiertypes. U kunt ook proefdrukken maken met behulp van URL&#39;s voor websites en andere webinhoud.

Voor een volledige lijst van gesteunde dossiertypes, zie [&#x200B; Ondersteunde het proef dossiertypes en groottegrenzen overzicht &#x200B;](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Hoe maak ik een bewijs?

### Antwoord

U kunt proefdrukken maken van statische bestanden, audiobestanden, videobestanden en URL&#39;s (zie ).

Om een proef in de rekening tot stand te brengen, moet u een gebruiker met het juiste toestemmingsprofiel zijn (zie [[!UICONTROL Proof Permissions Profiles] in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Als u meerdere bestanden tegelijk uploadt, maakt u meerdere proefdrukken die u via één e-mail naar dezelfde groep controleurs kunt verzenden. Als uw organisatie een [!UICONTROL Enterprise] of [!UICONTROL Unlimited] rekening heeft, kunt u dossiers in één enkele proef combineren (zie [&#x200B; een multi-paginaproef &#x200B;](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) creëren).

## Wat zijn proefrollen en e-mailalarm?

### Antwoord

Proefrollen bepalen welke acties een revisor moet uitvoeren als bewijs. Er zijn verschillende rolopties die u kunt gebruiken voor revisoren wanneer u een proefdruk maakt, afhankelijk van de vraag of u wilt dat deze revisoren opmerkingen kunnen maken, beslissingen kunnen nemen, enzovoort. Voor meer informatie, zie [&#x200B; Beheer de Rollen van het Bewijs binnen  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Met e-mailwaarschuwingen worden revisoren bijgewerkt over de voortgang van een bewijs (ze zijn anders dan nieuwe proefdrukken en recente proefdrukmeldingen). U kunt verschillende opties selecteren voor verschillende revisoren, afhankelijk van de rol van elke revisor op de proefdruk. Voor meer informatie, zie [&#x200B; een geavanceerde proef met [!UICONTROL Automated workflow]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md) creëren.

## Kan ik een proefdruk maken op basis van meerdere bestanden?

### Antwoord

Het combineren van meerdere bestanden tot één proefdruk is een functie die beschikbaar is in [!UICONTROL Enterprise] - en [!UICONTROL Unlimited] -editieplannen. Deze optie is alleen mogelijk voor statische bestanden, niet voor videobestanden. Voor meer informatie, zie [&#x200B; tot een multi-paginaproef &#x200B;](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) leiden.

## Kan ik proefdrukken maken van URL&#39;s?

### Antwoord

Ja, u kunt proefdrukken maken van websites en andere webinhoud. Wanneer u een URL toevoegt om een proefdruk te maken, kunt u opgeven of u een statische proefdruk of een interactieve proefdruk wilt:

* In een interactieve proefdruk kunnen revisoren op dezelfde manier navigeren en communiceren als gewoonlijk met de website of andere webinhoud, zoals advertenties met streaming video of audio, [!DNL Flash] -elementen in een advertentie, HTML-animaties en interactieve banners. Voor meer informatie, zie [&#x200B; een proef voor interactieve inhoud in een dossier van het PIT &#x200B;](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md) creëren.
* Voor een statische proefdruk maakt [!DNL Workfront] een set schermafbeeldingen van de pagina&#39;s en subpagina&#39;s die u opgeeft. Hyperlinks bevinden zich in de proefdruk, zodat u kunt testen of ze naar de juiste bestemming leiden. Voor meer informatie, zie [&#x200B; een statisch bewijs voor een website of andere Webinhoud &#x200B;](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md) creëren.

U kunt meerdere URL&#39;s tegelijk toevoegen als u deze scheidt met een spatie. Combinatie is alleen beschikbaar in [!UICONTROL Enterprise] - en [!UICONTROL Unlimited] -editieplannen.

## Kunnen mensen die geen aanmelding hebben proefdrukken maken in mijn account?

### Antwoord

U hebt aanmeldingsgegevens nodig om proefdrukken rechtstreeks in een [!DNL Workfront Proof] -account te maken.

## Wat betekent het delen van een bewijs?

### Antwoord

Door een proefdruk te delen, hebben revisoren toegang tot de proefdrukproef, zodat ze opmerkingen en markeringen kunnen toevoegen en er beslissingen over kunnen nemen. Gastrevisoren hebben toegang tot proefdrukken van het e-mailbericht dat ze ontvangen. Revisoren met hun eigen [!DNL Workfront Proof] -account hebben toegang tot proefdrukken op de [!UICONTROL Dashboard] .

## Hoe kan ik een bewijs delen?

### Antwoord

Wanneer u een proefdruk maakt, kunt u revisoren toevoegen in de sectie [!UICONTROL Workflow] van de pagina [!UICONTROL New Proof] . Als de proefdruk gereed is, stuurt [!DNL Workfront Proof] een e-mail naar de controleurs met een koppeling naar de proefdruk.

Als u voldoende rechten op een proef hebt, kunt u de het proef kijker, uw [!UICONTROL Dashboard], of om het even welke lijstmeningen gebruiken om recensenten aan een bestaand bewijs toe te voegen (zie [&#x200B; Deel een Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views]  Pagina in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

Het toevoegen van revisoren is de meest gebruikelijke manier om proefdrukken te delen. Zie voor meer informatie over andere beschikbare opties:

* [&#x200B; de proefdruk van het aandeel verbindingen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [&#x200B; Deel Openbare URL in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [&#x200B; Abonneren aan een Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Een Mini-proefdruk maken in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Moet u een gebruiker zijn om een proefdruk te controleren?

### Antwoord

Nee. Gastrevisoren (personen zonder [!DNL Workfront Proof] aanmeldingsgegevens) hebben toegang tot een proefdruk via het e-mailbericht dat ze ontvangen. U kunt een proefdruk delen met zoveel gasten als u wilt.

U kunt het delen van proefdrukken beperken tot personen met [!DNL Workfront Proof] aanmeldingsgegevens. Hiermee voegt u nog een beveiligingslaag toe aan uw proefdrukken. Voor uitgebreide beveiliging kunnen systeembeheerders van organisaties met [!UICONTROL Enterprise] - en [!UICONTROL Unlimited] -plannen deze vereiste configureren voor alle proefdrukken die in de organisatie zijn gemaakt.

Voor meer informatie over het vereisen van login, zie [&#x200B; veiligheid van het Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Als uw organisatie revisoren verplicht heeft proefdrukken elektronisch te ondertekenen, waarvoor u zich moet aanmelden bij [!DNL Workfront Proof] , kunnen gebruikers alleen proefdrukken delen met geregistreerde gebruikers. Dit is beschikbaar in [!UICONTROL Enterprise] - en [!UICONTROL Unlimited] -editieplannen. Voor meer informatie, zie [&#x200B; Begrijpend elektronische handtekeningen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Kan ik een deadline stellen voor mijn revisoren?

### Antwoord

U kunt een deadline instellen voor een nieuwe proefdruk of een nieuwe proefdrukversie wanneer u de proefdruk maakt. Dit doet u in de sectie [!UICONTROL Workflow] van de pagina [!UICONTROL New Proof] . Als u [!UICONTROL Automated Workflow] gebruikt, kunt u een andere deadline instellen voor elke fase van de revisie.

U kunt ook een deadline voor een bestaande proefdruk instellen of bijwerken met de pagina [!UICONTROL Proof Details] . Voor meer informatie, zie [&#x200B; Beheren de Details van het Bewijs in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Hoe kan ik een nieuwe versie van mijn bewijs maken?

### Antwoord

Revisoren vragen vaak om wijzigingen in hun opmerkingen op een proefdruk en willen een nieuwe versie van de proefdruk. U kunt nieuwe versies van een proefdruk maken. [!DNL Workfront Proof] onthoudt de proefdrukinstellingen van de vorige versie. U kunt deze instellingen nog steeds bewerken als u revisoren voor de proefdruk wilt toevoegen of verwijderen.

U moet elke versie delen met de specifieke controleurs die deze moeten bekijken. Als u bijvoorbeeld alleen versie 3 deelt met een revisor, kan die persoon geen versies 1 en 2 zien. De toezichthouders en de Beheerders in uw rekening zien alle projecten in de rekening, zodat kunnen zij alle versies van de proef zien en uitgeven.

Zie voor meer informatie.

## Kan ik bestanden delen met [!DNL Workfront Proof]?

### Antwoord

Ja. Als u iets met andere mensen wilt delen, maar u hebt hen niet nodig om het als proef (of als het een dossiertype te bekijken dat niet door [!DNL Workfront Proof] wordt gesteund) te bekijken, kunt u het als dossier aan uw [!DNL Workfront Proof] rekening uploaden. Net als bij proefdrukken kunt u uw bestanden ordenen in mappen, bestanden labelen en een aangepast bericht toevoegen aan het e-mailbericht wanneer u het bestand deelt. Voor meer informatie, zie [&#x200B; Dossiers en de Inhoud van het Web aan  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md) uploaden.

Wanneer uw ontvangers de e-mailmelding ontvangen over een bestand dat u deelt, kunnen ze het bestand downloaden door op de koppeling in het bericht te klikken.

[!DNL Workfront Proof] -gebruikers kunnen bestanden omzetten in proefdrukken nadat ze in hun account zijn opgeslagen.

<!--Is there a limit-->
