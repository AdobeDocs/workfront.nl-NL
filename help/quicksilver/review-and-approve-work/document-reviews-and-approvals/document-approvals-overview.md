---
product-area: documents
navigation-topic: approvals
title: Algemeen overzicht van revisie en goedkeuring
description: Meer informatie over uniforme revisie en goedkeuring van Workfront en Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 32cb95c2-8d12-492b-ad89-b38e2a337fc5
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: c989b5d6a91a4b1f19b044916b4f68a1738f9b16
workflow-type: tm+mt
source-wordcount: '3874'
ht-degree: 0%

---


# Algemeen overzicht van revisie en goedkeuring

De verenigde revisie en goedkeuring brengt Adobe Workfront en Adobe Frame.io samen tot één enkele, diep verbonden ervaring-het dichten van de hiaten tussen marketing beheer, creatief overzicht, en inhoudslevering.
Projectcoördinatoren beheren het werk in Workfront, terwijl ontwerpers, marketers en belanghebbenden hun middelen in de professionele viewer Frame.io controleren en goedkeuren, allemaal zonder bestanden te verplaatsen tussen ontkoppelde gereedschappen.

![&#x200B; Diagram die het verenigde overzicht en goedkeuringswerkschema tonen, met projectcoördinatoren die het werk in Workfront beheren en recensenten en fiatteurs die teruggeven en besluiten nemen in de kijker Frame.io.](assets/Unified-Review-Approvals-Image.png)


## Integratievereisten

* Workfront en Frame.io moeten worden geïmplementeerd in dezelfde Identity Management System (IMS)-organisatie.

* Gebruikers kunnen binnen de IMS-organisatie slechts tot één Workfront-instantie behoren.

* De Workfront-instantie moet zijn ingeschakeld op de Adobe Unified Experience en Adobe Enterprise storage.


## Gebaseerd op Adobe Enterprise Storage

De verenigde revisie en goedkeuring is gebaseerd op Adobe Enterprise Storage — een cloudgebaseerde opslagoplossing die fungeert als centrale opslagplaats voor bedrijfsmiddelen in Adobe, waaronder Workfront en Frame.io. <!--, and Creative Cloud.-->

De belangrijkste voordelen van Adobe Enterprise Storage zijn:

* Geïntegreerde opslaglaag voor creatieve middelen en bedrijfsbeheermiddelen
* Gecentraliseerde machtigingen met het Adobe Identity Management-systeem (IMS) voor veilig toegangsbeheer
* De zichtbaarheid van end-to-end elementen in Workfront en Frame.io <!--, and Creative Cloud apps -->
* Schaalbare opslag en quotabeheer voor bedrijfsbehoeften

Voor meer details, zie [&#x200B; overzicht van de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Geïntegreerde revisie en goedkeuring

Met de verenigde revisie en goedkeuring kunt u:

* Recensies en goedkeuringen rechtstreeks vanuit Workfront maken en beheren
* De status van revisies en goedkeuringen bijhouden in real-time
* Feedback en goedkeuringen op één plaats centraliseren
* Ervoor zorgen dat alle belanghebbenden toegang hebben tot de nieuwste versies van middelen
* AI Reviewers gebruiken om beoordelingen van naleving van merk te automatiseren
* en meer

Voor meer informatie, zie [&#x200B; Verenigde documentgoedkeuringen: artikelindex &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### De viewer Frame.io gebruiken

Met de viewer Frame.io kunt u elementen controleren en goedkeuren. De viewer Frame.io biedt

* Gereedschappen voor markeringen en opmerkingen
* Versiegeschiedenis en vergelijking
* Opmerkingen met tijdstempel voor videorevisies
* Mobiele toegang voor revisies en goedkeuringen onderweg

Voor meer informatie, zie [&#x200B; begonnen worden met verenigde overzicht en goedkeuring &#x200B;](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

#### Limieten voor videorevisie

Er is een jaarlijks maximum voor videoproefdrukaanvragen dat is ingesteld op 10% van de totale betaalde Workfront-gebruikerslicenties voor een organisatie: Standard en Light. Dit plafond wordt toegepast op het niveau van de organisatie.

Workfront-beheerders ontvangen meldingen wanneer het gebruik 80% en 100% van de limiet bereikt.

Deze limiet geldt niet voor Enterprise-klanten van Frame.io.

#### Ondersteunde bestandstypen in de viewer Frame.io

De viewer Frame.io ondersteunt alle gangbare typen video, afbeeldingen, audio, PDF en MS® Office. Voor een gedetailleerde lijst van gesteunde dossiers, zie [&#x200B; Gesteunde Types van Dossier op Frame.io &#x200B;](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Toegang tot en licenties voor de Frame.io-viewer

De viewer Frame.io is de standaardviewer voor alle Workfront-workflows voor revisie en goedkeuring. Deze wordt automatisch opgenomen voor alle Workfront-gebruikers met een betaalde licentie. Er is geen aanvullende Frame.io-licentie vereist als u de Frame.io-viewer wilt gebruiken voor revisies en goedkeuringen.

Als uw organisatie gebruik wil maken van extra Frame.io-functionaliteit die beschikbaar is met deze integratie, zoals het rechtstreeks uploaden van middelen naar projecten in Frame.io, kunt u een Frame.io Enterprise-licentie aanschaffen. Neem contact op met uw Adobe-accountvertegenwoordiger om een demo te plannen en de voordelen van de volledige Frame.io-oplossing te verkennen.

Workfront Proofing-functionaliteit is niet beschikbaar bij deze integratie.

## Krachtig projectbeheer in Workfront

Projectcoördinatoren kunnen gebruikmaken van de krachtige mogelijkheden voor projectbeheer van Workfront om werk te plannen, te volgen en te beheren.

Voor meer informatie over het beheren van projecten in Workfront, zie [&#x200B; Projecten: artikelindex &#x200B;](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Gedwongen conventies voor structuur en naamgeving

Omdat de verenigde overzicht en de goedkeuring gebruikend de ondernemingsopslag van Adobe worden gebouwd, zijn er sommige gedwongen structuur en noemende overeenkomsten om zich van bewust te zijn wanneer het beheren van projecten en documenten.

* Objectnamen moeten uniek zijn en kunnen niet worden gedupliceerd.
* Voor Adobe Enterprise Storage zijn unieke namen nodig voor peer-objecten met hetzelfde bovenliggende element in de hiërarchiestructuur.
* Documenten kunnen niet dezelfde naam hebben als ze tot hetzelfde project behoren.
* Objectnamen mogen geen van de volgende speciale tekens bevatten: \ / : * ? &quot; | &lt; >
* Objectnamen mogen maximaal 255 tekens bevatten.

Met het oog op deze beperkingen wijzigt Workfront automatisch de naam van objecten of documenten om conflicten te voorkomen.

### Delen en machtigingen

Als onderdeel van de integratie, worden de gebruikerstoestemmingen gecontroleerd in Workfront en stroom neer aan Frame.io. Dit betekent u kunt geen gebruiker aan een project in Frame.io uitnodigen of gebruikerstoestemmingen in Frame.io wijzigen. Deze acties moeten worden uitgevoerd via het modaal project voor het delen van projecten in Workfront.

In de volgende tabel wordt aangegeven hoe Workfront-machtigingen worden toegewezen aan Frame.io-machtigingen:

<table>
<tr>
<th>Workfront-gebruikersrechten</th>
<th>Frame.io-gebruikersmachtigingen</th>
</tr>
<tr>
<td>Beheren</td>
<td>Bewerken en delen</td>
</tr>
<tr>
<td>Contribute</td>
<td>Bewerken en delen</td>
</tr>
<tr>
<td>Weergave</td>
<td>Alleen opmerkingen</td>
</tr>
</table>



### Documentbeheer in Workfront

Documenten die naar Workfront worden geüpload, worden opgeslagen in Adobe Enterprise Storage en zijn toegankelijk in zowel Workfront als Frame.io. Wanneer u een document uploadt naar een taak of uitgave in Workfront, wordt een door het systeem gegenereerde map gemaakt in Adobe Enterprise storage die de machtigingen van de taak of uitgave overneemt. Alle documenten die naar die taak of uitgave zijn geüpload, worden in die map opgeslagen en nemen er rechten van over. Voor meer informatie over documenten in Workfront, zie [&#x200B; het nieuwe overzicht van het documentengebied &#x200B;](/help/quicksilver/documents/managing-documents/documents-area.md) en [&#x200B; de toestemmingen van Objecten en het overzicht van het toegangsniveau voor het model van de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Beperkingen voor ervaring met documenten

De volgende documentmogelijkheden zijn niet inbegrepen:

<!--* External document providers-->
* Toegang tot proefdrukken in Workfront
* Documentviewer in Workfront
* Favoriete documenten
* Documenten aanvragen

## Ga aan de slag met de verenigde revisie en goedkeuring

Om met verenigde overzicht en goedkeuring begonnen te worden, zie [&#x200B; begonnen met verenigde overzicht en goedkeuring &#x200B;](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md).

## Veelgestelde vragen

### Aan de slag met één revisie en goedkeuring

+++ Vouw uit om de veelgestelde vragen weer te geven om aan de slag te gaan met één revisie en goedkeuring.

**wat verenigde overzicht en goedkeuring is?**

De verenigde revisie en goedkeuring is een native integratie tussen Adobe Workfront en Adobe Frame.io die werkbeheer en creatieve revisie samenbrengt in één verbonden systeem. Projectcoördinatoren plannen en volgen het werk in Workfront, terwijl revisoren en fiatteurs de professionele viewer Frame.io gebruiken om feedback te geven, elementen te markeren en goedkeuringsbeslissingen te nemen, zonder te schakelen tussen afzonderlijke gereedschappen of bestanden handmatig te verplaatsen.

De controle en de goedkeuring plaatsen bij het centrum van elke inhoudsverrichting. Hier komen creatief werk, inbreng van belanghebbenden en zakelijke beslissingen bij elkaar. Wanneer dat proces over losgemaakte hulpmiddelen-e-maildraden, praatjeberichten, de prijsverhogingen van het schermafbeelding wordt verspreid — de gevolgen samenstelling: langzamere tijd aan markt, verloren terugkoppel, versieconflicten, en tijd bestede het beheren van dossiers in plaats van het creëren van inhoud.

De verenigde overzicht en de goedkeuring richten dit door het lappendeken van losgemaakte overzichtshulpmiddelen met één modern systeem-één enkele bron van waarheid te vervangen die waar het werk reeds gebeurt.

**wat zijn de vereisten om deze integratie te gebruiken?**

Als u een uniforme beoordeling en goedkeuring wilt gebruiken, moet aan de volgende voorwaarden zijn voldaan:

* Workfront en Frame.io moeten worden geïmplementeerd in dezelfde Adobe Identity Management System (IMS)-organisatie.

* Gebruikers kunnen binnen de IMS-organisatie slechts tot één Workfront-instantie behoren.

* De Workfront-instantie moet zijn ingeschakeld op de Adobe Unified Experience en Adobe Enterprise storage.

* Workfront-klanten moeten zich op een V2 SKU bevinden (hiervoor is mogelijk een contractgebeurtenis vereist—neem contact op met uw Adobe-accountvertegenwoordiger).

**heb ik een vergunning Frame.io nodig om deze integratie te gebruiken?**

Nee. De viewer Frame.io wordt automatisch zonder extra kosten opgenomen voor alle Workfront-gebruikers met een betaalde licentie. U hebt geen aparte Frame.io-licentie nodig om elementen via Workfront te bekijken en goed te keuren.

Als uw organisatie toegang tot extra mogelijkheden Frame.io wil — zoals het uploaden van activa rechtstreeks aan projecten in Frame.io — kunt u een vergunning van de Onderneming kopen Frame.io. Neem contact op met uw Adobe-accountvertegenwoordiger voor meer informatie.

**vervangt dit Workfront Proof?**

Ja. Wanneer de verenigde revisie en goedkeuring wordt toegelaten, wordt de kijker Frame.io de primaire revisieoppervlakte in Workfront, die Workfront Proof vervangt.

Bestaande klanten behouden toegang tot de Workfront Proofing-functionaliteit voor alle projecten die zijn gemaakt voordat de integratie is ingeschakeld.

**hoe ik toegang tot Verenigde Overzicht en Goedkeuring krijg?**

**wat moet ik doen om toegang te krijgen?**

Uw organisatie moet zich op een Workfront V2 SKU bevinden om toegang te krijgen tot een uniforme revisie en goedkeuring. Als u momenteel niet op V2 SKU bent, zal dit een contractgebeurtenis met Adobe vereisen. Aan de slag:

* Neem contact op met uw Adobe-accountvertegenwoordiger om te bevestigen of uw huidige Workfront-abonnement ondersteuning biedt voor een uniforme beoordeling en goedkeuring.

* Als een SKU-upgrade nodig is, begeleidt uw accountvertegenwoordiger u door het proces voor het sluiten van contracten.

* Zodra uw account op de juiste SKU staat, configureert Adobe Professional Services de integratie voor uw organisatie.

   * Als u niet zeker weet wie uw Adobe-accountvertegenwoordiger is, kunt u contact opnemen via het Adobe-ondersteuningsportaal of Experience League bezoeken voor contactopties.

+++

### Uniforme revisie en goedkeuring

+++ Vouw uit om de veelgestelde vragen weer te geven over de werking van een uniforme revisie en goedkeuring.

**hoe het overzicht en goedkeuringswerkschema werken?**

De workflow volgt de volgende algemene stappen:

1. Een projectcoördinator maakt een project in Workfront en uploadt of koppelt middelen.

1. Wanneer een middel klaar voor overzicht is, leidt de coördinator tot een goedkeuringswerkschema-of een enig-gebruiksgoedkeuring of door een herbruikbare goedkeuringsmalplaatje toe te passen.

1. Toegewezen revisoren en fiatteurs worden via e-mail op de hoogte gesteld en kunnen het middel rechtstreeks openen in de viewer Frame.io.

1. Revisoren kunnen opmerkingen en markeringen toevoegen. De fiatteurs moeten een formeel besluit nemen.

1. De coördinator volgt de status in real-time van Workfront.

**wat is het verschil tussen een recensent en een fiatteur?**

Revisoren kunnen opmerkingen toevoegen en elementen markeren in de viewer Frame.io. Als ze klaar zijn, markeren ze de revisie als voltooid. Hun actie is echter niet vereist voor de goedkeuringswerkstroom om verder te gaan.

fiatteurs moeten een van de volgende beslissingen nemen om de goedkeuringswerkstroom vooruit te helpen:

* **keur** goed: De activa zijn klaar om ongewijzigd te gebruiken.

* **het werk van behoeften**: De activa vereist veranderingen en moet als nieuwe versie voor hergoedkeuring opnieuw worden voorgelegd.

**Welke types van goedkeuringswerkschema&#39;s kan ik creëren?**

* **goedkeuringen voor eenmalig gebruik**: U kunt een enig-gebruiksgoedkeuring direct op een document in een project, een taak, of een kwestie tot stand brengen. U wijst revisoren en fiatteurs toe, stelt een deadline in en configureert indien nodig meerdere stappen. Geautomatiseerde e-mailherinneringen worden 72 uur voor, 24 uur voor en op de deadline verzonden.

* **malplaatjes van de Goedkeuring**: U kunt herbruikbare malplaatjes in de Opstelling van Workfront tot stand brengen. Een sjabloon definieert de revisoren, fiatteurs en een relatief lange voltooiingstijd. Indien nodig kunt u meerdere fasen maken. Wanneer een sjabloon op een element is toegepast, wordt de deadline automatisch berekend.

**hoe nemen de externe gebruikers aan overzichten deel?**

Externe Workfront-gebruikers worden via e-mail op de hoogte gesteld wanneer ze worden toegewezen aan een revisie of goedkeuring. Zij zullen worden ertoe aangezet om een login Frame.io tot stand te brengen om tot de kijker toegang te hebben en aan het overzichtsproces deel te nemen.

**Hoe volg ik overzicht en goedkeuringsvooruitgang?**

Projectcoördinatoren kunnen alle goedkeuringen tijdens de vlucht op verschillende manieren controleren:

* De widget Mijn goedkeuringen in het gebied Start van Workfront biedt een realtime samenvatting van goedkeuringen die nog in behandeling zijn en die nog moeten worden uitgevoerd.

* De widget Metrische gegevens voor documentgoedkeuring geeft gemiddelde goedkeuringstijden en beslissingsuitsplitsingen weer.

* Aangepaste rapportdashboards kunnen worden ingebouwd in Canvasdashboards voor een grotere zichtbaarheid in revisie- en goedkeuringsactiviteiten.

+++


### Elementen en video&#39;s evalueren en goedkeuren

+++ Vouw uit om de veelgestelde vragen over het controleren en goedkeuren van middelen en video&#39;s weer te geven.

**zijn er om het even welke grenzen op videooverzichten?**

Ja. Er geldt een jaarlijkse limiet voor videoproefdrukken die is ingesteld op 10% van de totale betaalde Workfront-gebruikerslicenties (Standard en Light) voor uw organisatie. Dit plafond geldt op organisatieniveau.

Workfront-beheerders ontvangen meldingen in de app wanneer het gebruik 80% en 100% van de limiet bereikt.

Deze limiet geldt niet voor Enterprise-klanten van Frame.io. Als uw organisatie regelmatig grote hoeveelheden video-inhoud controleert, neemt u contact op met uw Adobe-accountvertegenwoordiger voor meer informatie over de licentie voor Frame.io Enterprise.

**kan de zelfde gebruiker in veelvoudige stadia van een goedkeuringswerkschema verschijnen?**

Ja. Een gebruiker kan worden toegewezen aan meerdere fasen binnen dezelfde goedkeuringswerkstroom.

**kan ik stadia toevoegen om een multi-stadium goedkeuringswerkschema tot stand te brengen?**

Ja. Workflows voor meerfasengoedkeuring worden ondersteund, zodat u elementen in elke fase kunt doorsturen via opeenvolgende toetsings- en goedkeuringsrondes met verschillende deelnemers.

<!--
**Can I modify the trigger for a later stage---for example, based on all approved versus the due date ending?**

Stages in a multi-stage approval workflow proceed sequentially based on all required decisions being made in the current stage. When all assigned approvers in a stage have made their decisions, the next stage begins and the previous stage is locked. There is no option to trigger a stage based on the due date ending. If the "One decision required" toggle is enabled on a stage, the first approver decision completes that stage and advances the workflow.

**Can I remove the due date from an approval?**

Yes. Due dates are optional for both single-use approvals and approval templates. When creating a single-use approval, you can leave the deadline field empty. For approval templates, the relative completion timeframe is also optional.

**Can I change the default due date on new approval templates?**

Yes. When creating or editing an approval template, the timeframe (or "Workdays until due date" for multi-stage templates) can be adjusted per stage or left empty. The deadline is calculated automatically from this timeframe when the template is applied to an asset, so updating the template changes the default for all future approvals that use it.

**What happens when the deadline is reached for a review stage?**

For both single-stage and multi-stage reviews, automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. However, reaching the deadline does not automatically reject the asset, lock the stage, or advance the workflow. Approvers and reviewers can still make decisions or complete their review after the deadline has passed. In a multi-stage workflow, each stage has its own independent deadline, and stages still advance based on all required decisions being made---not based on the deadline.
-->

**kan goedkeuringsmalplaatjes groepen of teams omvatten, of slechts individuele gebruikers?**

Goedkeuringssjablonen ondersteunen momenteel individuele gebruikers en teams.

**zijn goedkeurers per e-mail op de hoogte gebracht wanneer zij iets aan overzicht hebben?**

Ja. fiatteurs en revisoren ontvangen e-mailmeldingen wanneer ze zijn toegewezen aan een revisie of goedkeuring. Geautomatiseerde herinneringse-mails worden ook 72 uur voor de deadline, 24 uur voor, en op de deadline zelf verzonden.

De mogelijkheid om e-mailberichten aan te passen is momenteel niet beschikbaar, maar staat op de routekaart van het product.

<!--
**Can I change the notification frequency for a unified approver or reviewer (for example, all comments, replies to my comments, or daily summaries)?**

No. Notification frequency settings such as receiving all comments, only replies to your comments, or daily digest summaries are not currently available for unified review and approval. The system sends email notifications automatically when a user is assigned as a reviewer or approver, and automated reminder emails are sent at 72 hours, 24 hours, and on the deadline. The ability to customize notification messages and frequency is on the product roadmap.
-->

**kan ik een privé van het overzichtsstadium van andere deelnemers houden?**

Er is momenteel geen functie voor het privéwerkgebied. Als u een revisie privé wilt houden van andere deelnemers, kunt u het beste een aparte kopie van het element maken, die specifiek voor die revisiegroep is bestemd. Opmerkingen worden momenteel niet gesegmenteerd door deelnemersgroep binnen één activum.

Merk op dat de versiegeschiedenis, met inbegrip van vroegere en huidige versies, altijd aan iedereen met toegang zichtbaar is om dat middel te bekijken.

**kan commentaren worden duidelijk zoals opgelost?**

Ja. Opmerkingen kunnen worden gemarkeerd als opgelost in de Frame.io-viewer.

**welke prijsverhoging en annotatiehulpmiddelen in de kijker Frame.io beschikbaar zijn?**

De viewer Frame.io bevat een volledige set visuele opmaakgereedschappen, waaronder vrije tekenvormen en standaardvormen zoals cirkels, pijlen en vierkanten. Voor video-elementen worden opmerkingen voorzien van een tijdstempel met een nauwkeurige framesnelheid. Feedback is daarom altijd gekoppeld aan het exacte tijdstip in de clip en niet alleen aan een algemene tijdstempel.

**zal commentaren die in de kijker Frame.io worden gemaakt in het project van Workfront verschijnen?**

Opmerkingen en annotaties blijven in de viewer Frame.io aanwezig, zodat ze hun volledige context behouden, inclusief tijdstempels en visuele markeringen. Dit kan zich in toekomstige versies ontwikkelen.

**is het mogelijk om commentaren aan een gedownloade versie van activa (b.v., een PDF) toe te voegen?**

Dit wordt momenteel niet ondersteund, maar het is een veelgevraagde functie die wordt overwogen voor een toekomstige release.

**Kan ik veelvoudige activa samen als groep herzien?**

De uitgebreide opties voor bulkrevisie zijn binnenkort beschikbaar. In de tussentijd kunnen elementen van verschillende bestandstypen, zoals een video- en een Word-document, worden opgenomen in een gegroepeerde middelenrevisie.

**is verenigde overzicht en goedkeuring slechts voor video, of steunt het andere dossiertypes?**

De verenigde overzicht en de goedkeuring worden ontworpen voor alle activa types, niet alleen video. De viewer Frame.io is aanzienlijk bijgewerkt ter ondersteuning van afbeeldingen, documenten, PDF&#39;s en andere veelgebruikte bestandsindelingen, naast video.

Raadpleeg de documentatie over door Frame.io ondersteunde bestandstypen op Experience League voor een volledige lijst met ondersteunde bestandstypen.

**Kan ik activa extern met belanghebbenden delen die geen toegang tot Workfront hebben?**

Ja. Assets kan extern worden gedeeld. Externe gebruikers worden via e-mail op de hoogte gesteld en worden gevraagd een Frame.io-aanmeldingsnaam te maken om toegang te krijgen tot de viewer en deel te nemen aan de revisie.

<!--
**Before unified review and approval, is a reviewer just directed to a proof?**

Yes. In the legacy proofing workflow (prior to unified review and approval), when a user was assigned as a reviewer they were directed to the Workfront Proof viewer (ProofHQ) to review the proof. With unified review and approval, reviewers are instead directed to the Frame.io viewer, which replaces the Workfront Proof viewer as the primary review surface.

**When I upload a document and not a proof, a proof gets generated. Will a proof always be generated?**

No. With unified review and approval enabled and Adobe enterprise storage active, uploading a document does not automatically generate a proof. Documents are stored in Adobe enterprise storage and are reviewed using the Frame.io viewer. A proof is only generated if you explicitly create one using the legacy proofing workflow. The Frame.io viewer serves as the primary review surface, so a separate proof is not needed for standard review and approval workflows.

**What is the difference between uploading a document and a proof after the 26.2 release?**

With unified review and approval enabled, uploading a document stores it in Adobe enterprise storage and makes it available for review in the Frame.io viewer. A unified approval workflow can be created directly on the document. Uploading a proof, by contrast, uses the legacy Workfront Proof viewer (ProofHQ) and its own proofing workflow. Both options are available for projects created before the integration was enabled, but the Frame.io viewer is the primary review surface going forward. The key difference is that a document uses the unified approval workflow and Frame.io viewer, while a proof uses the legacy proofing workflow and viewer.

**Reviews under My Approvals only show a "Complete my review" button and no link to the proofing viewer or the document. Is this intended?**

For unified review and approval, the My Approvals widget provides an "Open review" button that opens the asset in the Frame.io viewer, as well as action buttons to approve, request changes, or complete a review. Reviewers can complete their review directly from the widget. If you are only seeing a "Complete my review" button without a link to the viewer, this may reflect the reviewer role behavior---reviewers are not required to open the asset to mark their review as complete, though they can choose to open it in the Frame.io viewer to provide feedback before completing.

**Before unified review and approval, if a user is both an approver in a document approval and a reviewer/approver on a proof, both show up in the proof window. How do these work together?**

When using unified approvals alongside legacy proofing on the same document, the two workflows operate independently. Document approval participants are shown in the Document Summary panel, while proof participants are shown in the proofing workflow. The SOCD (Sent, Opened, Comment, Decision) indicators in the document list are proofing-related and do not reflect the unified approval decision status. These two workflows do not automatically sync---a decision made in one does not carry over to the other.

**If you upload a new version, the document approval users do not get repopulated. Is that intended?**

Yes. When a new version is uploaded, previous approval participants are not automatically repopulated. The previous version's approval process is closed and any outstanding approvals are marked as "Withdrawn." The document owner must manually add participants to the new version's approval workflow. An "Add all" button is available to quickly repopulate all participants from the previous version, and you can also selectively add previous participants or add new ones.
-->

+++

### Opslag- en bestandsbeheer

+++ Vouw uit om de veelgestelde vragen over opslag en bestandsbeheer weer te geven.

**wat is de ondernemingsopslag van Adobe en hoe verhoudt het zich tot deze integratie?**

Adobe Enterprise storage is de algemene opslaglaag die Workfront, Frame.io en Adobe Creative Cloud verbindt. Assets werkt op één locatie en is zonder handmatige bestandsoverdracht toegankelijk voor alle gereedschappen. Creatieven kunnen werken en revisoren zien altijd de nieuwste versie.

De belangrijkste voordelen van Adobe Enterprise Storage zijn:

* Eén opslaglaag voor alle bestanden in uitvoering, in Workfront en Frame.io

* Gecentraliseerd toegangsbeheer beheerd via Adobe Identity Management System (IMS)

* Zichtbaarheid van end-to-end element—geen versieverschuiving, geen verloren metagegevens

* Schaalbaar opslagbeheer op bedrijfsniveau

**zijn er het noemen of structuurvereisten voor dossiers en projecten?**

Ja. Omdat de integratie gebruikmaakt van Adobe Enterprise-opslag, zijn de volgende conventies van toepassing:

* Namen van objecten en documenten moeten uniek zijn binnen hetzelfde bovenliggende element in de mappenhiërarchie.

* Documenten binnen hetzelfde project kunnen geen naam delen.

* Namen van programma&#39;s, portfolio&#39;s, projecten, sjablonen, taken, uitgaven, documenten en documentmappen mogen niet de volgende speciale tekens bevatten: `\\ / : \* ? \" \| \< \>` en zijn beperkt tot 255 tekens.

Workfront wijzigt automatisch de naam van objecten of documenten als dat nodig is om conflicten te voorkomen.

**Welke dossiertypes in de kijker Frame.io worden gesteund?**

De viewer Frame.io ondersteunt meer dan 40 bestandsindelingen, waaronder alle gangbare video-, afbeeldings-, audio-, PDF- en Microsoft Office-typen. Ondersteuning voor video omvat native afspelen voor professionele indelingen zoals ProRes, H.265 en DNxHD, met ondersteuning voor bestanden tot 500 GB.

Frame.io is speciaal ontwikkeld voor creatieve revisie, wat betekent dat het alle typen elementen verwerkt waarmee marketing- en creatieve teams werken.

+++

### Machtigingen en toegang

+++ Vouw uit om de veelgestelde vragen over machtigingen en toegang weer te geven.

**hoe worden de gebruikerstoestemmingen beheerd?**

Gebruikersmachtigingen worden ingesteld en beheerd in Workfront en worden automatisch doorgevoerd in Frame.io. U kunt geen gebruikers uitnodigen of toestemmingen direct in Frame.io voor deze integratie wijzigen. Al toegangsbeheer moet worden gedaan gebruikend het project aandeel modaal in Workfront.

In de onderstaande tabel ziet u hoe Workfront-machtigingen worden toegewezen aan Frame.io-machtigingen:

<table>
  <thead>
    <tr>
      <th>Workfront-machtiging</th>
      <th>Frame.io-machtiging</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Beheren</td>
      <td>Bewerken en delen</td>
    </tr>
    <tr>
      <td>Contribute</td>
      <td>Bewerken en delen</td>
    </tr>
    <tr>
      <td>Weergave</td>
      <td>Alleen opmerkingen</td>
    </tr>
  </tbody>
</table>

+++


### Integratie en geavanceerde mogelijkheden

+++ Vouw uit om de veelgestelde vragen over integratie en geavanceerde mogelijkheden weer te geven.

**hoe beïnvloedt dit de bestaande insteekmodules van Creative Cloud met Adobe Express en GenStudio?**

Integraties die de viewerervaring van Frame.io ondersteunen, zijn momenteel in ontwikkeling voor Adobe Express en GenStudio Performance Marketing. De nieuwe integratie zal op het zelfde verenigde overzicht en goedkeuringssysteem worden voortgebouwd, zodat zullen zij hefboomwerking de kijker Frame.io voor een verenigbare overzichtservaring over alle drie producten.

**is Frame.io geïntegreerd binnen Workfront, of navigeren de gebruikers aan een afzonderlijke interface?**

Gebruikers kunnen de viewer Frame.io rechtstreeks vanuit Workfront starten. Alle revisie- en goedkeuringsactiviteiten vinden plaats in de viewer Frame.io en worden automatisch weer gesynchroniseerd naar Workfront.

**Kan ik goedgekeurde activa naar Adobe Experience Manager (AEM) verzenden?**

Ja. Zodra een middel de herbeoordeling en goedkeuringscyclus voltooit, kunt u het naar Adobe Experience Manager Assets voor definitieve opslag en distributie overbrengen. Hierdoor wordt Workfront for work management, Frame.io for review en AEM for digital asset management verbonden met een supply chain voor uniforme inhoud.

Voor meer informatie, zie voor meer informatie, [&#x200B; Gebruik Adobe Experience Manager met de integratie Frame.io &#x200B;](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

**hoe verenigde overzicht en goedkeuring in Adobe GenStudio past?**

De verenigde overzicht en de goedkeuring is een grondcomponent van Adobe GenStudio-Adobe bredere visie voor een verbonden inhoud supply chain. GenStudio maakt van Workfront, Frame.io, Creative Cloud, Adobe Express, Adobe Experience Manager Assets en GenStudio for Performance Marketing een uniforme workflow, van campagnemateriaal tot levering van inhoud.

In dat ecosysteem fungeren evaluatie en goedkeuring als het kritieke eindpunt tussen creatie en levering. Op deze locatie komt creatief werk overeen met de inbreng van belanghebbenden, wordt de kwaliteit gevalideerd en kan de inhoud worden gepubliceerd. Wanneer die handoff snel, zichtbaar, en betrouwbaar is, ontgrendelt het snelheid over de volledige inhoud supply chain-AI kan verwezenlijking versnellen, kan de automatisering distributie behandelen, maar een knelpunt in overzicht kapt de winst aan beide kanten. Door Workfront en Frame.io aan te sluiten, wordt dat knelpunt verwijderd.

**wat is de AI eigenschap van de Recensent?**

De verenigde revisie en goedkeuring omvat een AI Reviewer-functie die controles op de naleving van de brandwerendheid automatiseert als onderdeel van het revisieproces. De AI Reviewer kan middelen beoordelen aan de hand van richtlijnen van het merk en mogelijke problemen markeren voordat menselijke revisoren worden betrokken, zodat teams problemen sneller kunnen ondervangen en sneller kunnen gaan.

Raadpleeg de documentatie bij Workfront op Experience League voor meer informatie over het instellen en gebruiken van AI Reviewer.

+++

### Contracten, SKU&#39;s en opslag

+++ Vouw uit om de veelgestelde vragen over contracten, SKU&#39;s en opslag weer te geven.

**wanneer verenigde overzicht en goedkeuring aan me beschikbaar zal zijn?**

De verenigde revisie en goedkeuring zijn nu beschikbaar. Voor toegang is een upgrade naar een Workfront V2 SKU vereist. Als uw contract werd ondertekend alvorens V2 SKUs beschikbaar was, kunt u tot toegang op één van twee manieren verkrijgen:

* Bij verlenging: Toegang wordt ingeschakeld op de volgende datum van contractvernieuwing.

* Vroege hercontractering: uw Adobe-accountteam kan u snel opnieuw contracteren om de nieuwe SKU-rechten toe te voegen terwijl de einddatum van uw bestaande contract behouden blijft. Er is geen prijsverhoging wanneer naar een gelijkwaardig pakket wordt overgegaan.

Neem contact op met uw Adobe-accountvertegenwoordiger om het beste pad voor uw organisatie te bepalen.

<!--
**Before we sign the contract, what changes will we see in Workfront?**

Before signing the V2 SKU contract, your Workfront instance will continue to operate using the existing document and proofing experience. No unified review and approval features---such as the Frame.io viewer, Adobe enterprise storage, or multi-stage approval templates---will be available until the V2 SKU is contracted and Adobe Professional Services configures the integration for your organization.
-->

**geeft de bevordering aan V2 SKU me meer opslag?**

Ja. Met de V2 SKU krijgt elke gebruiker met licentie 60 GB opslagruimte, tot 30 GB in de vorige versie.

**hoe ik tussen de ondernemingsopslag van Adobe en erfenisopslag van Workfront kies?**

Enterprise Storage maakt de viewerervaring van Frame.io mogelijk en is vereist voor uniforme revisie en goedkeuring. Bij verouderde opslag wordt standaard de Workfront Proof-viewer (ProofHQ) gebruikt.

Als uw organisatie een combinatie van eenvoudige werkstromen en complexere het proefdrukken werkschema&#39;s heeft, kunt u aan welke werkschema&#39;s voorrang geven om eerst te migreren.

Opslag op bedrijfsniveau biedt u de flexibiliteit om de nieuwe ervaring stapsgewijs uit te voeren, te beginnen met de workflows die de meeste voordelen opleveren.

**hoe worden de vergunningen Frame.io beheerd?**

Na ondertekening van de V2 SKU hebben alle Workfront-gebruikers toegang tot de Frame.io-viewer voor revisie- en goedkeuringswerkstromen. Hiervoor is geen aparte Frame.io Enterprise-licentie vereist.

Als uw organisatie aanvullende Frame.io Enterprise-functies nodig heeft, zoals

* Geavanceerde watermerken (dynamisch en forensisch)
* Digitaal rechtenbeheer met automatische verwijdering van bedrijfsmiddelen
* Inhoudsreferenties voor door AI gegenereerde inhoud
* Aangepaste creatieve metagegevens
* Integraties van Camera naar Cloud
* Uw eigen werkruimte voor creatief werk in uitvoering

U kunt met uw Adobe-accountteam het juiste aantal Frame.io Enterprise-licenties bepalen. Alle licenties worden beheerd via de Adobe Admin Console.

+++

### Sandbox en rollout

+++ Vouw uit om de veelgestelde vragen over de sandbox en rollout weer te geven.

**Kan ik verenigde overzicht en goedkeuring in een zandbakmilieu testen?**

gedeeltelijk. Goedkeuringswerkstromen kunnen worden getest in een Workfront-sandboxomgeving. De viewerervaring voor Frame.io is echter niet beschikbaar in de sandbox. Voor het testen van het oppervlak van de revisie zelf is een productieomgeving vereist.

Als u de belichting tijdens de rollout wilt beperken, kunt u een uniforme revisie en goedkeuring voor een specifieke groep in uw Workfront-productieomgeving inschakelen. Hierdoor kunt u een doelpiloot met een kleinere groep gebruikers uitvoeren voordat u een grotere rol gaat spelen.

<!--
**How should we test future quarterly releases involving unified review and approval if the Frame.io viewer is not available in sandbox?**

Because the Frame.io viewer experience is not available in the Workfront sandbox environment, testing future quarterly releases should be done using a controlled pilot group in your production environment. You can enable unified review and approval for a specific group within your Workfront production instance, allowing a smaller set of users to validate new features as they release. Approval workflow configuration and template setup can still be tested in sandbox, but the full review experience---including the Frame.io viewer---must be validated in production.
-->

+++

### Interactieve proefdrukken en HTML

+++ Vouw uit om de veelgestelde vragen voor interactieve proefdrukken en HTML weer te geven.

**steunt verenigde overzicht en goedkeuring interactieve proeven of HTML URLs?**

Zip HTML-bestanden worden momenteel ondersteund voor interactieve revisie. Ondersteuning voor HTML URL (live web URL review) staat op de routekaart en wordt verwacht in het derde kwartaal.

Raadpleeg de Workfront-releaseopmerkingen op Experience League voor updates.

+++

### Fusie en automatisering

+++ Breid uit om de veelgestelde vragen over Fusion en automatisering weer te geven.

**heb ik de Fusie van Workfront nodig om verenigde overzicht en goedkeuring te gebruiken?**

Nee. De verenigde overzicht en de goedkeuring is een inheemse productintegratie en vereist geen Fusie. De workflow is direct ingebouwd in Workfront.

**de schakelaars van de Fusie voor verenigde overzicht en goedkeuring beschikbaar zullen zijn?**

Ja. Fusieacties voor uniforme evaluatie en goedkeuring zijn momenteel in ontwikkeling en zullen naar verwachting beschikbaar zijn in het derde kwartaal. Raadpleeg de Workfront-releaseopmerkingen op Experience League voor updates zodra deze beschikbaar zijn.

**kan Fusie worden gebruikt om een overzicht automatisch teweeg te brengen wanneer een document wordt geupload?**

Ja. Dit type automatisering is mogelijk met Workfront-webhaken in combinatie met Fusion.

**Hoe zullen de bestaande die werkschema&#39;s van de Fusie op Workfront Proof worden voortgebouwd worden beïnvloed?**

Het effect hangt af van de manier waarop elke workflow wordt samengesteld. In het algemeen:

* **geef uit of werk** bij: De werkschema&#39;s waar de bestaande op proef betrekking hebbende actie een direct equivalent in verenigde goedkeuringen heeft kunnen worden bijgewerkt om de nieuwe actie te gebruiken.

* **herbouwt**: De werkschema&#39;s waar de onderliggende stappen beduidend zijn veranderd, of waar de nieuwe mogelijkheden bestaan, kunnen van kras moeten worden herbouwd.

Zodra de Fusion API&#39;s voor uniforme goedkeuringen beschikbaar zijn, zal er een duidelijker beeld ontstaan. Men adviseert om uw bestaande werkschema&#39;s van de Fusie te controleren en hen tegen de nieuwe verenigde goedkeuringsmogelijkheden op dat ogenblik te evalueren.

+++






