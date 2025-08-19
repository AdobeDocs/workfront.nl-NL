---
title: Overzicht van projectgezondheid
content-type: reference
description: De functie Projectgezondheid gebruikt de kracht van AI Assistant om u direct een evaluatie te geven van de prestaties van uw projecten.
author: Jenny
feature: Get Started with Workfront
exl-id: e4d200c6-7f35-4919-96d3-2880a655ed62
source-git-commit: 2024f19709f7859ed6f19b830321d9e4c09e71f8
workflow-type: tm+mt
source-wordcount: '1822'
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

Voor meer informatie over AI Medewerker, zie [ AI Hulpoverzicht ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

+++ Vouw uit om de vereisten voor toegang weer te geven. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-plan</p></td> 
   <td> 
<p>Selecteren, Prime of Ultimate </p> 
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
   <td><p>Beheerder voor het beheren van configuraties in de projectgezondheid </p>
   <p>Bewerken om projectgezondheidsconfiguraties toe te passen </p>
     <p>Weergeven om de configuraties van Projectgezondheid weer te geven </p>
  </td> 
  </tr>  
    </tr>  
</tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Inschrijven in de bètaversie van de projectgezondheid

Als u Projectgezondheid wilt gebruiken, moet uw organisatie AI Assistant hebben ingeschakeld.

Als u AI Assistant wilt inschakelen voor uw organisatie, moet u het volgende toepassen:

* Uw organisatie moet zijn gemigreerd naar Adobe IMS (Identity Management System).
* De Adobe Unified Experience moet zijn ingeschakeld.
* Adobe moet een ondertekende Adobe Gen AI-overeenkomst in het bestand hebben.
* De Workfront-beheerder moet AI Assistant inschakelen voor gebruikers in uw organisatie. De Medewerker van AI wordt toegelaten door toegangsniveaus.

Voor meer informatie, zie [ AI Hulpoverzicht ](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

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
    </tr>
    <tr>
        <td>Op doel</td>
        <td>Wanneer de de Voortgangsstatus van het project op Tijd is, is de projectvoorwaarde op Doel.</td>
    </tr>
    <tr>
        <td>Risico</td>
        <td>Wanneer de de Voortgangsstatus van het project achter of op Risico is, is de projectvoorwaarde Op Risico.</td>
    </tr>
    <tr>
        <td>In problemen</td>
        <td>Wanneer de de Voortgangsstatus van het project te laat is, is de projectvoorwaarde Op Risico.</td>
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

1. (Facultatief) op de pagina van configuratiedetails, vervang *Naamloze Configuratie* met een nieuwe a configuratie **Naam**.

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

   ![ de volledigheidsgebieden van het Project ](assets/project-completeness-fields.png)


1. Klik **sparen** in de hoger-juiste hoek.

## Projectgezondheidsconfiguraties toepassen

Zodra een beheerder een configuratie van de Gezondheid van het Project heeft gecreeerd, kunnen de gebruikers met Edit toegang het op een project toepassen.


{{step1-to-projects}}

1. Voor de **pagina van Projecten**, selecteer een project.

1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png) aan het recht van de projectnaam, dan uitgezocht **geef** uit. Het **geeft het paneel van de Zijde van het Project** uit opent.

1. In het linkerpaneel, uitgezochte **Montages van het Project**.

1. Op het **gebied van de Configuratie van de Gezondheid van het 0} Project, selecteer de configuratie u op dit project wilt toepassen.**

   ![ gebied van de Configuratie van de Gezondheid van het Project ](assets/project-health-configurations.png)

1. Klik **sparen** in de laag-linkerhoek van het paneel.

## Een projectevaluatie genereren voor een project of programma

Als u de toegang van de Mening voor een project of een programma hebt, kunt u zijn beoordeling van de Gezondheid van het Project produceren gebruikend AI medewerker.

Als u een beoordeling voor een project produceert, kan dit of van de projectpagina worden gedaan, of door de projectnaam van verwijzingen te voorzien wanneer u de medewerker vraagt hoe het project presteert.

Als u een beoordeling voor een programma produceert, kunt u dit van de pagina van de programmadetails doen.

>[!NOTE]
>
>Een beoordeling van de gezondheid van het Project kan niet voor een project worden geproduceerd tot het project is begonnen. U kunt vormen welke gebeurtenis een project teweegbrengt om in projectmontages te beginnen.

Voor meer informatie, zie de volgende sectie in dit artikel: [ beheert de configuraties van de projectgezondheid ](#manage-project-health-configurations).

1. Navigeer naar het project of het programma waarvoor u een beoordeling van de Gezondheid van het Project wilt produceren.

1. Voor de pagina van project/programmadetails, klik het **pictogram AI van de Medewerker** AI Medewerker pictogram ![ in de hoger-juiste hoek van het scherm. ](assets/ai-assistant-icon.png) AI Assistant wordt geopend.

1. Typ het volgende op **Vraag me over Workfront** gebied: *wat is de gezondheid van dit project?*

   of

   Typ het volgende op **Vraag me over Workfront** gebied: *wat is de gezondheid van dit programma?*

   >[!NOTE]
   >
   >Als u tot AI Medewerker van een verschillende pagina in Workfront toegang hebt, kunt u *typen wat de gezondheid van de NAAM van het project [ PROJECT ] is?* of *wat is de gezondheid van de NAAM van het programma [ PROGRAMMA ]?* <br>
   >Voor een volledige lijst van de huidige herinneringen kunt u ingaan, zie de volgende sectie in dit artikel: [ AI Medewerker zet lijst ](#ai-assistant-prompts-list) ertoe aan.

1. Hit **verzendt** pictogram ![ verzendt pictogram ](assets/send-icon.png). De projectevaluatie wordt gegenereerd en in het deelvenster weergegeven. Bovenaan elke projectevaluatie wordt een badge weergegeven die de huidige toestand van het project weerspiegelt.

   ![ de gezondheidsbeoordeling van het Project ](assets/health-assessment.png)

   Als u een beoordeling voor een portefeuille produceert, zullen de veelvoudige badges worden vermeld die de voorwaarde van elk project in het programma tonen. Voor meer informatie over de badgeetiketten, zie de volgende sectie in dit artikel: [ lijst van de Project en van de programmavoorwaarden ](#project-and-program-conditions-list).

1. (Optioneel) Klik op een van de evaluatiepunten om de details ervan uit te breiden.

1. (Optioneel) Klik in de modus Uitgebreide details op de taakkoppeling om de taakdetails te openen.

   ![ Uitgebreide details ](assets/expanded-details.png)

1. Na het herzien van de details van de projectgezondheid, klik het **Dichte** pictogram ![ Dichte pictogram ](assets/close-icon.png) in de hoger-juiste hoek van AI Medewerker.

## Een projectevaluatie genereren voor meerdere projecten

U kunt een gecombineerde beoordeling van de Gezondheid van het Project voor alle projecten produceren u momenteel de toegang van de Mening (of hoger) voor hebt.

Een project wordt alleen opgenomen in de gecombineerde projectevaluatie als het project is gestart. U kunt vormen welke gebeurtenis een project teweegbrengt om in projectmontages te beginnen. Voor meer informatie, zie de volgende sectie in dit artikel: [ beheert de configuraties van de projectgezondheid ](#manage-project-health-configurations).

1. Klik het **pictogram AI van de Medewerker** AI Hulppictogram ![ in de hoger-juiste hoek van het scherm. ](assets/ai-assistant-icon.png) AI Assistant wordt geopend.

1. Typ het volgende in het **vraagt me over het gebied van Workfront**: *wat is de gezondheid van mijn projecten?*

   Voor een volledige lijst van de huidige herinneringen kunt u ingaan, zie de volgende sectie in dit artikel: [ AI Medewerker zet lijst ](#ai-assistant-prompts-list) ertoe aan.

1. Hit **verzendt** pictogram ![ verzendt pictogram ](assets/send-icon.png). De projectevaluatie wordt gegenereerd en in het deelvenster weergegeven.

   ![ Veelvoudige projectevaluatie ](assets/multiple-projects-assessment.png)

   Wanneer het produceren van een beoordeling voor veelvoudige projecten, AI Medewerker groepeert de resultaten die op hoe de projecten momenteel presteren worden gebaseerd.

1. (Optioneel) Klik op een van de badges voor de gezondheidsvoorwaarde van het project om de projectlijst uit te breiden en selecteer vervolgens een koppeling voor een specifiek project om naar de detailpagina van dat project te gaan.

1. Na het herzien van de de gezondheidsdetails van projecten, klik het **dichte pictogram** dicht pictogram ![ in de hoger-juiste hoek van AI Medewerker om het te sluiten.](assets/close-icon.png)


## Een rapport met een projectgezondheidstabel maken op een Canvasdashboard

>[!IMPORTANT]
>
>De functie Canvasdashboards is momenteel alleen beschikbaar voor gebruikers die deelnemen aan de bètafase. Voor meer informatie, zie {de bètainformatie van de Dashboards van het 0} Canvas [.](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)

U kunt een lijstrapport aan een Dashboard van het Canvas toevoegen om uw gegevens van de Gezondheid van het Project in een lijstformaat gemakkelijk te visualiseren.

### Vereisten

U moet een dashboard tot stand brengen alvorens u een lijstrapport kunt bouwen.

Voor meer, zie [ een Dashboard van het Canvas ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md) creëren.

### Een rapport met een projectgezondheidstabel samenstellen

Er zijn vele configuratieopties beschikbaar voor de bouw van een de lijstrapport van de Gezondheid van het Project. In deze sectie, zullen wij u door het proces lopen om één tot stand te brengen die de volgende kolommen toont:

* **Naam**: Bevat de projectnaam.
* **Analyse van de Gezondheid van het Project**: Bevat een samenvatting van de beoordeling van de Gezondheid van het Project.
* **Gezondheid van het Project creeerde bij**: Bevat de datum/de tijd toen de beoordeling van de Gezondheid van het Project het laatst werd geproduceerd.
* **Etiket van de Gezondheid van het Project**: Bevat het etiket van het project (b.v. Op streefwaarde, Risico, of in problemen).

{{step1-to-dashboards}}

1. In het linkerpaneel, klik **de Dashboards van het Canvas**.
1. In de hoger-juiste hoek, klik **Nieuw Dashboard**.
1. In **creeer dashboard** doos, ga de 2} Naam van het dashboard **en** Beschrijving **in.**
1. Klik **creëren**.
1. In **voeg rapport** doos toe, uitgezocht **creeer rapport**.
1. Voor de linkerkant, uitgezochte **Lijst**.
1. In de hoger-juiste hoek, klik **creëren rapport**.
1. (Facultatief) volg de stappen hieronder om de **het pictogram van Details** ![ ](assets/details-icon.png) sectie van Details te vormen:
   1. Ga een rapport **Naam** in.
   1. Ga een rapport **Beschrijving** in.
1. Volg hieronder de stappen om de **bouwt lijst** ![ bouwt lijstpictogram ](assets/drilldown-column.png) sectie te vormen:
   1. In het linkerpaneel, klik het **kolommen van de Lijst** pictogram.
   1. Klik **toevoegen kolom**, dan selecteren **Project** > **Naam**.
   1. Klik **toevoegen kolom**, dan selecteren **Project** > **Gezondheid van het Project** > **de Analyse van de Gezondheid**.
   1. Klik **toevoegen kolom**, dan uitgezocht **Project** > **Gezondheid van het Project** > **creeerde bij**.
   1. Klik **toevoegen kolom**, dan selecteren **Project** > **Gezondheid van het Project** > **Etiket van de Gezondheid**.

1. Volg hieronder de stappen om de **** het pictogram van de Filter ![ sectie te vormen van de Filter ](assets/filter-icon.png) {:
   1. In het linkerpaneel, klik het **pictogram van de Filter**.
   1. Selecteer **filter uitgeven**.
   1. Klik **toevoegen voorwaarde** en specificeer dan het gebied u tegen en de bepaling wilt filtreren die bepaalt welk soort voorwaarde het gebied moet ontmoeten. De kolom verschijnt in de voorproefsectie op het recht.
   1. (Facultatief) klik **toevoegen filtergroep** om een andere reeks het filtreren criteria toe te voegen. De standaardoperator tussen de sets is AND. Klik op de operator om deze te wijzigen in OR.

1. Volg hieronder de stappen om de **** montages van de Groep 1} ![ sectie te vormen van de Montages van de DrilldownGroep ](assets/drilldown-group-icon.png):
   1. In het linkerpaneel, klik het **pictogram van de Montages van de Groep**.
   1. Klik **toevoegen groeperend** knoop en dan het gebied selecteren u als groepering wilt tot stand brengen. De kolom voor cijfergroepering wordt weergegeven in de voorbeeldsectie aan de rechterkant.

1. Klik **sparen** om het rapport tot stand te brengen.
