---
title: Overzicht van projectgezondheid
content-type: reference
description: De functie Projectgezondheid gebruikt de kracht van AI Assistant om u direct een evaluatie te geven van de prestaties van uw projecten.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: dce36c38a626b4d3799fb1d1f673bdc49d81e274
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 0%

---

# Overzicht van projectgezondheid

>[!IMPORTANT]
>
>De functie Projectgezondheid is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase.

De functie Projectgezondheid van Adobe Workfront maakt gebruik van de kracht van AI Assistant om u direct een beoordeling te geven van de manier waarop uw projecten presteren, welke gebieden uw aandacht behoeven en hoe u problemen kunt vermijden die u tijd en geld kunnen kosten.

De Medewerker van AI kan een Beoordeling van de Gezondheid van het Project voor de volgende voorwerpen produceren:

* Eén project
* Eén enkel programma
* Meerdere projecten

Voor meer informatie over AI Medewerker, zie [&#x200B; AI Hulpoverzicht &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-pakket</p></td> 
   <td> 
<p>Selecteren of hoger </p> 
<p>Werkstroom selecteren of hoger</p>
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licentie</p></td> 
   <td> 
<p>Standard</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuraties op toegangsniveau</p></td> 
   <td><p>U moet een systeembeheerder zijn om de configuraties van de Gezondheid van het Project te beheren </p>
   <p>Toegang tot projecten bewerken om projectgezondheidsconfiguraties toe te passen </p>
     <p>Toegang tot projecten weergeven om de configuraties van Projectgezondheid weer te geven </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Inschrijven in de bètaversie van de projectgezondheid

Als u Projectgezondheid wilt gebruiken, moet uw organisatie AI Assistant hebben ingeschakeld.

Als u AI Assistant en Projectgezondheid voor uw organisatie wilt inschakelen, moet u het volgende toepassen:

* Uw organisatie moet zijn gemigreerd naar Adobe IMS (Identity Management System).
* Uw organisatie moet een Select-, Prime- of Ultimate Workfront-abonnement hebben
* De Adobe Unified Experience moet zijn ingeschakeld.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
* De Workfront-beheerder moet AI Assistant inschakelen voor gebruikers in uw organisatie. De Medewerker van AI wordt toegelaten door toegangsniveaus.
* U moet de opties AI inschakelen en Projectgezondheid inschakelen selecteren in de sectie AI-voorkeuren bij Instellen > Systeem > Voorkeuren.

  ![&#x200B; AI sectie van Voorkeur &#x200B;](assets/ai-preferences.png)

Voor meer informatie, zie [&#x200B; AI Hulpoverzicht &#x200B;](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md) en [&#x200B; vorm systeemvoorkeur &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Lijst met vragen voor AI Assistant

Hieronder vindt u een lijst met aanwijzingen die u kunt gebruiken om AI-evaluatie te vragen om een projectevaluatie te genereren voor een project, programma of alle projecten in uw account.

<table>
    <tr>
        <td><b>Locatie</b></td>
        <td><b>Vragen</b></td>
    </tr>
    <tr>
        <td>Een specifieke pagina met projectdetails</td>
        <td><em>Wat is de gezondheid van dit project?</em></td>
    </tr>
    <tr>
        <td>Elke pagina in Workfront </td>
        <td><em>Wat is de gezondheid van project [NAAM VAN PROJECT]?</em></td>
    </tr>
    <tr>
        <td>Elke pagina in Workfront </td>
        <td><em>Wat is de gezondheid van mijn projecten?</em></td>
    </tr>
       <tr>
        <td>Een pagina met specifieke programmagegevens</td>
        <td><em>Wat is de gezondheid van dit programma?</em></td>
    </tr>
       <tr>
        <td>Elke pagina in Workfront </td>
        <td><em>Wat is de gezondheid van programma [NAAM VAN PROGRAMMA]?</em></td>
    </tr>
   </table>


## Lijst van projecten en programma&#39;s

Hieronder ziet u de beschikbare voorwaarden die AI Assistant aan uw project of programma toewijst wanneer een projectevaluatie wordt gegenereerd.

<table>
    <tr>
        <td><b>Projectvoorwaarde</b></td>
        <td><b>Voortgang van project</b></td>
        <td><b>Projectvoorwaardelementen</b></td>
    </tr>
    <tr>
        <td>Op doel</td>
        <td>Deze analyse wordt toegepast wanneer het gemiddelde risiconiveau voor de volgende factoren binnen de gezonde drempel valt.
        </td>
        <td> 
        <ul><li>kneep</li>
        <li>Ontbrekende velden</li>
        <li>Wijzigingen plannen</li>
        <li>Onderschat werk</li>
        <li>Voortgang van project</li>
        <li>Achterstallige taken</li>
        <li>Begroting</li>
        </ul></td>
    </tr>
    <tr>
        <td>Risico</td>
        <td>Deze analyse wordt toegepast wanneer het gemiddelde risiconiveau voor de volgende factoren net onder de gezonde drempel daalt.</td>
        <td>
        <ul><li>kneep</li>
        <li>Ontbrekende velden</li>
        <li>Wijzigingen plannen</li>
        <li>Onderschat werk</li>
        <li>Voortgang van project</li>
        <li>Achterstallige taken</li>
        <li>Begroting</li>
        </ul></td>
    </tr>
    <tr>
        <td>In problemen</td>
        <td>Deze analyse wordt toegepast wanneer het gemiddelde risiconiveau voor de volgende factoren onder de gezonde drempel daalt.</td>
        <td>
        <ul><li>kneep</li>
        <li>Ontbrekende velden</li>
        <li>Wijzigingen plannen</li>
        <li>Onderschat werk</li>
        <li>Voortgang van project</li>
        <li>Achterstallige taken</li>
        <li>Begroting</li>
        </ul></td>
    </tr>
    </tr>
   </table>

## Projectgezondheidsconfiguraties beheren

Een configuratie van de projectgezondheid bevat specifieke criteria die bepalen hoe uw projectgezondheid wordt berekend. Nadat een configuratie wordt gecreeerd, kunt u het op een project dan toepassen.

>[!NOTE]
>
>U moet een Beheerder van het Systeem zijn om de configuraties van de Gezondheid van het Project te beheren.

{{step-1-to-setup}}

1. Klik **Voorkeur van het Project** in het linkerpaneel, dan uitgezochte **Gezondheid van het Project** in de drop-down die verschijnt.

1. In de hoger-juiste hoek van de pagina, uitgezochte **Nieuwe Configuratie**.

1. (Facultatief) op de pagina van configuratiedetails, vervang *Naamloze Configuratie* met een nieuwe configuratie **Naam**.

1. In **welke factoren u in de sectie van de projectgezondheid** zou willen omvatten, schrap om het even welke factor u inbegrepen niet wilt wanneer het bepalen van uw criteria van de projectgezondheid:
   * **kneep van het werkingsgebied**: Hoeveel het projectwerkingsgebied is uitgebreid sinds het begon.

   * **Vereiste gebieden**: Als om het even welke vereiste gebieden (b.v. projectbeschrijving) ontbreken. Deze vereiste gebieden bepalen projectvolledigheid en worden gespecificeerd in **Welke gebieden wilt u volledigheid controleren?** -configuratiesectie verderop.


   * **veranderingen van het Programma**: Hoeveel programmaveranderingen zijn voorgekomen sinds het begonnen project.

   * **Taakraming**: Hoe nauwkeurig is het taakwerk geschat (b.v. geen achterstallige taken momenteel in het project).

   * **Ingang van de Taak**: Hoe het projectwerk in vergelijking met de projectchronologie vordert.

   * **achterstallige taken**: Hoeveel taken zijn momenteel voorbij hun vervaldatum.

   * **Kosten**: Als het project momenteel over begroting is.

1. In **wanneer begint uw project officieel?** selecteert u in de vervolgkeuzelijst de gebeurtenis die het begin van het project aangeeft.

1. In **hoe schat u het werkingsgebied aan een project?** selecteert u welke projectfactor wordt verhoogd naarmate het projectbereik wordt vergroot.

1. In **welke gebieden wilt u volledigheid controleren?** selecteert u een of meer velden die worden gecontroleerd om de volledigheid van het project te bepalen.

   ![&#x200B; de volledigheidsgebieden van het Project &#x200B;](assets/project-completeness-fields.png)


1. Klik **sparen** in de hoger-juiste hoek.

## Projectgezondheidsconfiguraties toepassen

Zodra een beheerder een configuratie van de Gezondheid van het Project heeft gecreeerd, kunnen de gebruikers met Edit toegang het op een project toepassen.


{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. Klik het **Meer** pictogram ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de projectnaam, dan uitgezocht **geef** uit. Het **geeft het paneel van de Zijde van het Project** uit opent.

1. In het linkerpaneel, uitgezochte **Montages van het Project**.

1. Op het **gebied van de Configuratie van de Gezondheid van het 0&rbrace; Project, selecteer de configuratie u op dit project wilt toepassen.**

   ![&#x200B; gebied van de Configuratie van de Gezondheid van het Project &#x200B;](assets/project-health-configurations.png)

1. Klik **sparen** in de laag-linkerhoek van het paneel.

## Een projectevaluatie genereren voor een project of programma

Als u de toegang van de Mening voor een project of een programma hebt, kunt u zijn beoordeling van de Gezondheid van het Project produceren gebruikend AI medewerker.

Als u een beoordeling voor een project produceert, kan dit of van de projectpagina worden gedaan, of door de projectnaam van verwijzingen te voorzien wanneer u de medewerker vraagt hoe het project presteert.

Als u een beoordeling voor een programma produceert, kunt u dit van de pagina van de programmadetails doen.

>[!NOTE]
>
>Een beoordeling van de gezondheid van het Project kan niet voor een project worden geproduceerd tot het project is begonnen. U kunt vormen welke gebeurtenis een project teweegbrengt om in projectmontages te beginnen.

Voor meer informatie, zie de volgende sectie in dit artikel: [&#x200B; beheert de configuraties van de projectgezondheid &#x200B;](#manage-project-health-configurations).

1. Navigeer naar het project of het programma waarvoor u een beoordeling van de Gezondheid van het Project wilt produceren.

1. Voor de pagina van project/programmadetails, klik het **pictogram AI van de Medewerker** AI Medewerker pictogram ![&#x200B; in de hoger-juiste hoek van het scherm. &#x200B;](assets/ai-assistant-icon.png) AI Assistant wordt geopend.

1. Typ het volgende op **Vraag me over Workfront** gebied: *wat is de gezondheid van dit project?*

   of

   Typ het volgende op **Vraag me over Workfront** gebied: *wat is de gezondheid van dit programma?*

   >[!NOTE]
   >
   >Als u tot AI Medewerker van een verschillende pagina in Workfront toegang hebt, kunt u *typen wat de gezondheid van de NAAM van het project [ PROJECT ] is?* of *wat is de gezondheid van de NAAM van het programma [ PROGRAMMA ]?* <br>
   >Voor een volledige lijst van de huidige herinneringen kunt u ingaan, zie de volgende sectie in dit artikel: [&#x200B; AI Medewerker zet lijst &#x200B;](#ai-assistant-prompts-list) ertoe aan.

1. Hit **verzendt** pictogram ![&#x200B; verzendt pictogram &#x200B;](assets/send-icon.png). De projectevaluatie wordt gegenereerd en in het deelvenster weergegeven. Bovenaan elke projectevaluatie wordt een badge weergegeven die de huidige toestand van het project weerspiegelt.

   ![&#x200B; de gezondheidsbeoordeling van het Project &#x200B;](assets/health-assessment.png)

   Als u een beoordeling voor een portefeuille produceert, zullen de veelvoudige badges worden vermeld die de voorwaarde van elk project in het programma tonen. Voor meer informatie over de badgeetiketten, zie de volgende sectie in dit artikel: [&#x200B; lijst van de Project en van de programmavoorwaarden &#x200B;](#project-and-program-conditions-list).

1. (Optioneel) Klik op een van de evaluatiepunten om de details ervan uit te breiden.

1. (Optioneel) Klik in de modus Uitgebreide details op de taakkoppeling om de taakdetails te openen.

   ![&#x200B; Uitgebreide details &#x200B;](assets/expanded-details.png)

1. Na het herzien van de details van de projectgezondheid, klik het **Dichte** pictogram ![&#x200B; Dichte pictogram &#x200B;](assets/close-icon.png) in de hoger-juiste hoek van AI Medewerker.

## Een projectevaluatie genereren voor meerdere projecten

U kunt een gecombineerde beoordeling van de Gezondheid van het Project voor alle projecten produceren u momenteel de toegang van de Mening (of hoger) voor hebt.

Een project wordt alleen opgenomen in de gecombineerde projectevaluatie als het project is gestart. U kunt vormen welke gebeurtenis een project teweegbrengt om in projectmontages te beginnen. Voor meer informatie, zie de volgende sectie in dit artikel: [&#x200B; beheert de configuraties van de projectgezondheid &#x200B;](#manage-project-health-configurations).

1. Klik het **pictogram AI van de Medewerker** AI Hulppictogram ![&#x200B; in de hoger-juiste hoek van het scherm. &#x200B;](assets/ai-assistant-icon.png) AI Assistant wordt geopend.

1. Typ het volgende in het **vraagt me over het gebied van Workfront**: *wat is de gezondheid van mijn projecten?*

   Voor een volledige lijst van de huidige herinneringen kunt u ingaan, zie de volgende sectie in dit artikel: [&#x200B; AI Medewerker zet lijst &#x200B;](#ai-assistant-prompts-list) ertoe aan.

1. Hit **verzendt** pictogram ![&#x200B; verzendt pictogram &#x200B;](assets/send-icon.png). De projectevaluatie wordt gegenereerd en in het deelvenster weergegeven.

   ![&#x200B; Veelvoudige projectevaluatie &#x200B;](assets/multiple-projects-assessment.png)

   Wanneer het produceren van een beoordeling voor veelvoudige projecten, AI Medewerker groepeert de resultaten die op hoe de projecten momenteel presteren worden gebaseerd.

1. (Optioneel) Klik op een van de badges voor de gezondheidsvoorwaarde van het project om de projectlijst uit te breiden en selecteer vervolgens een koppeling voor een specifiek project om naar de detailpagina van dat project te gaan.

1. Na het herzien van de de gezondheidsdetails van projecten, klik het **dichte pictogram** dicht pictogram ![&#x200B; in de hoger-juiste hoek van AI Medewerker om het te sluiten.](assets/close-icon.png)

<!--

## Build a Project Health table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md). 

You can add a table report to a Canvas Dashboard in order to easily visualize your Project Health data in a table format.  

### Prerequisites 

You must create a dashboard before you can build a table report. 

For more, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

### Build a Project Health table report 

There are many configuration options available for building a Project Health table report. In this section, we'll walk you through the process of creating one that displays the following columns: 

* **Name**: Contains the project name. 
* **Project Health Analysis**: Contains a summary of the Project Health assessment. 
* **Project Health Created At**: Contains the date/time when the Project Health assessment was last generated. 
* **Project Health Label**: Contains the project's label (e.g. On Target, At Risk, or In Trouble).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. In the upper-right corner, click **New Dashboard**. 
1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**. 
1. Click **Create**. 
1. In the **Add report** box, select **Create report**. 
1. On the left side, select **Table**. 
1. In the upper-right corner, click **Create report**. 
1. (Optional) Follow the steps below to configure the **Details** ![Details icon](assets/details-icon.png) section: 
    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
1. Follow the steps below to configure the **Build table** ![Build table icon](assets/drilldown-column.png) section: 
    1. In the left panel, click the **Table columns** icon. 
    1. Click **Add column**, then select **Project** > **Name**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Analysis**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Created At**. 
    1. Click **Add column**, then select **Project** > **Project Health** > **Health Label**. 

1. Follow the steps below to configure the **Filter** ![Filter icon](assets/filter-icon.png) section: 
    1. In the left panel, click the **Filter** icon. 
    1. Select **Edit filter**. 
    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.
    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** ![Group settings](assets/drilldown-group-icon.png) section: 
    1. In the left panel, click the **Group Settings** icon. 
    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report.

-->
