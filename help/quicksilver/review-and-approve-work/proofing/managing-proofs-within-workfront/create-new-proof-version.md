---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een nieuwe versie van een proefdruk maken
description: Het beheren van feedback in meerdere versies of revisies van een stuk werk kan een enorme uitdaging zijn. Workfront vereenvoudigt dit proces door meerdere versies van een proefdruk te maken en te vergelijken.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1454'
ht-degree: 0%

---

# Een nieuwe versie van een proefdruk maken

<!-- Audited: 4/2025 -->

Het beheren van feedback in meerdere versies of revisies van een stuk werk kan een uitdaging zijn. Adobe Workfront vereenvoudigt dit proces door meerdere versies van een proefdruk te maken en te vergelijken.

Houd rekening met het volgende wanneer u een nieuwe versie van een proefdruk maakt:

* U kunt een gebruiker toestemming geven om één versie maar niet een andere te zien. Omgekeerd, als u een recentere versie met een gebruiker deelt, kan die gebruiker vroegere versies niet zien tenzij u teruggaat en hen toegang tot die vorige versies verleent.
* Als u een nieuwe versie wilt maken, hebt u bewerkingsrechten nodig op de proefdruk.

  Voor meer informatie, zie [ de Rollen van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) beheren en [ Profielen van de Toestemmingen van de Bewijs in Workfront Proof ](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

  Zie voor informatie over het delen van proefversies  [ Deel een Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Als er een proefdruk wordt gemaakt in Adobe Workfront, moeten er ook nieuwe versies voor die proefdruk worden gemaakt in Workfront. U kunt in Workfront Proof geen nieuwe versie van een proefdruk maken als die proefdruk in Workfront is gemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werken of plannen</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot documenten bewerken</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nieuwe proefdrukversie maken in Workfront

Er zijn verschillende manieren om een nieuwe proefversie te uploaden in Workfront. De standaardproefdrukinstellingen kunnen afhankelijk van de geselecteerde methode al dan niet worden overgenomen uit de vorige versie:

* **produceert automatisch proeven wanneer het uploaden van documenten**: Als u dit plaatsen die in uw gebruikersprofiel wordt toegelaten hebt, dragen de standaardproefdrukmontages niet over wanneer u sleept en een nieuwe versie laat vallen.
* **creeer proef > Eenvoudig**: Als u deze optie selecteert, dragen de standaardproefdrukmontages niet van de vorige versie over.
* **voeg nieuw toe > Versie > Bewijs**: Als u deze optie selecteert, dragen de standaardproefdrukmontages van de vorige versie over.
* **creeer proef > Geavanceerd**: Als u deze optie selecteert, dragen de standaardproefmontages van de vorige versie over.

Een nieuwe versie van een proefdruk maken:

1. Open de documentlijst met de proefdruk.
1. Sleep vanuit het bestandssysteem van uw computer een nieuw bestand over de proefdruk.

   of

   Selecteer de rij waar de proef vermeld is, klik **nieuwe** toevoegen > **Versie**, dan klik de optie u wilt gebruiken om de nieuwe versie van de proef toe te voegen.

   ![ voeg nieuwe versie ](assets/add-new-proof-version.png) toe

## Een nieuwe proefdrukversie maken met de proefdrukviewer (alleen Workfront Proof)

Als u de standalone Workfront Proof gebruikt, kunt u een nieuwe versie van een proef tot stand brengen die één enkel dossier of Web vangt bevatten. 

>[!NOTE]
>
>Als uw account zich op een Enterprise-abonnement bevindt en u meerdere bestanden of webvastleggingen uploadt, worden deze automatisch gecombineerd in één nieuwe versie. Gelieve te zien [ een multipage bewijs ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) voor meer informatie creëren.

Een nieuwe versie van een proefdruk maken in Workfront Proof:

1. Open de proefdruk.
1. In de upper-left hoek, klik het **drop-down menu van de Versie**, dan klik **+ Nieuwe versie** in de doos die verschijnt. De nieuwe pagina met proefdrukversies wordt geopend.

   ![ voeg nieuwe versie ](assets/new-version-button.png) toe

1. In **voeg dossiers** sectie toe, upload een dossier als nieuwe proefversie door het van uw computer te slepen en te laten vallen of door **te klikken doorbladert** en een dossier te selecteren.

   of

   Leg een webpagina vast als een nieuwe versie van de proefdruk door een URL in te voeren.

   >[!NOTE]
   >
   >Slepen en neerzetten is alleen beschikbaar in browsers die HTML5 volledig ondersteunen. Internet Explorer 7 tot en met 9 en Safari zijn hiervan uitgesloten.

1. (Optioneel) Selecteer de proeftitel en voer een nieuwe **proefdruknaam** voor de versie in.

1. In de **sectie van het Werkschema**, maak om het even welke volgende veranderingen om controleurs voor deze proefdrukversie toe te voegen (dit zal de recensenten van de vorige versie vervangen):

   * (Facultatief) verander de **Eigenaar** van de versie in een andere gebruiker in uw rekening.

     Voor informatie, zie [ Profielen van de Toestemmingen van de Bewijs in Workfront Proof ](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * (Facultatief) Gebruikend de **het contactnaam of e-mailadres van het Type om een ontvankelijke** doos toe te voegen, voeg recensenten aan de versie toe. U kunt de rol van het a **Bewijs** en **e-mailalarm** type voor elke ontvanger dan selecteren.

     Voor informatie, zie [ Groepen aan een Bewijs ](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md) toevoegen en [ Beheren de Rollen van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

     >[!NOTE]
     >
     >Als de de bewijsschepper of eigenaar heeft het Made e-mail van het Bewijs door gebrek in hun persoonlijke montages wordt onbruikbaar gemaakt, zullen zij geen Bewijs of Nieuwe proefe-mails ontvangen zelfs als **ontvangers van de Prijsverklaring over deze proefdruk** doos op de Nieuwe proefdrukpagina wordt gecontroleerd. Voor informatie, zie [ de montages van het e-mailbericht in Workfront Proof ](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) vormen, [ het Bewijs e-mail ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) maakte, en [ Nieuwe proef e-mail ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md).

   * (Optioneel) Stel een proefdrukdeadline in.

   * (Facultatief en Voorwaardelijk) selecteer een nieuwe primaire besluitvormer in de **primaire beslissingsrechten van de Overdracht aan** drop-down.

   * (Facultatief) selecteer **vereisen slechts één besluit voor dit stadium** vakje om de optie te verwijderen om een gebruiker als nieuwe primaire besluitvormer te plaatsen.

1. In de **E-mail- bericht** sectie, selecteer om het even welke volgende montages:

   * (Facultatief) **breng ontvangers op de hoogte over deze proef**: Selecteer deze optie om de recensenten van de nieuwe versie op de hoogte te brengen. Uw selectie zal het programma worden geopend in de **sectie van de Activiteit** van de **pagina van de details van het Bewijs**. Voor meer informatie, zie [ Beheren de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * (Voorwaardelijk en Facultatief) **voeg douaneonderwerp en bericht** toe: Selecteer deze optie om een lijn en een bericht van het douaneonderwerp aan het e-mailbericht toe te voegen.

1. In de **sectie van de Organisatie**, selecteer om het even welke volgende montages:

   * Pas een of meer labels toe op de proefdruk. Voor meer informatie, zie [ Codes in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md) creëren en beheren.

   * Voeg de versie toe aan een map. De map wordt gekopieerd uit de vorige versie van de proefdruk. Als u een andere map selecteert, wordt de hele proefdruk (die alle versies omvat) verplaatst. Voor meer informatie, zie [ Mappen in Workfront Proof beheren ](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

   * De facturerende beheerders en de Beheerders kunnen het omslaggebied over de volledige rekening in de **Montages** tabel verplicht maken.

1. In de **sectie van de Montages van het Bewijs**, selecteer om het even welke volgende montages:

   * Een gebruiker moet zich aanmelden om de proefdruk te bekijken.
   * Vereisen elektronische handtekeningen op het bewijs (ondernemingsplan slechts).
   * Vergrendel het bewijs wanneer alle beslissingen worden genomen.
   * Downloaden van het oorspronkelijke bestand toestaan.
   * Openbaar delen van het bewijs toestaan.
   * Abonneren op de proefdruk toestaan.

     De selecties die in deze sectie worden gemaakt zullen in de **pagina van de Details van het Bewijs** worden getoond (waar sommige gebieden kunnen worden uitgegeven). Voor meer informatie, zie [ Beheren de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Create a new version of a proof from the proofing viewer</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create a new version from the proofing viewer</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof.</li>
<li value="2"> <p>Click the <strong>Version</strong> drop-down menu in the upper-left corner, then click <strong>+ New version</strong> in the box that appears.</p> <p>On the <strong>New proof version of</strong> page that appears, you can see all the reviewers from the previous version, including their roles and email notification settings. You can easily edit the roles and notifications of existing reviewers or remove existing reviewers from the new version on this page.</p> </li>
<li value="3"> <p>Under <strong>Add files</strong>, upload a file as a new version of the proof by dragging and dropping from your computer or by clicking <strong>browse</strong> and selecting the file you want. You can type a&nbsp;<strong>Proof name</strong>&nbsp;for the version or leave this box blank to&nbsp;use the same filename with a version number added on the end.</p> <p>Or<br></p> <p>Capture a web page as a new version of the proof by typing a URL</p> <note type="note">
Drag and drop is available only with browsers that fully support HTML5. This excludes Internet Explorer 7 through 9 and Safari.
<br>
</note> </li>
<li value="4"> <p>Under <strong>Workflow</strong>, make any of the following changes to specify the reviewers for this version of the proof.</p> <p>Reviewers from the previous version are replaced by the reviewers you add.</p>
<ul>
<li>Change the <strong>Owner</strong> of the version to another user in your account.<br>For information about owner permissions, see <a href="../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md" class="MCXref xref">Proof Permissions Profiles in Workfront Proof</a>.</li>
<li> <p>Using the <strong>Type contact name or email address to add a recipient box</strong>, add reviewers to the version. You can specify a <strong>Proof role</strong> and an <strong>Email alerts</strong> type for each recipient.</p> <p>For information about adding groups to the proof, see&nbsp;<a href="../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md" class="MCXref xref">Add Groups to a Proof</a>.&nbsp;For information about roles, see <a href="../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md" class="MCXref xref">Manage Proof Roles in Workfront Proof</a>.</p> <note type="note">
If the creator or owner of&nbsp;&nbsp;the proof has
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> disabled by default (in their personal settings), they won't receive any Proof made or New proof emails even if the Notify people by email box is checked on the New proof page. For information about email notifications, see
<a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Configure email notification settings in Workfront Proof</a>.&nbsp;See also
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">The Proof Made email</a> and
<a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">New proof email</a>.
<br>
</note> </li>
<li>Set a proof deadline for the version.</li>
<li>Hover over a reviewer's name to see any decisions he or she made on a previous version.</li>
</ul> </li>
<li value="5">Under <strong>Email notification</strong>, do any of the following:
<ul>
<li>Specify whether you want to notify the reviewers of the new version.<br>Your selection will be logged in the Proof activity section on the Proof details page.</li>
<li>Add a custom subject and message.</li>
</ul></li>
<li value="6">Under Proof settings, make any of the changes below:
<ul>
<li>Require login on the proof</li>
<li>Require electronic signatures on the proof (Enterprise plan only)</li>
<li>Lock the proof when all decisions are made</li>
<li>Allow or block download of original file</li>
<li>Public sharing of the proof,&nbsp;including public sharing settings</li>
<li>Subscription to the proof<br>The selections made in this section will be shown in the Proof details page.</li>
</ul></li>
</ol>
-->

## Het bericht Nieuwe versie

Als de vorige versie van de proefdruk een aangepast onderwerp/bericht bevat, wordt dit bericht standaard weergegeven op de pagina Nieuwe versie. U kunt:

* Bewerk het onderwerp en het bericht.
* Schakel het selectievakje Personen per e-mail waarschuwen uit. Dit betekent dat er geen e-mail naar de controleurs wordt verzonden om hen te laten weten dat ze een nieuwe versie hebben die ze kunnen controleren.

  >[!NOTE]
  >
  >Dit wordt niet beïnvloed door een standaardaangepast onderwerp/bericht dat in uw persoonlijke instellingen wordt opgeslagen.

Als u een standaardonderwerp en een bericht hebt opgeslagen in uw persoonlijke montages, zal dit bepalen welk bericht door gebrek op de Nieuwe versiepagina wordt getoond:

* Als u de controleurs via de standaard-e-mail op de hoogte hebt gebracht van de vorige proefversie (bijvoorbeeld geen aangepast onderwerp/bericht), wordt uw aangepaste onderwerp/bericht (uw persoonlijke instellingen) weergegeven op de pagina Nieuwe versie. Vervolgens kunt u het aangepaste onderwerp en het aangepaste bericht bewerken of de selectie van Personen per e-mail op de hoogte stellen opheffen. Dit houdt in dat er geen e-mail naar de revisoren wordt verzonden om hen te laten weten dat ze een nieuwe versie hebben die moet worden gecontroleerd.
* Als u de controleurs niet op de hoogte hebt gebracht van de vorige proefversie (bijvoorbeeld geen standaard of aangepast e-mailbericht), bevat de pagina Nieuwe versie standaard geen bericht. Als u de controleurs op de hoogte wilt stellen van de nieuwe versie, klikt u op de koppeling Bericht verzenden. Deze koppeling geeft uw standaardaangepast onderwerp/bericht weer (volgens uw persoonlijke instellingen). Vervolgens kunt u het aangepaste onderwerp en het aangepaste bericht naar wens bewerken.

Als u geen standaardonderwerp en -bericht hebt opgeslagen in uw persoonlijke instellingen, wordt het volgende weergegeven op de pagina Nieuwe versie:

* Als u de controleurs via de standaard-e-mail op de hoogte hebt gebracht van de vorige proefversie (bijvoorbeeld geen aangepast onderwerp/bericht), wordt de optie Personen per e-mail waarschuwen standaard geselecteerd op de pagina Nieuwe versie. Als u een aangepast bericht wilt toevoegen, klikt u op de koppeling.
* Als u de controleurs niet op de hoogte hebt gebracht van de vorige proefversie (bijvoorbeeld geen standaard of aangepast e-mailbericht), bevat de pagina Nieuwe versie standaard geen bericht. Als u de controleurs op de hoogte wilt stellen van de nieuwe versie, klikt u op de koppeling Bericht verzenden. Vervolgens kunt u een aangepast onderwerp en bericht toevoegen door op de koppeling Aangepast bericht toevoegen te klikken.
