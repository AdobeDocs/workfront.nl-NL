---
user-type: administrator
product-area: system-administration;projects
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: Kick-start scenario-eenvoudig project en taak de invoervoorbereiding
description: Beschrijft in detail de beschikbare montages en de controles voor een basisProject en de Invoer van de Taak gebruikend de methode van het Begin van de Kick.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c095ce9d-b189-449b-bd13-2633837697ed
source-git-commit: b872ae1f712aa1b5af9ef73b87c5fbd51697626e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Kick-Starts-scenario: eenvoudig project en taak de invoervoorbereiding

Beschrijft in detail de beschikbare montages en de controles voor een basisProject en de Invoer van de Taak gebruikend de methode van het Begin van de Kick.

## Scenario

Het implementatieteam importeert liever project- en taakinformatie voor actieve projecten in plaats van deze gegevens handmatig in te voeren in het systeem.

* [Projecten](#projects)
* [Takenlijst](#task-list)

### Projecten {#projects}

De volgende lijst toont vier Projecten en hun basisdetails die in de het dossierformaten van het Begin van het Kick moeten worden in kaart gebracht.

In dit scenario wordt ervan uitgegaan dat gebruikers al in Adobe Workfront zijn geïmporteerd. Als de gebruikers nog niet in Workfront zijn, plaats verschillende namen of voltooi het Scenario van het Begin van de Kick met gebruikers voorafgaand aan dit scenario.

1. Implementeer Workfront.

   | Geplande begindatum | Vandaag |
   |---|---|
   | Projectmanager | Jennifer Campbell |
   | Projectsponsor | Marc Lewis |
   | Groep | Marketing |
   | Bedrijf | *YourCompany* |

   {style="table-layout:auto"}

1. Voer het Systeem van u uit.

   | Geplande begindatum | 14 juli 2010XX |
   |---|---|
   | Projectmanager | Pam Reynolds |
   | Projectsponsor | Marc Lewis |
   | Groep | Marketing |
   | Bedrijf | *YourCompany* |

   {style="table-layout:auto"}

1. Documentbeheersysteem implementeren.

   | Geplande begindatum | 22 augustus 20XX |
   |---|---|
   | Projectmanager | Jennifer Campbell |
   | Projectsponsor | Ray Andrews |
   | Groep | IT |
   | Bedrijf | *YourCompany* |

   {style="table-layout:auto"}

1. Nieuw kalendersysteem implementeren.

   | Geplande begindatum | 6 september, 20XX |
   |---|---|
   | Projectmanager | Pam Reynolds |
   | Projectsponsor | Ray Andrews |
   | Groep | IT |
   | Bedrijf | *YourCompany* |

   {style="table-layout:auto"}

### Takenlijst {#task-list}

In de volgende takenlijst worden te vereenvoudigde takenlijsten voor de projecten weergegeven. Het enige verschil tussen de projecten is de begindatum en de vooruitgang die bij elk project is geboekt.

De taken van de ouder erven de Duur, het Werk, en de Percentage Voltooiing van kindtaken. Het is niet nodig om die waarden in te stellen voor dat worden summiere taken.

>[!NOTE]
>
>De instructies in dit scenario zijn niet zo expliciet als de stapsgewijze instructies in [Kick-start Scenario: Bedrijf, Groep, Rol, en de Kick-Begint Voorbereiding van de Gebruiker](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-scenario-company-group-role-user-prep.md). De veronderstelling is u reeds hebt geleerd om waarden van het Bedrijf en de Bladen van de Groep op te zoeken en te kopiëren, zodat zullen deze stappen worden vermeld, maar niet specifiek geschetst.

1. Configureren.
1. Importeer gebruikers.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bovenliggende taak</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>1 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>1 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Kalender: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Machtigingen instellen.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bovenliggende taak</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prood</td> 
      <td>2</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>1 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>1 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Kalender: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Groepen samenstellen.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Ray Andrews</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bovenliggende taak</td> 
      <td>1</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prood</td> 
      <td>4</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>2 dagen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>4 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 100%</p> <p>Kalender: 25%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Training voorbereiden.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>2 dagen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>4 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 50%</p> <p>Kalender: 100%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Doorlopend ondersteuningsbeleid ontwikkelen.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>2 dagen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>4 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 100%</p> <p>Docs: 50%</p> <p>Kalender: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Uitrollen.

   | Prood | 1, 6, 7 |
   |---|---|

   {style="table-layout:auto"}

1. Treingebruikers.

   <table style="table-layout:auto"> 
    <col width="50%"> 
    <col width="50%"> 
    <tbody> 
     <tr> 
      <td role="rowheader">Toegewezen aan</td> 
      <td>Chris Manning</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bovenliggende taak</td> 
      <td>8</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Duur</td> 
      <td>1 dag</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Werk</td> 
      <td>2 uur</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Percentage voltooid</td> 
      <td> <p>Workfront: 0%</p> <p>HR: 0%</p> <p>Docs: 0%</p> <p>Kalender: 0%</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Sjabloon downloaden

Ga naar de Kick-Starts pagina. Selecteer het Bedrijf, de Groep, het Project, de Taak, en de voorwerpen van de Gebruiker. Schakel het selectievakje Bestaande gegevens opnemen in (voer deze handeling uit om snel te verwijzen naar bedrijven, groepen en gebruikers-id&#39;s). Klik op de knop Downloaden.

## Details invoerproject

Open het Workfront.xlsx-bestand dat u net hebt gedownload. Ga naar het PROJ-projectblad.

![](assets/im2-350x14.png)\
Tenzij u reeds projecten in Workfront hebt gecreeerd, zou het leeg moeten zijn.

![](assets/im10-350x42.png)

Stel de waarden in voor de volgende projectvelden:

* **De kolom isNew instellen**
Voer TRUE in de rijen 3 tot en met 6 in voor de kolom isNew.
* **Unieke id&#39;s instellen**
Voer een unieke id in elke rij in voor de kolom Id. Gewoonlijk werken gehele getallen die beginnen bij 1 goed bij het maken van nieuwe records.
* **Projectnamen instellen**
Voer de namen van elk project in de kolom setName in.
* **Projectschema instellen**

  Voer de id in van het programma dat u wilt gebruiken in het veld setScheduleID

* **De geplande begindatum van het project instellen**

  Voer de datum en de tijd in de kolom setPlannedStartDate in met de tijd en de datum waarop het project moet worden gestart. Als het project leeg wordt gelaten, importeert Workfront het met de datum van de huidige dag en een tijdstempel van middernacht van die dag volgens de tijdzone van de browser.

* **Taaknummers instellen**
De waarden van de input in de setTaskNumber kolom om de orde te controleren de taken in het projectplan zullen verschijnen.
* **Geef projectdatums op.**
Voer de geplande begindatum in voor elk project in de kolom setPlannedStartDate.
* **Stel andere benodigde gegevens in.**
Vul desgewenst andere gegevens in, zoals een beschrijving of de huidige status. Zoek omhoog IDs van de Groep voor elk project op het blad van de Groep van de GROEP en input hen in de setGroupID kolom voor de respectieve projecten. Zoek omhoog identiteitskaart van het Bedrijf voor de projecten op het blad van het Bedrijf CMPY en input het in de kolom setCompanyID. Zoek de Gebruiker - identiteitskaart voor elke projecteigenaar op het Gebruikersblad van de GEBRUIKER en voer het in de setOwnerID kolom in. Zoek de gebruikersnaam voor elke projectsponsor op het gebruikersblad en voer deze in de kolom setSponsorID in.

![](assets/im9-350x24.png)

>[!NOTE]
>
>Acceptabele waarden voor de velden Status en Prioriteit kunnen worden gevonden door de status en voorkeuren voor de prioriteit van elk object in het gedeelte Workflow Setup van Workfront te bekijken.

## Gegevens invoertaak

U kunt informatie over de taken op het project toevoegen, aangezien u het project gebruikend schoppen-begin invoert.

Open het Workfront.xlsx-bestand dat u net hebt gedownload. **Ga naar het TASK Taakblad.**

Dit blad moet leeg zijn, tenzij u al taken hebt gemaakt in Workfront.

![](assets/im8-350x14.png)

![](assets/im7-350x43.png)

![](assets/im6-350x16.png)

De gemakkelijkste manier om taken in kaart te brengen is één project in een tijd (vooral wanneer de taken het zelfde op elk project zijn). U kunt het taakplan voor het eerste project dan kopiëren en kleine aanpassingen aan het taakplan voor de verdere projecten aanbrengen. Bij de overige stappen wordt ervan uitgegaan dat u alleen taken voor het Workfront-project implementeren maakt. Volgens het scenario, zult u 9 taken per project invoeren, zodat inputWAAR in rijen 3 door 11 voor de isNew kolom.

Stel de waarden in voor de volgende taakvelden:

* **Id&#39;s instellen**
Voer in elke rij een unieke id in voor de kolom Id.
* **Namen instellen**
Voer de taaknamen in de kolom setName in.
* **Project-id bevestigen**
Voer de id in die u instelt voor het Workfront-project Implementeren. Controleer het PROJ-projectblad om te controleren of deze de juiste id heeft.
* **Gebruikers instellen**
Ga naar het Gebruikersblad van de Gebruiker omhoog identiteitskaart voor de gebruiker te zoeken die aan elke taak wordt toegewezen en deze waarden in de respectieve cellen in de setAssignedToID kolom in te voeren.
* **Taakrelaties identificeren**
Voor de taken 2 tot en met 5 voert u een 1 in de kolom setParentID in. Voer voor taak 9 een 8 in de kolom setParentID in. Voer in de kolom setPredecessorString het taaknummer voor elke voorgangstaak in. In gevallen waar een taak veelvoudige voordecessors, zoals taak 8 in dit scenario heeft, zult u een komma moeten gebruiken om elke identiteitskaart van de voorgangertaak te scheiden. De voorgangers kunnen met vertraging op niet-Finish-Begin verhoudingen worden bepaald door steno te gebruiken die in het Creërende artikel van de Verhouding van de Voorganger wordt beschreven.
* **Duur instellen**
Stel de duur voor elke taak in door het aantal uren, dagen, weken of maanden voor de taak in te voeren in het veld setDuration. Voer vervolgens de tijdseenheid in het veld setDurationUnit in.

  |   | Acceptabele waarde |
  |---|---|
  | Minuten | M |
  | Uren | H |
  | Dagen | D |
  | Weken | W |
  | Maanden | T |

  Minuten kunnen ook worden weergegeven als fractie van een uur (bijv. minuten = 5 uur)

* Stel de hoeveelheid inspanning voor elke taak in het veld setWorkRequired in. Voer vervolgens de werkeenheid in het veld setWorkUnit in. Als de waarde Vereist werk van de duur verschillend is, zult u ook A in het setDurationType gebied moeten invoeren.

  | Duur | Acceptabele waarde |
  |---|---|
  | Berekende toewijzing | A |
  | Berekend werk | W |
  | Inzet gedreven | D |
  | eenvoudig | S |

* Voer de gehele numerieke representatie in van het percentage dat is voltooid in het veld setPercentComplete voor elke taak. Deze waarde mag het percentagesymbool (%) niet bevatten.
* Voeg desgewenst een beschrijving en andere details toe voor elke taak die u maakt.

  ![](assets/im5-350x35.png)

* De kolommen setPlannedStartDate en setTaskConstraint worden niet gebruikt om de chronologie van dit project uit te bouwen omdat wij op predecessor verhoudingen vertrouwen. In plaats daarvan kunt u een datum invoeren voor elke taak. Als u dit doet, zeker ben u ook een geldige taakbeperking in de setTaskConstraint kolom verstrekt. Controleer de Taakbeperking en verwante artikelen voor details over geldige waarden voor dit gebied.

  In het geval van dit scenario, is de gemakkelijkste manier om de taken voor de andere projecten uit te bouwen u invoert de taken kopieert u enkel bepaalde en hen kleeft hieronder, die op rij 12 beginnen. Dan zult u:

   1. De waarden in de kolom Id opnieuw nummeren.
   1. Werk de setProjectID-kolom bij naar de waarde die u instelt voor het volgende project.
   1. Werk de waarden setParentID en setPredecessorString bij om de nieuwe id&#39;s te weerspiegelen die aan de taken van dit project zijn toegewezen.
   1. Werk de taaktoewijzingen bij en het percentage is voltooid.
   1. Herhaal deze stappen voor de taken van het volgende project.

* **Het Excel-bestand importeren**

  Volg de aanwijzingen in [Gegevens naar Adobe Workfront importeren met een Kick-startsjabloon](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
