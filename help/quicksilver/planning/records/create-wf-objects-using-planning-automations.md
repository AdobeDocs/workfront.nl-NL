---
title: Workfront-objecten maken met Adobe Workfront Planning Record Automations
description: U kunt automatiseringen in de Planning van Workfront vormen die, wanneer geactiveerd, tot voorwerpen in Workfront leiden.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 00e58ea9a207037b701e1be010c2c4c2995d60e0
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Objecten maken met Adobe Workfront Planning-recordautomatisering

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

U kunt automatiseringen in de Planning van Adobe Workfront vormen die, wanneer geactiveerd, tot voorwerpen in de Planning van Workfront of Workfront leiden.

U kunt de automatisering in de verslagpagina vormen en activeren. Het object dat wordt gemaakt, wordt verbonden met de planningsrecord en in het veld geplaatst dat u opgeeft in de automatisering.

U kunt bijvoorbeeld een automatisering maken die een Workfront-planningscampagne voert en een project maakt in Workfront om de voortgang van die campagne te volgen. Het project zou worden gekoppeld aan de planningscampagne van Workfront.

Voor meer informatie over verbonden verslagen, zie [ Verbonden verslagenoverzicht ](/help/quicksilver/planning/records/connected-records-overview.md).

## Toegangsvereisten

+++ Breid uit om toegangsvereisten voor de Planning van Workfront te bekijken.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Producten</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-abonnement*</p></td> 
   <td> 
<p>Een van de volgende Workfront-plannen:</p> 
<ul><li>Selecteren</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is niet beschikbaar voor oudere Workfront-plannen</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-planningspakket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Neem contact op met uw Workfront-accountmanager voor meer informatie over wat er in elk Workfront-planningsplan is opgenomen. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-platform</p></td> 
   <td> 
<p>Het geval van Workfront van uw organisatie moet aan de Adobe Verenigde Ervaring worden genegeerd om tot alle mogelijkheden van de Planning van Workfront te kunnen toegang hebben.</p> 
<p>Voor meer informatie, zie <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md"> Adobe Verenigde Ervaring voor Workfront </a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie*</p></td> 
   <td> Standaard
   <p>Workfront Planning is niet beschikbaar voor oudere Workfront-licenties</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p> 
   <p>Bewerk de toegang in Workfront voor de objecttypen die u wilt maken (projecten, portfolio's, programma's). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Rechten beheren in de werkruimte waaraan u records wilt toevoegen. </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (projecten) toe te voegen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Lay-outsjabloon</p></td> 
   <td> <p>Aan alle gebruikers, inclusief Workfront-beheerders, moet een lay-outsjabloon worden toegewezen die het planningsgebied in het hoofdmenu bevat </p> </td> 
  </tr> 
</tbody> 
</table>

*Voor meer informatie over de toegangsvereisten van Workfront, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Overwegingen bij het maken van objecten en records via een automatisering

* De nieuwe object- of recordnaam is gelijk aan de naam van de record waaruit u deze maakt.
* Als in de record waarvoor u de automatisering gebruikt, al objecten van hetzelfde type zijn verbonden in het veld dat u selecteert om nieuwe objecten toe te voegen, worden de nieuwe objecten toegevoegd aan het verbindingsveld en blijven bestaande objecten ook verbonden.

## Automatisering configureren in Workfront-planning

U moet een automatisering in de Planning van Workfront vormen alvorens u het kunt gebruiken om voorwerpen tot stand te brengen.

{{step1-to-planning}}

1. Klik op een recordtypekaart en klik vervolgens op de naam van een record.

   De pagina met recordtypen wordt geopend.
1. Klik **Meer** menu ![](assets/more-menu.png) aan het recht van de naam van het verslagtype, dan klik **leidt automatiseringen**.

   De lijst met beschikbare automatiseringen wordt geopend.

1. Klik **Nieuwe automatisering** in de hoger-juiste hoek van het scherm. Het **Nieuwe automatiserings** vakje opent.
1. Werk de volgende velden bij:

   * Vervang **Naamloze automatisering** met de tekst die u op de automatiseringsknoop wilt verschijnen. Gebruikers klikken op deze knop wanneer ze de automatisering gebruiken om een Workfront-object te maken.
   * **Beschrijving**: Voeg een beschrijving toe om het doel van de automatisering te identificeren.

1. Voor de detailspagina van de automatisering, werk de volgende gebieden in de **1} sectie van Trekkers bij {:**

   * **Trekker**: Selecteer de actie die de automatisering zal teweegbrengen. Bijvoorbeeld, uitgezochte **Knoop klikt**. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Werk de volgende gebieden in de **sectie van Acties** bij:
   * **Type van Objecten**: Selecteer het voorwerp dat u de automatisering wilt tot stand brengen. Dit is een verplicht veld.

     U kunt de volgende objecten maken van Workfront Planning-records:

      * Project
      * Portfolio
      * Programma
      * Groep
      * Opnemen
1. (Voorwaardelijk) Afhankelijk van het type object dat u wilt maken, werkt u de volgende velden bij:

   * **Project**:
      * **Verbonden gebied waar het voorwerp** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe project zal tonen. Dit is een verplicht veld
      * **Malplaatje waarvan om het project** tot stand te brengen: Selecteer een projectmalplaatje dat Workfront zal gebruiken om het project tot stand te brengen.
   * **Portfolio**:
      * **Verbonden gebied waar het voorwerp** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe portefeuille zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan bijlage aan de nieuwe portefeuille**: Selecteer een douaneformulier om aan de nieuwe portefeuille vast te maken. U moet een aangepast portfolioformulier maken voordat u het kunt selecteren.
   * **Programma**:
      * **Verbonden gebied waar het voorwerp** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe programma zal tonen. Dit is een verplicht veld.
      * **portefeuille van het Programma**: Selecteer een portefeuille waar het nieuwe programma zal worden toegevoegd. Dit is een verplicht veld.
      * 
         * **Vorm van de Douane aan het nieuwe programma** vast te maken: Selecteer een douanevorm om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **Groep**:
      * **Verbonden gebied waar het voorwerp** wordt gecreeerd: Dit is het verbonden gebied waar de nieuwe groep zal tonen. Dit is een verplicht veld.
      * **Vorm van de Douane aan de nieuwe groep** vast te maken: Selecteer een douaneformulier om aan het nieuwe programma vast te maken. U moet een aangepast programma maken voordat u het kunt selecteren.
   * **Verslag**:
      * **Verbonden verslagtype**: Selecteer het verslagtype u wilt tot stand brengen.
      * **Verbonden gebied waar het verslag** wordt gecreeerd: Dit is het verbonden gebied waar het nieuwe verslag zal tonen. Dit is een verplicht veld.
      * **gebied van de Kaart**: Selecteer gebieden van het verslagtype de automatisering voor wordt gecreeerd om hen aan de gebieden van het verbonden verslagtype in kaart te brengen.
      * **aan verbonden verslaggebied**: Selecteer gebieden van het verbonden verslag dat aan de gebieden van het verslagtype zal beantwoorden u de automatisering voor creeert.
1. (Facultatief en voorwaardelijk) als u geen verbindingsgebied voor een objecten van Workfront type hebt, klik **creeer een verbindingsgebied** pictogram ![](assets/create-a-connection-field-icon.png) om een gebied toe te voegen.
1. (Facultatief en voorwaardelijk) als u selecteerde om een verslag toe te voegen, **** op het **gebied van de Kaart** toevoegen en in kaart te brengen om extra gebieden toe te voegen, dan selecteren een gebied aan **Overdracht van** en een gebied aan **Overdracht aan** om te wijzen op welk gebied van het oorspronkelijk geselecteerde verslag op welk gebied van het verbonden verslag zou moeten tonen.
1. Klik **sparen**.

   De automatisering wordt weergegeven in de lijst met automatiseringen en is beschikbaar voor gebruik in records.
1. (Optioneel) Ga als volgt te werk om een automatisering te bewerken, uit te schakelen of te verwijderen:

   Van de lijst van automatiseringen, houd over de naam van een bewaarde automatisering, dan klik **Meer** menu ![](assets/more-menu.png), dan kies één van de volgende opties:

   * **geeft** uit: De informatie van de update over en vormt gebieden op de automatisering.
   * **maak** onbruikbaar: De automatisering zal niet als optie in de toolbar van de de lijstmening van verslagen tonen en de gebruikers kunnen het niet meer gebruiken om verslagen of voorwerpen tot stand te brengen. Om het opnieuw beschikbaar te maken, klik **Meer** menu ![](assets/more-menu.png) opnieuw, dan klik **activeert**.
   * **Schrapping**: De automatisering wordt geschrapt en kan niet worden teruggekregen. Records die zijn gemaakt met de automatisering, blijven verbonden met de oorspronkelijk geselecteerde record.

## Een Workfront-planningsautomatisering gebruiken om een object te maken

1. Open in Workfront Planning de pagina met recordtypen die de records bevat die u wilt gebruiken om Workfront-objecten te maken.
1. Open de tabelweergave.
1. Selecteer een of meer records.

   Onder aan de tabel wordt een blauwe balk weergegeven met extra knoppen, zoals automatiseringsknoppen.
1. Klik op de automatiseringsknop in de rechterbenedenhoek van het scherm.

   ![ knoop van de Automatisering ](assets/automation-custom-button.png)

   Het nieuwe object wordt weergegeven in het verbonden veld dat u hebt aangegeven in de instelling van de automatiseringsknop.

   >[!NOTE]
   >
   >We raden u aan te controleren of het object is gemaakt en verbonden zoals u had verwacht.

1. (Optioneel) Klik op het nieuwe object in het verbonden veld. De objectpagina wordt geopend en u kunt aanvullende wijzigingen in het nieuwe object aanbrengen.

<!--you might need to add something about notifications and emails?!-->
