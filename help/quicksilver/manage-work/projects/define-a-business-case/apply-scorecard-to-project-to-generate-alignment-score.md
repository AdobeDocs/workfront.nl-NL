---
navigation-topic: business-case-and-scorecards
title: Pas een scorecard op een project toe en produceer een Score van de Uitlijning
description: U kunt een scorecard gebruiken om te meten hoe goed een project zich op de eerder vastgestelde criteria van een portefeuille richt. Een scorecard weerspiegelt vaak de missie, de waarden, en de strategische doelstellingen van een organisatie.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 921749caf6a61fa4f0efae9357c6e05c581421c5
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 0%

---

# Pas een scorecard op een project toe en produceer een Score van de Uitlijning

U kunt een scorecard gebruiken om te meten hoe goed een project zich op de eerder vastgestelde criteria van een portefeuille richt. Een scorecard weerspiegelt vaak de missie, de waarden, en de strategische doelstellingen van een organisatie.

Voor meer informatie over scorecards en hoe u kunt creëren, zie [Een scorecard maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Zakelijk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten bewerken</p> <p>Toegang tot Portfolio weergeven of vergroten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een project beheren</p> <p>Machtigingen voor een portfolio weergeven of hoger </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Projectscorecards {#project-scorecards}

* [Overzicht van Scorecards](#scorecards-overview)
* [Projectscorecards](#project-scorecards)

### Overzicht van Scorecards {#scorecards-overview}

Typisch, voltooit een projectmanager de scorecard informatie om een groeperingswaarde tussen 0 en 100 voor het project te veroorzaken. De geproduceerde waarde wordt later gebruikt wanneer de portefeuillebeheerder de projecten in portefeuille optimizer controleert om hen te vergelijken.

Raadpleeg het artikel voor meer informatie over het optimaliseren van portfolio&#39;s [Overzicht van Portfolio optimaliseren](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Pas een scorecard op een project toe

Als gebruiker met een vergunning van het Plan en leidt toestemmingen aan een project, kunt u een scorecard aan het project vastmaken.

Voor meer informatie over projecttoestemmingen, zie [Een project delen in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

U kunt scorecards aan een project als deel van de bouw van het bedrijfsgeval voor het project toevoegen.

Voor meer informatie over het bouwen van een bedrijfscase raadpleegt u [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Uw beheerder van Adobe Workfront of groepsbeheerder moet de sectie van het Scorecard op het BedrijfsGeval gebied van uw projecten toelaten alvorens u tot scorecards van de BedrijfsGeval kunt toegang hebben. Voor informatie over het opzetten van projectvoorkeur en het toelaten van gebieden van het BedrijfsGeval, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Een scorecard toepassen op een project:

1. Ga naar een project waarop u een scorecard wilt toepassen.
1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. Zoek de **Scorecard** van de Business Case.\
   U moet een scorecard vóór creëren **Scorecard** in de Business Case weergegeven.

   Voor informatie over het creëren van een scorecard, zie [Een scorecard maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Selecteer een scorecard in het keuzemenu.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Geef een antwoord op voor alle vragen in de scorecard.

   Workfront past een score toe op elke beantwoorde vraag en berekent een algemene projectscore op basis van de individuele score van elke vraag.

   Voor meer informatie over het produceren van de project algemene groeperingsscore, zie [Een uitlijningsscore genereren voor een project](#generate-an-alignment-score-for-a-project).

1. Klikken **Opslaan** om scorecard te bewaren en het project te scoren.

   scorecard wordt nu geassocieerd met het project en het project wordt genoteerd.

1. (Voorwaardelijk) wanneer de veranderingen in de waarden van scorecard vragen voorkomen, moet u scorecard opnieuw berekenen om op de nieuwe waarden voor de projectscore te wijzen. U kunt als volgt de scorecard opnieuw berekenen:

   1. Ga naar een lijst met projecten en selecteer alle projecten in de lijst.
   1. Klik op de knop **Bewerken** boven aan de lijst.
   1. Klikken **Instellingen** in het linkerpaneel, dan controleer **Scorecards opnieuw berekenen** aan het einde van het gebied Instellingen.
   1. Klik op Opslaan. Hierdoor wordt de score opnieuw berekend op basis van de scorecards die voor alle geselecteerde projecten zijn gekoppeld.

      >[!NOTE]
      >
      >   <span class="preview">De optie om scorecards opnieuw te berekenen is verwijderd uit de voorvertoningsomgeving wanneer u projecten bulksgewijs bewerkt. </span>


## Een uitlijningsscore genereren

* [Een uitlijningsscore genereren voor een project](#generate-an-alignment-score-for-a-project)
* [Een uitlijningsscore genereren voor een portfolio](#generate-an-alignment-score-for-a-portfolio)

### Een uitlijningsscore genereren voor een project {#generate-an-alignment-score-for-a-project}

De uitlijningsscore is de waarde die wordt geproduceerd nadat de scorecard is voltooid.

Scorecards bevatten vragen met antwoordkeuzen waaraan numerieke waarden zijn toegewezen, uitlijningspunten genoemd. Deze punten worden gebruikt om te bepalen hoe goed het project zich op uw organisatie richt. De uitlijningspunten voor elke vraag bevatten een getal tussen 0 en 100.

Wanneer scorecard wordt voltooid, berekent Workfront de groeperingsscore van het project als percentage, gebruikend de volgende formule:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Zie voor meer informatie [Een scorecard maken](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Een uitlijningsscore genereren voor een portfolio {#generate-an-alignment-score-for-a-portfolio}

De uitlijningsscore van het portfolio is een gemiddelde van de uitlijningsscores van alle projecten in het portfolio.

Wanneer de scorecards van de projecten worden voltooid, gebruikt Workfront die waarden om de groeperingsscore van de portefeuille als percentage te berekenen, gebruikend de volgende formule:

Portfolio-uitlijningsscore = de som van de percentages van de uitlijningsscores van het project/het aantal projecten in het portfolio

>[!NOTE]
>
>Als een project geen scorecard verbonden aan het heeft, en daarom heeft het geen groeperingsscore, wordt het beschouwd als om een 0% groepering in de portefeuille te hebben. Het project wordt in aanmerking genomen in het aantal projecten in de portefeuille.

## De uitlijningsscore weergeven

U kunt de groeperingsscore van een project op het projectniveau, of in Portfolio bekijken Optimizer.

* [De score voor uitlijning weergeven voor een project](#View%20the)
* [Bekijk de Scores van de Uitlijning van het project en van de portefeuille in Portfolio Optimizer](#View%20the2)

### De score voor uitlijning weergeven voor een project

U kunt de uitlijningsscore van een project weergeven op projectniveau als u Contribute-rechten voor het project hebt.

1. Ga naar het project waarvan de Score van de Uitlijning u wilt bekijken.
1. Klikken **Bedrijfs-case** in het linkerdeelvenster.
1. Ga naar de **Overzicht van bedrijfscase** aan de rechterkant van het scherm.

   De score voor uitlijning bevindt zich in het overzicht Bedrijfscase, in het gedeelte **Uitgelijnd** waarde.

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Bekijk de Scores van de Uitlijning van het project en van de portefeuille in Portfolio Optimizer

U kunt de uitlijningsscore van een project of van een portfolio weergeven in Portfolio Optimizer als u beheertoegang tot het portfolio hebt.

Voor meer informatie over de informatie die in de Optimizer van de Portfolio wordt getoond, zie [Overzicht van Portfolio optimaliseren](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Zoek de score voor uitlijning van het project in Portfolio Optimizer](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Zoek de uitlijningsscore van het portfolio in Portfolio Optimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Zoek de score voor uitlijning van het project in Portfolio Optimizer {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png)vervolgens **Portfolio**.

1. Klik op de naam van een Portfolio.
1. Klikken **Portfolio optimaliseren** in het linkerdeelvenster.

   De functie Portfolio optimaliseren wordt weergegeven.

1. De uitlijningsscore van een project wordt weergegeven als een percentage in het deelvenster **Uitlijning** kolom van de Portfolio Optimizer.

   Dit is de groeperingsscore van het project dat op scorecard wordt gebaseerd verbonden aan het project.

#### Zoek de uitlijningsscore van het portfolio in Portfolio Optimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Ga naar de **Projecten** in de algemene navigatiebalk.
1. Selecteer **Portfolio** tab.
1. Klik op de naam van een Portfolio.
1. Selecteer **Portfolio optimaliseren** tab.
1. Boven aan de functie Portfolio optimaliseren vindt u de **Uitgelijnd** en de **Uitlijning** een maatstaf die de uitlijningsscore van de portefeuille aangeeft.

   Dit is de uitlijningsscore van het portfolio.

   Voor meer informatie over hoe de uitlijningsscore van een portfolio wordt gegenereerd, raadpleegt u [Een uitlijningsscore genereren voor een portfolio](#generate-an-alignment-score-for-a-portfolio).

## Overzicht van de Portfolio Optimizer Score

Er is een verschil tussen de uitlijningsscore en de optimaliseringsscore van een project voor het portfolio.

De groeperingsscore van een project wordt berekend gebaseerd op de punten die na de voltooiing van scorecard worden verkregen. Deze score wordt vervolgens gebruikt om de uitlijningsscore van het portfolio te bepalen. De uitlijningsscore wordt weergegeven als een percentage.

De uitlijningsscore van een project wordt weergegeven in het deelvenster **Uitlijning** kolom van de Portfolio Optimizer.

De score voor het optimaliseren van het portfolio is een positie die automatisch wordt berekend in de Portfolio Optimizer waarmee aan projecten prioriteiten kunnen worden toegewezen. De score voor het optimaliseren van het portfolio wordt weergegeven als een indicatiepictogram, vergezeld van een nummer en wordt weergegeven in het dialoogvenster **Score** kolom van de Portfolio Optimizer. Een Portfolio Optimizer score wordt geproduceerd slechts wanneer alle secties van het BedrijfsGeval, behalve Doelstellingen worden voltooid.

Voor meer informatie over het creëren van een BedrijfsGeval voor een project, zie [Een bedrijfscase maken voor een project](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Voor meer informatie over het berekenen van de score van een project voor het optimaliseren van het portfolio raadpleegt u [Overzicht van de Portfolio Optimizer Score](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
