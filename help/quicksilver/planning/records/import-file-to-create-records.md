---
title: Records maken door gegevens uit een CSV- of Excel-bestand te importeren
description: Records zijn afzonderlijke instanties van recordtypen. Dit zijn de objecttypen van Adobe Workfront Planning. In de Planning van Workfront, kunt u verslagen tot stand brengen door informatie van een CSV of dossier van Excel in te voeren.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---


# Records maken door gegevens te importeren uit een CSV- of Excel-bestand

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Records zijn afzonderlijke instanties van recordtypen. Dit zijn de objecttypen van Adobe Workfront Planning. In de Planning van Workfront, kunt u verslagen tot stand brengen door informatie van een CSV of dossier van Excel in te voeren.

Voor meer informatie over het creëren van verslagen, zie [&#x200B; verslagen &#x200B;](/help/quicksilver/planning/records/create-records.md) creëren.

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
   <td> <p>Draag of hoger toestemmingen aan de werkruimte bij en verslagtype waar u verslagen invoert. </p>
   <p>Systeembeheerders hebben machtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt</p>
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
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Overwegingen bij het importeren van records met een Excel- of CSV-bestand

* De kolomkoppen in elk blad worden de velden die zijn gekoppeld aan records.
* Elke rij in elk blad wordt een unieke record.
* Als het Excel-bestand meer dan één blad bevat, wordt alleen de informatie uit één blad geïmporteerd die u tijdens het importeren selecteert.
* Het bestand mag het volgende niet overschrijden:
   * 25.000 rijen
   * 500 kolommen
* Het bestand mag niet groter zijn dan 5 MB.
* Lege bladen worden niet ondersteund.
* Velden van de volgende typen worden niet ondersteund en kunnen niet worden toegewezen aan velden op het importblad:

   * Verbind gebieden met Workfront en AEM Assets objecten types. U kunt slechts verbindingsgebieden aan de types van het Verslag van de Planning in kaart brengen.
   * Velden opzoeken van verbonden planningsrecords of Workfront- en AEM Assets-objecten
   * Formuliervelden
   * Gemaakt op
   * Laatst gewijzigd op
   * Goedgekeurd op
   * Mensen
   * Als een multi- of single-select gebied wordt ingevoerd en het meer keuzen dan een gelijkaardig gebied in Planning heeft, worden de extra opties gecreeerd tijdens de invoer. Alleen gebruikers met de machtiging Beheren in de werkruimte kunnen nieuwe keuzen importeren.

## Records maken door een CSV- of Excel-bestand te importeren

{{step1-to-planning}}

1. Klik op de werkruimte waar u records wilt maken.

   of

   Vouw in een werkruimte de pijl omlaag naar rechts uit, zoek naar een werkruimte en selecteer deze wanneer de werkruimte in de lijst wordt weergegeven.
1. Klik op de kaart van het recordtype waar u de records wilt importeren.
1. Klik **Nieuw verslag** in de hoger-juiste hoek van het scherm.

   ![&#x200B; kies manier om verslagen drie knoopdoos toe te voegen &#x200B;](assets/choose-way-to-add-records-three-button-box.png)
1. Klik **uploaden van dossier**, dan **verdergaan**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Sleep en laat vallen een Excel of Csv- dossier eerder op uw computer, of klik **Uitgezocht een Csv of dossier van Excel** om voor te doorbladeren.
1. Klik **Voorproef en geef uit**.
1. (Voorwaardelijk) als het ingevoerde dossier meer dan één blad heeft, selecteer het radioknoop van het blad u in **wilt invoeren Selecteer een blad om** doos in te voeren, dan klik **daarna**. Anders gaat u door met de volgende stap.

   ![&#x200B; selecteer een blad om verslagen in te voeren &#x200B;](assets/select-a-sheet-to-import-box.png)
1. In de **Kaart de gebieden van de Planning aan uw kolomkopballen** selecteren het **Geplande gebied** dat het best de informatie in elk van de kolommen van het blad aanpast.

   ![&#x200B; Kaart de gebieden van de Planning aan kolommen wanneer het invoeren van verslagen &#x200B;](assets/map-planning-fields-to-columns-when-importing-records.png)

   Elke rij vertegenwoordigt een nieuwe record. Alleen de eerste 10 records worden weergegeven in het vak Voorbeeld en bewerken.

   >[!TIP]
   >
   >Niet alle veldtypen worden ondersteund. Voor meer informatie, zie de sectie [&#x200B; Overwegingen over het invoeren van verslagen gebruikend een Excel of Csv- dossier &#x200B;](#considerations-about-importing-records-using-an-excel-or-csv-file) in dit artikel.


1. (Facultatief en voorwaardelijk) als u hebt leiden toestemmingen aan de werkruimte, **creeer ontbrekende opties** in de laag-linkerhoek van het scherm. Als deze optie is ingeschakeld, worden de ontbrekende keuzen van velden met één of meerdere selecties toegevoegd.

   >[!NOTE]
   >
   >Als het geselecteerde recordtype bijvoorbeeld een enkel-geselecteerd statusveld met de opties Nieuw, Bezig en Gesloten heeft en een statusveld dat uit een bestand is geïmporteerd, ook de statuskeuze Status In wachtstand heeft, wordt de statuskeuze in de wachtstand ook toegevoegd.
   >
   >Als u geen beheermachtigingen hebt voor de werkruimte, kunt u records importeren, maar worden de extra opties niet gemaakt. In plaats daarvan, ontvangt u het volgende bericht in de hoger-juiste hoek van de Kaart de gebieden van de Planning aan uw doos van kolomkopballen: **de keuzen die niet in verbinding bestaan, zullen enig- of multi-uitgezochte gebieden niet worden toegevoegd**.

1. Klik **Invoer**.

   De volgende informatie wordt geïmporteerd in Workfront Planning:

   * Nieuwe records die onder aan de tabelweergave van het geselecteerde recordtype worden weergegeven.
   * Nieuwe veldwaarden voor bestaande velden die aan elke record zijn gekoppeld.
   * Nieuwe keuzen van een multi- of enig-uitgezocht gebied dat niet in Planning bestond.  <!--when we add connected records - add those here too-->

   U kunt velden en records beheren op de pagina met recordtypen.

   Iedereen met toegang tot de Planning van Workfront en de werkruimte kan nu de ingevoerde verslagen en hun informatie bekijken en uitgeven.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
