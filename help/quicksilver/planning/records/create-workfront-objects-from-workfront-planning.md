---
title: Workfront-objecten maken vanuit Workfront Planning wanneer u deze verbindt met records
description: U kunt Workfront-objecttypen maken terwijl u deze verbindt vanuit andere records in Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1257'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Workfront-objecten maken vanuit Workfront Planning wanneer u deze verbindt met records

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

U kunt op de volgende manieren Adobe Workfront-objecten maken via Workfront Planning:

* Als u Workfront-objecten verbindt met planningsrecords

  In dit artikel wordt beschreven hoe u Workfront-objecten kunt maken via Workfront Planning terwijl u deze verbindt vanuit planningsrecords.
* Wanneer u automatisering vanaf de pagina van een record gebruikt.

  Voor informatie over het creëren van de voorwerpen van Workfront die automatiseringen gebruiken, zie [&#x200B; voorwerpen creëren gebruikend Adobe Workfront de verslagautomatiseringen van de Planning van &#x200B;](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>U kunt de volgende voorwerpen van Workfront van de Planning van Workfront tot stand brengen wanneer u hen met de verslagen van de Planning verbindt:
>
>* Projecten
>* Portfolio&#39;s
>* Programma&#39;s
>
>U kunt de volgende Workfront-objecten verbinden met planningsrecords, maar u kunt ze niet maken tijdens het verbindingsproces:
>
>* Groepen
>* Bedrijven
>

Houd rekening met het volgende wanneer u Workfront-objecten verbindt en maakt met Workfront Planning-records:

* U kunt Workfront-projecten, -portfolio&#39;s, -programma&#39;s, -groepen en -bedrijven verbinden vanuit een verbindingsveld vanuit de volgende Workfront-planningsgebieden:

   * De tabelweergave van een recordtype
   * De pagina Details of het voorvertoningsvak van een record
   * Het tabblad Verbindingen van een record

* U kunt projecten van de volgende gebieden van de Planning van Workfront tot stand brengen:

   * De tabelweergave van een recordtype
   * Het gebied Details van een record in het verbindingsveld
   * De verbonden verslagpagina van een verslag

* U kunt portfolio&#39;s en programma&#39;s maken op basis van de volgende gebieden van Workfront Planning:

   * De tabelweergave van een recordtype
   * Het gebied Details van een record in het verbindingsveld

Voor informatie over het verbinden van verslagen van de Planning met de voorwerpen van Workfront, zie [&#x200B; verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

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
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuratie op toegangsniveau</p></td> 
   <td> <p>Er zijn geen toegangsniveaucontroles voor de Planning van Adobe Workfront</p> 
   <p>Bewerk de toegang tot Create-objecten in Workfront voor de objecttypen die u wilt maken (projecten, portfolio's, programma's). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objectmachtigingen</p></td> 
   <td> <p>Draag of hogere toestemmingen aan de werkruimte bij en verslagtype waar u verslagen wilt toevoegen. </p>  
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
   <p>Rechten voor Workfront-objecten (portfolio's) beheren om onderliggende objecten (projecten) toe te voegen.</p>
   </td> 
  </tr>   
</tbody> 
</table>

Voor meer informatie over de toegangsvereisten van Workfront, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## Vereisten voor het maken van Workfront-objecten wanneer deze worden verbonden met records uit Workfront Planning

U moet het volgende hebben alvorens u nieuwe projecten of portefeuilles kunt toevoegen door hen van bestaande verslagen te verbinden:

* Recordtypen die zijn verbonden met Workfront-projecten, -portfolio&#39;s of -programma&#39;s. Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).
* Records voor de recordtypen die zijn verbonden met Workfront-objecten. Voor informatie, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.
* De correcte toegang en de toestemmingen in de Planning van Workfront en Workfront, zoals die in de sectie [&#x200B; vereisten van de Toegang &#x200B;](#access-requirements) in dit artikel worden beschreven.

## Projecten maken terwijl u ze verbindt met records van Workfront Planning

U kunt projecten tot stand brengen aangezien u hen met verslagen in de Planning van Workfront op de volgende gebieden van de Planning van Workfront verbindt:

* De tabelweergave van een recordtype of het gebied Details van een record in het verbindingsveld
* De verbonden verslagpagina van een verslag, in het gebied van Details van een verslag

### Projecten maken in het gebied Details van een record of in de tabelweergave van een recordtype

Om projecten tot stand te brengen aangezien u hen van andere verslagen verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de projecten van Workfront aan te sluiten, zoals die in artikel [&#x200B; worden beschreven verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. (Voorwaardelijk) klik **toevoegen project**
of
Begin de naam van een project te typen, dan klik **voegt project** toe als u het niet kunt vinden. De Add knoop wordt gevolgd door de projectnaam u typte.

   ![&#x200B; voeg project toe wanneer het verbinden van het van een verbindingsgebied &#x200B;](assets/add-project-when-connecting-it-from-connection-field.png)

   **creeer project** doos opent.

1. (Facultatief) werk de **naam van het Project** bij. Standaard krijgt het project de naam van wat u als zoekopdracht hebt toegevoegd wanneer u het project verbindt vanuit de record.
1. (Facultatief) selecteer a **malplaatje van het Project**. Als u geen sjabloon selecteert, maakt Workfront een leeg project zonder taken.
1. Klik **creëren**.
1. (Voorwaardelijk) als u selecteerde om een project van een malplaatje tot stand te brengen, volg de stappen in het artikel [&#x200B; een project tot stand brengen gebruikend een malplaatje &#x200B;](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) artikel om het project te beëindigen toevoegend.

   Het nieuwe project wordt gecreeerd en aan het verbonden gebied van het geselecteerde verslag toegevoegd.

1. (Optioneel) Klik op de naam van het nieuwe project in Workfront Planning om de projectpagina in Workfront te openen en aanvullende updates voor het project uit te voeren.

### Projecten maken van de verbonden recordpagina van een record

1. Sluit het objecttype Project aan op een recordtype voor Workfront Planning in de tabelweergave.

   Voor informatie, zie [&#x200B; verbind verslagtypes &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klik in een weergave op de naam van een record. Het voorvertoningsvak Details wordt geopend.

1. Voeg a **Verbonden verslagenpagina** voor projecten toe.

   Voor informatie, zie [&#x200B; een Verbonden verslagenpagina aan een verslag &#x200B;](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) toevoegen.

   De pagina Verbonden records wordt weergegeven in de tabelweergave. Verbonden projecten worden in de tabel weergegeven.

   ![&#x200B; de lijstmening van Projecten in verbonden verslagenpagina &#x200B;](assets/projects-connected-records-page-table.png)

1. Klik **Nieuwe rij** in de projectenlijst om een project toe te voegen.

   U kunt alleen een leeg project in dit gebied toevoegen. U kunt geen project toevoegen gebruikend een malplaatje.
1. (Optioneel) Klik op de naam van het project in de tabelweergave om het project te openen in Workfront en meer informatie toe te voegen.

## Portefeuilles tot stand brengen aangezien u hen met verslagen van de Planning van Workfront verbindt

U kunt portfolio&#39;s maken vanuit de tabelweergave van een recordtype of de pagina Details van een record.

Om portefeuilles tot stand te brengen aangezien u hen van de verslagen van de Planning verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [&#x200B; worden beschreven verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. (Voorwaardelijk) klik **toevoegen portefeuille**

   of

   Begin de naam van een portefeuille te typen, dan klik **toevoegen portefeuille** als u het niet kunt vinden. De knop Toevoegen wordt gevolgd door de naam van het portfolio die u hebt opgegeven.

   ![&#x200B; voeg portefeuille toe wanneer het verbinden van het van een verbindingsgebied &#x200B;](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Het portfolio wordt gemaakt en toegevoegd aan het verbindingsveld van de record die u hebt geselecteerd.

1. (Optioneel) Klik op de naam van het nieuwe portfolio van Workfront Planning om de pagina van het portfolio te openen in Workfront en aanvullende updates voor het portfolio uit te voeren.

## Programma&#39;s maken terwijl u deze verbindt met records van Workfront Planning

U kunt programma&#39;s van de lijstmening van een verslagtype of de pagina van Details van een verslag tot stand brengen.

Om programma&#39;s tot stand te brengen aangezien u hen van de verslagen van de Planning verbindt:

1. Ga naar de detailspagina van een verslag of naar de lijst van het verslagtype en begin de verslagen van de Planning van Workfront met de portefeuilles van Workfront aan te sluiten, zoals die in het artikel [&#x200B; worden beschreven verbindt verslagen &#x200B;](/help/quicksilver/planning/records/connect-records.md).

1. Klik **toevoegen programma**

   of

   Begin de naam van een programma te typen, dan klik **programma** toevoegen als u het niet kunt vinden. De Add knoop wordt gevolgd door de programmanaam u typt.

   ![&#x200B; voeg het programma van Workfront toe wanneer het verbinden van het verbindingsgebied &#x200B;](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Het **Create programma** vakje opent.

1. Werk de **naam van het Programma** bij. Dit is een verplicht veld.
1. Kies a **Portfolio** van drop-down, of begin de naam van een portefeuille te typen, dan het te selecteren wanneer het in de lijst toont. Dit is een verplicht veld.
1. Klik **creëren**.

   Het programma wordt gemaakt en toegevoegd aan het verbindingsveld van de geselecteerde record.

1. (Optioneel) Klik op de naam van het nieuwe programma in Workfront Planning om de pagina van het programma in Workfront te openen en aanvullende updates voor het programma uit te voeren.

