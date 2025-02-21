---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Een nieuwe versie van een proefdruk maken
description: Het beheren van feedback in meerdere versies of revisies van een stuk werk kan een enorme uitdaging zijn. Workfront vereenvoudigt dit proces door meerdere versies van een proefdruk te maken en te vergelijken.
author: Courtney
feature: Digital Content and Documents
exl-id: ee0c859e-349b-4e7a-ac80-164740b950f0
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1737'
ht-degree: 0%

---

# Een nieuwe versie van een proefdruk maken

Het beheren van feedback in meerdere versies of revisies van een stuk werk kan een enorme uitdaging zijn. Workfront vereenvoudigt dit proces door meerdere versies van een proefdruk te maken en te vergelijken.

Neem de volgende informatie in overweging wanneer u een nieuwe versie van een proefdruk maakt:

* U kunt een gebruiker toestemming geven om één versie maar niet een andere te zien. Omgekeerd, als u een recentere versie met een gebruiker deelt, kan die gebruiker vroegere versies niet zien tenzij u teruggaat en uitdrukkelijk de gebruikerstoegang tot die vorige versies verleent.
* Als u een nieuwe versie van een proefdruk wilt maken, moet u over bewerkingsrechten op de proefdruk beschikken.

  Zie [ de Rollen van het Bewijs in Workfront Proof beheren ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) en [ Profielen van de Toestemmingen van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) om meer informatie te krijgen over wie rechten op een proef uitgeeft heeft.

  Zie voor informatie over het delen van proefversies  [ Deel een Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md).

>[!IMPORTANT]
>
>Als er in Adobe Workfront een proefdruk wordt gemaakt, moeten ook nieuwe versies voor die proefdruk in Workfront worden gemaakt. U kunt in Workfront Proof geen nieuwe versie van een proefdruk maken als die proefdruk in Workfront is gemaakt.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig abonnement: Pro of hoger</p> <p>of</p> <p>Verouderd abonnement: Selecteren of Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref"> Toegang tot het proefdrukken van functionaliteit in Workfront </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werk of Plan</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, rol, of Profiel van de Toestemming van het Bewijs u hebt, contacteer uw beheerder van Workfront of van Workfront Proof.

+++

## Een nieuwe versie van een proefdruk maken in Workfront

Er zijn verschillende manieren om een nieuwe proefversie te uploaden in Workfront. De standaardproefdrukinstellingen kunnen afhankelijk van de gekozen methode al dan niet worden overgenomen uit de vorige versie:

* **produceert automatisch proeven wanneer het uploaden van documenten**: De standaardproefdrukmontages dragen niet over. Als u deze instelling hebt ingeschakeld in uw gebruikersprofiel, worden de standaardproefdrukinstellingen niet overgedragen wanneer u een nieuwe versie sleept en neerzet.
* **creeer proef > Eenvoudig**: De standaardproefdrukmontages dragen niet over. Als u bij het maken van een nieuwe proefversie de optie Eenvoudig kiest, worden de standaardproefdrukinstellingen niet overgenomen uit de vorige versie.
* **voeg nieuw toe > Versie > Bewijs**: De standaardproefmontages dragen van de vorige versie over.
* **creeer bewijs > Geavanceerd**: De standaardproefmontages dragen over van de vorige versie.

  <table>
  <tbody>
  <tr>
  <td>Automatisch proefdrukken genereren bij het uploaden van documenten</td>
  <td>Standaardproefdrukinstellingen worden niet overgedragen. Als u deze instelling hebt ingeschakeld in uw gebruikersprofiel, worden de standaardproefdrukinstellingen niet overgedragen wanneer u een nieuwe versie sleept en neerzet.</td>
  </tr>
  <tr>
  <td>Proef maken &gt; Eenvoudig</td>
  <td>Standaardproefdrukinstellingen worden niet overgedragen. Als u bij het maken van een nieuwe proefversie de optie Eenvoudig kiest, worden de standaardproefdrukinstellingen niet overgenomen uit de vorige versie.</td>
  </tr>
  <tr>
  <td>Nieuw &gt; Versie &gt; Proef toevoegen</td>
  <td>De standaardproefdrukinstellingen worden overgenomen van de vorige versie.</td>
  </tr>
  <tr>
  <td>Proef maken &gt; Geavanceerd</td>
  <td>De standaardproefdrukinstellingen worden overgenomen van de vorige versie.</td>
  </tr>
  </tbody>
  </table>




Een nieuwe versie van een proefdruk maken:

1. Open de documentlijst met de proefdruk.
1. Sleep vanuit het bestandssysteem van uw computer een nieuw bestand over de proefdruk.

   of

   Selecteer de rij waar de proef vermeld is, klik **nieuwe** toevoegen > **Versie**, dan klik de optie u wilt gebruiken om de nieuwe versie van de proef toe te voegen.

   ![ voeg nieuwe versie ](assets/add-new-version-350x185.png) toe

## Een nieuwe versie van een proefdruk maken met de proefdrukviewer (alleen Workfront Proof)

Als u de standalone Workfront Proof gebruikt, kunt u een nieuwe versie van een proef tot stand brengen die één enkel dossier of Web vangt bevatten. 

>[!NOTE]
>
>Als uw account zich op een Enterprise-abonnement bevindt en u meerdere bestanden of webvastleggingen uploadt, worden deze automatisch gecombineerd in één nieuwe versie. Gelieve te zien [ een multipage bewijs ](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md) voor meer informatie creëren.

Een nieuwe versie van een proefdruk maken in Workfront Proof:

1. Open de proefdruk.
1. Klik het **drop-down menu van de Versie** in de upper-left hoek, dan klik **+ Nieuwe versie** in de doos die verschijnt.

   Op de **Nieuwe proefdrukversie van** pagina die verschijnt, kunt u alle recensenten van de vorige versie, met inbegrip van hun rollen en e-mailberichtmontages zien. U kunt de rollen en meldingen van bestaande revisoren eenvoudig bewerken of bestaande revisoren verwijderen uit de nieuwe versie op deze pagina.

1. Onder **voegt dossiers** toe, upload een dossier als nieuwe versie van de proef door te slepen en van uw computer te vallen of door **te klikken doorbladert** en het dossier te selecteren u wilt. U kunt de naam van het a **Bewijs** voor de versie typen of dit vakje leeg verlaten om zelfde filename met een versieaantal te gebruiken dat op het eind wordt toegevoegd.

   of

   Leg een webpagina vast als een nieuwe versie van de proefdruk door een URL te typen.

   >[!NOTE]
   >
   >Slepen en neerzetten is alleen beschikbaar in browsers die HTML5 volledig ondersteunen. Internet Explorer 7 tot en met 9 en Safari zijn hiervan uitgesloten.

1. Onder **Werkschema**, maak om het even welke volgende veranderingen om de recensenten voor deze versie van de proef te specificeren.

   Revisoren van de vorige versie worden vervangen door de revisoren die u toevoegt.

   * Verander de **Eigenaar** van de versie in een andere gebruiker in uw rekening.\
     Voor informatie over eigenaartoestemmingen, zie [ Profielen van de Toestemmingen van de Bewijs in Workfront Proof ](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

   * Gebruikend de **het contactnaam of e-mailadres van het Type om een ontvankelijke doos** toe te voegen, voeg recensenten aan de versie toe. U kunt de rol van het a **Bewijs** en een **E-mail alarm** type voor elke ontvanger specificeren.

     Voor informatie over het toevoegen van groepen aan de proef, zie  [ voegt Groepen aan een Bewijs ](../../../workfront-proof/wp-mnguserscontacts/groups/add-groups.md) toe. Voor informatie over rollen, zie [ de Rollen van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) leiden.

     >[!NOTE]
     >
     >Indien de maker of eigenaar van  de proef heeft [ het Bewijs E-mail van Made ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) gehandicapt door gebrek (in hun persoonlijke montages), zullen zij om het even welke Made van het Bewijs of Nieuwe proef e-mails niet ontvangen zelfs als de Notify mensen door e-mailvakje op de Nieuwe proefdrukpagina wordt gecontroleerd. Voor informatie over e-mailberichten, zie [ de montages van het e-mailbericht in Workfront Proof ](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md) vormen. Zie ook [ het Bewijs e-mail ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md) en [ Nieuwe proef e-mail ](../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md) maakte.

   * Stel een proefdrukdeadline in voor de versie.
   * Houd de muisaanwijzer boven de naam van een controleur om de beslissingen te zien die hij of zij in een vorige versie heeft genomen.

1. Onder **E-mail- bericht**, doe om het even welke volgend:

   * Geef op of u de controleurs op de hoogte wilt stellen van de nieuwe versie.\
     Uw selectie wordt aangemeld in het gedeelte Activiteit van de pagina Proefgegevens. Voor meer informatie, zie [ Beheren de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

   * Voeg een aangepast onderwerp en bericht toe.

1. In de **sectie van de Organisatie**, doe om het even welke volgend: 

   * Pas een of meer labels toe op de proefdruk. Voor meer informatie, zie [ Codes in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-and-manage-tags.md) creëren en beheren.\
     Tags worden ook overgeërfd van de vorige versie van de proefdruk. Als u een nieuwe tag toevoegt aan de nieuwe versie, worden vorige versies ook gecodeerd.

   * Voeg de versie toe aan een map. Zie [ Mappen in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md) voor meer informatie beheren. De map wordt gekopieerd uit de vorige versie van de proefdruk. Als u een andere map selecteert, wordt de hele proefdruk (alle versies) verplaatst.

   * Factureringsbeheerders en beheerders kunnen het mapveld verplicht maken voor de gehele account op het tabblad Instellingen. Zie voor meer informatie.

1. Breng onder Proefinstellingen een of meer van de onderstaande wijzigingen aan:

   * Aanmelding op de proefdruk vereisen
   * Elektronische handtekeningen op de proefdruk vereisen (alleen ondernemingsplan)
   * Het bewijs vergrendelen wanneer alle beslissingen worden genomen
   * Downloaden van oorspronkelijke bestand toestaan of blokkeren
   * Openbaar delen van de proefdruk, inclusief instellingen voor openbaar delen
   * Abonnement op het bewijs\
     De selecties die in deze sectie worden gemaakt, worden weergegeven op de pagina Proefgegevens (waar sommige velden kunnen worden bewerkt). Voor meer informatie, zie [ Beheren de Details van het Bewijs in Workfront Proof ](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

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

Als u een standaardonderwerp en een bericht hebt opgeslagen in uw persoonlijke instellingen, heeft dit invloed op welk bericht standaard wordt weergegeven op de pagina Nieuwe versie:

* Als u ervoor kiest om de controleurs via e-mail op de hoogte te stellen van de vorige versie van de proefdruk met de standaard-e-mail (bijvoorbeeld geen aangepast onderwerp/bericht), wordt uw standaard aangepaste onderwerp/bericht (uw persoonlijke instellingen) weergegeven op de pagina Nieuwe versie. U kunt het aangepaste onderwerp en het aangepaste bericht vervolgens bewerken of de selectie van Personen per e-mail op de hoogte stellen opheffen (er wordt dan geen e-mail verzonden naar uw revisoren om hen te laten weten dat ze een nieuwe versie hebben die moet worden gecontroleerd).
* Als u ervoor kiest om de controleurs geen e-mail te sturen voor de vorige versie van de proefdruk (bijvoorbeeld geen standaard- of aangepaste e-mail), bevat de pagina Nieuwe versie standaard geen bericht. Als u de controleurs op de hoogte wilt stellen van de nieuwe versie, klikt u op de koppeling Bericht verzenden. Deze koppeling geeft uw standaardaangepast onderwerp/bericht weer (volgens uw persoonlijke instellingen). Indien nodig kunt u het aangepaste onderwerp en het aangepaste bericht bewerken.

Als u geen standaardonderwerp en -bericht hebt opgeslagen in uw persoonlijke instellingen, wordt het volgende weergegeven op de pagina Nieuwe versie:

* Als u ervoor kiest om de controleurs via e-mail op de hoogte te stellen van de vorige versie van de proefdruk met de standaard-e-mail (bijvoorbeeld geen aangepast onderwerp/bericht), wordt de optie Personen per e-mail waarschuwen standaard geselecteerd op de pagina Nieuwe versie. Klik op de koppeling om een aangepast bericht toe te voegen.
* Als u ervoor kiest om de controleurs geen e-mail te sturen voor de vorige versie van de proefdruk (bijvoorbeeld geen standaard- of aangepaste e-mail), bevat de pagina Nieuwe versie standaard geen bericht. Als u de controleurs op de hoogte wilt stellen van de nieuwe versie, klikt u op de koppeling Bericht verzenden. Vervolgens kunt u een aangepast onderwerp en bericht toevoegen door op de koppeling Aangepast bericht toevoegen te klikken.
