---
title: Adobe Workfront-planningsautomatisering configureren
description: U kunt automatiseringen in de Planning van Adobe Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront of verslagen in de Planning van Workfront leiden. De gemaakte objecten en records worden automatisch verbonden met bestaande planningsrecords. In dit artikel wordt beschreven hoe u automatiseringen kunt beheren, zoals het bewerken, uitschakelen of verwijderen ervan.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Adobe Workfront-planningsautomatisering configureren

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

U kunt automatiseringen in de Planning van Adobe Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront of verslagen in de Planning van Workfront leiden wanneer teweeggebracht van een verslag van de Planning. De gemaakte objecten of records worden automatisch verbonden met de records waaruit u de automatisering activeert.

U kunt de automatisering in de verslagtype pagina in de Planning van Workfront vormen en activeren.

U kunt bijvoorbeeld een automatisering maken die een Workfront-planningscampagne voert en een project maakt in Workfront om de voortgang van die campagne te volgen.

In dit artikel wordt beschreven hoe u automatiseringen kunt beheren, zoals het bewerken, uitschakelen, verwijderen en activeren van objecten en records.

Voor informatie over hoe u verslagen of voorwerpen creeert gebruikend een bestaande automatisering, zie [ voorwerpen creëren gebruikend het verslag van de Planning van Adobe Workfront automatiseringen ](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Toegangsvereisten

+++ Breid uit om de toegangsvereisten voor de functionaliteit in dit artikel te bekijken. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Alle Workfront en alle planningspakketten</p> <p>Willekeurige workflow en planningspakket</p>
<p>Neem voor meer informatie over wat er in elk planningspakket voor Workfront staat, contact op met uw Workfront-accountvertegenwoordiger. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Beheer machtigingen voor de werkruimte en voor het recordtype waarin u automatiseringen wilt maken. </p>
   <p>Systeembeheerders hebben beheermachtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   </td> 
  </tr>  
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and to the record type where you want to create automations. </p>
   <p>System Administrators have Manage permissions to all workspaces, including the ones they did not create</p>
   </td> 
  </tr> 
</tbody> 
</table> -->

## Automatisering configureren in Workfront-planning

U moet een automatisering voor een verslagtype in de Planning van Workfront vormen alvorens u het kunt gebruiken om voorwerpen te creëren.

{{step1-to-planning}}

1. Klik op een recordtypekaart en klik vervolgens op de naam van een record.

   De pagina met recordtypen wordt geopend.
1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype, dan klik **leiden automatiseringen**.

   De lijst met beschikbare automatiseringen voor het geselecteerde recordtype wordt geopend.

1. Klik **Nieuwe automatisering** in de hoger-juiste hoek van het scherm. Het **Nieuwe automatiserings** vakje opent.
1. Werk de volgende velden bij:

   * Vervang **Naamloze automatisering** met de tekst die u op de automatiseringsknoop wilt verschijnen. Gebruikers klikken op deze knop wanneer ze de automatisering gebruiken om een Workfront-object of een planningsrecord te maken.
   * **Beschrijving**: Voeg een beschrijving toe om het doel van de automatisering te identificeren.
1. Klik **sparen**.
De pagina met gegevens over automatisering wordt geopend.

1. Voor de detailspagina van de automatisering, werk de volgende gebieden in de **1} sectie van Trekkers bij {:**

   * **Trekker**: Selecteer de actie die de automatisering zal teweegbrengen. Bijvoorbeeld, uitgezochte **Knoop klikt**. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Werk de volgende gebieden in de **sectie van Acties** bij: <!--submitted bugs for these fields - see if they need changing here-->
   * **Acties**: Selecteer de actie die u Workfront wilt uitvoeren wanneer het teweegbrengen van de automatisering. Dit is een verplicht veld.
Selecteer een van de volgende handelingen:

      * Meerdere projecten maken
      * Eén project maken
      * Project maken
      * Record maken
      * Programma maken
      * Portefeuille maken
      * Groep maken

     >[!TIP]
     >
     >Nadat u de automatisering hebt opgeslagen, kunt u de geselecteerde actie in dit veld niet meer wijzigen.

1. (Voorwaardelijk) Afhankelijk van de actie die u hebt geselecteerd, werkt u de volgende velden bij:

   * **creeer één enkel project**: <!--replace to the left: Create a single project-->
      * **Verbonden gebied waar het project** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe project zal tonen. Dit is een verplicht veld.
      * **malplaatje van het Project**: Selecteer een projectmalplaatje dat Workfront zal gebruiken om het project tot stand te brengen.

   * Meerdere projecten maken:
      * **Verbonden gebied waar het project** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe project zal tonen. Dit is een verplicht veld.
      * **Gebied de waarvan keuzen tot de verslagen** zullen leiden: Kies een multi- of enig-uitgezocht gebied van het geselecteerde verslagtype. Workfront maakt een project voor elke veldkeuze die momenteel is geselecteerd in de record waaruit de automatisering wordt geactiveerd.

     >[!TIP]
     >
     >Een project wordt gecreeerd slechts voor de opties die momenteel op het multi- of enig-uitgezochte gebied van het verslag worden geselecteerd u de automatisering van in werking stelt, en niet voor alle mogelijke keuzen voor dat gebied.
     >

      * **Gebruik het zelfde malplaatje**: Selecteer deze optie om het zelfde malplaatje voor elk nieuw project te gebruiken. Als de optie wordt geschrapt, selecteer a **malplaatje van het Project** voor elke gebiedskeuze.
      * **malplaatje van het Project**: Als u **het zelfde malplaatje** optie selecteerde, selecteer een projectmalplaatje dat Workfront zal gebruiken om de projecten tot stand te brengen.

   * **creeer portefeuille**:
      * **Verbonden gebied waar de portefeuille** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe portefeuille zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan bijlage aan de nieuwe portefeuille**: Selecteer een douaneformulier om aan de nieuwe portefeuille vast te maken. U moet een aangepast portfolioformulier maken voordat u het kunt selecteren.
   * **creeer programma**:
      * **Verbonden gebied waar het programma** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe programma zal tonen. Dit is een verplicht veld.
      * **portefeuille van het Programma**: Selecteer een portefeuille waar het nieuwe programma zal worden toegevoegd. Dit is een verplicht veld.
      * **Vorm van de Douane aan het nieuwe programma** vast te maken: Selecteer een douanevorm om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **creeer groep**:
      * **Verbonden gebied waar de groep** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe groep zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan de nieuwe groep** vast te maken: Selecteer een douaneformulier om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **creeer verslag**:
      * **Type van Verslag**: Selecteer het verslagtype u wilt tot stand brengen.

        De **sub-sectievertoningen van Montages**. Werk de volgende gebieden in de **sub-sectie van Montages** bij:

         * **Gebied op het verbonden verslagtype waar het huidige verslag** zal tonen: Dit is het verbonden gebied op het verslagtype dat voor de actie wordt geselecteerd waar het huidige verslag zal tonen.

        Als u bijvoorbeeld een automatisering maakt voor campagnes om productrecords met elkaar te verbinden, is dit het verbonden veld op het productrecordtype waarin de campagnes worden weergegeven, nadat de producten met de automatisering zijn gemaakt.

        Dit is een verplicht veld.

        <!--submitted a change in functionality and UI text for this - revise??-->
Op het **gebied van de Kaart**, werk de volgende informatie bij:

         * **Overdracht van**: Selecteer gebieden van het verslagtype de automatisering voor wordt gecreeerd om hen aan de gebieden van het verbonden verslagtype in kaart te brengen.
         * **Overdracht aan**: Selecteer gebieden van het pas gecreëerde verslag dat met informatie van het verslag zal bevolken u de automatisering van in werking stelt.

        >[!TIP]
        >
        >* De veldtypen van het oorspronkelijke recordtype moeten overeenkomen met de veldtypen van het nieuwe recordtype.
        >* Als u geen gebieden kiest, zullen de namen van de nieuwe verslagen **Naamloos verslag** zijn.

1. (Facultatief en voorwaardelijk) als u selecteerde om een verslag tot stand te brengen, **voegt gebieden** toe om extra raadplegingsgebieden van één verslag aan een andere in kaart te brengen.
1. (Voorwaardelijk) als er geen verbindingsgebieden tussen het originele verslagtype en het verslagtype zijn dat op het **wordt geselecteerd het type van Verslag** gebied, **klikken voegt verbonden gebied** toe.

   ![ opstelling van de Automatisering om een verslag ](assets/automation-setup-create-record.png) te creëren

   De volgende twee velden worden gemaakt:

   * Een nieuw verbindingsgebied genoemd **Verbonden verslag** wordt gecreeerd voor het verslagtype u op het **type van Verslag** gebied wees.
   * Een nieuw verbindingsgebied met de zelfde naam zoals die op het **wordt vermeld het type van het Verslag** gebied wordt gecreeerd voor het verslagtype u de automatisering voor vormt.

     Bijvoorbeeld, als u een automatisering voor Campagnes vormt om een ander verslagtype automatisch tot stand te brengen genoemd Banden en u **klikt voeg verbonden gebied** toe, worden de volgende gebieden gecreeerd:

      * Het **Verbonden verslag** verbindingsgebied wordt gecreeerd voor het **Merken** verslagtype.
      * Het **Merken** verbindingsgebied wordt gecreeerd voor het **3} verslagtype van Campagnes {.**

1. (Facultatief) als er geen verbindingsgebieden tussen het originele verslagtype en het voorwerp van Workfront dat op het gebied van Acties wordt geselecteerd zijn, klik **voeg verbonden gebied** toe.

   ![ opstelling van de Automatisering om veelvoudige projecten ](assets/automation-setup-create-multiple-projects.png) tot stand te brengen

   Het volgende wordt gemaakt:

   * Een nieuw verbindingsgebied genoemd **Verbonden &lt; naam van het voorwerp van Workfront >** wordt gecreeerd voor het verslagtype u de automatisering voor bouwt. Bijvoorbeeld, wordt het a **Verbonden project** gebied gecreeerd voor het verslagtype u de automatisering voor bouwt, wanneer u verkiest om projecten automatisch tot stand te brengen.
   * Er wordt een nieuwe recordtypekaart toegevoegd aan de sectie Planning van een Workfront-project, in Workfront met de naam van het recordtype waarvoor u de automatisering configureert.

1. Klik **sparen** in de hoger-juiste hoek van de pagina van de automatiseringsdetails.

   De automatisering wordt weergegeven in de lijst met automatiseringen en is beschikbaar voor gebruik in records.

## Bestaande automatisering beheren

{{step1-to-planning}}

1. Klik op een recordtypekaart en klik vervolgens op de naam van een record.

   De pagina met recordtypen wordt geopend.
1. Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) aan het recht van de naam van het verslagtype, dan klik **leiden automatiseringen**.

   De lijst met beschikbare automatiseringen voor het geselecteerde recordtype wordt geopend.

1. (Optioneel) Voer een van de volgende handelingen uit om een automatisering te bewerken, uit te schakelen of te verwijderen:

   1. Van de lijst van automatiseringen, houd over de naam van een bewaarde automatisering, dan klik **Meer** menu ![ Meer menu ](assets/more-menu.png).

   1. Klik **uitgeven** om de volgende informatie bij te werken:

      * Klik **Meer** menu ![ Meer menu ](assets/more-menu.png) rechts van de automatiseringsnaam, dan klik **uitgeven** om de naam van de automatisering te veranderen.
      * Om het even welke gebieden in de automatisering, behalve het **gebied van Acties**.

        >[!TIP]
        >
        >U kunt de oorspronkelijk geselecteerde actie voor een automatisering niet wijzigen.


   1. Klik **onbruikbaar maken** om de automatisering uit de de lijstmening van het verslag te verwijderen en gebruikers te verhinderen het te gebruiken om verslagen of voorwerpen tot stand te brengen.

      Records die zijn gemaakt met een uitgeschakelde automatisering, blijven verbonden met de oorspronkelijk geselecteerde record.

      Om het opnieuw beschikbaar te maken, klik **Meer** menu ![ ](assets/more-menu.png) opnieuw, dan klik **activeren**.
   1. Klik **Schrapping** om de automatisering te schrappen. Een verwijderde automatisering kan niet worden hersteld.

      Records die zijn gemaakt met een verwijderde automatisering, blijven verbonden met de oorspronkelijk geselecteerde record.
