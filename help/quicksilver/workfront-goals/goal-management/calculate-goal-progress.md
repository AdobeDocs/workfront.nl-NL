---
product-previous: workfront-goals
navigation-topic: goal-management
title: Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen
description: De vooruitgang van het doel wordt gedreven door vooruitgangsindicatoren zoals activiteiten, resultaten, of kinddoelstellingen. De voorwaarde van het doel wordt bepaald door de vooruitgang van het doel op het huidige tijdstip.
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 0%

---

# Overzicht van de voortgang en conditie van het doel in de Adobe Workfront-doelstellingen

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>Uw organisatie moet het volgende hebben om de functionaliteit te gebruiken die in dit artikel wordt beschreven:
>
>* Een Pro of hoger [Adobe Workfront-plan](https://www.workfront.com/plans).
>* Een Adobe Workfront Goals-licentie in aanvulling op een Workfront-licentie.
>
>Neem contact op met uw Workfront-accountmanager voor meer informatie over een Workfront Goals-licentie.
>Voor meer informatie over toegang tot Workfront Goals raadpleegt u [Vereisten voor het gebruik van Workfront-doelen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

Adobe Workfront berekent automatisch de voortgang van het doel op basis van de voortgangsindicatoren.

## Vereisten

U moet het volgende hebben voordat u kunt beginnen:

* Een lay-outsjabloon die het gebied Doelen in het hoofdmenu bevat.

## Overzicht van de voortgang en drempel van het doel

Nadat u een doel hebt geactiveerd, begint u met het berekenen van de voortgang en toestand van de Workfront Goals en worden de volgende indicatoren weergegeven wanneer u de cursor op het veld Voortgang plaatst:

| Indicator | Beschrijving van de indicator |
|---|---|
| Werkelijk percentage voltooid | Hoeveel van het doel is tot nu toe daadwerkelijk bereikt. Workfront Goals berekent deze waarde door het gemiddelde te nemen van het percentage van alle voortgangsindicatoren die bij het doel horen. |
| Verwacht percentage voltooid | Hoeveel van het doel moet tot nu toe worden verwezenlijkt om het doel tijdig te kunnen voltooien. De Doelen van Workfront berekent deze waarde door de Duur van het doel en het huidige tijdstip te bekijken. Deze waarde moet op het huidige tijdstip worden weergegeven als het doel op tijd moet worden voltooid. |
| Voortgang | Een label dat aangeeft of het doel op tijd moet worden voltooid of dat het risico loopt of niet kan worden voltooid. |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [Werkelijk percentage voltooid](#actual-percent-complete)
* [Verwacht percentage voltooid](#expected-percent-complete)
* [Voortgang en toestand](#progress)

### Werkelijk percentage voltooid {#actual-percent-complete}

De Doelen van Workfront berekent automatisch het daadwerkelijke percentage volledig van een doel dat op het percentage volledig gemiddelde van de indicatoren van de doelvooruitgang wordt gebaseerd.

De volgende punten worden beschouwd als voortgangsindicatoren voor doelstellingen:

* Resultaten

  Voor informatie over het toevoegen van resultaten aan doelstellingen, zie [Resultaten toevoegen aan doelen in Adobe Workfront-doelen](../../workfront-goals/results-and-activities/add-results-to-goals.md).

* Activiteiten

  Voor informatie over het toevoegen van activiteiten met inbegrip van projecten aan doelstellingen, zie [Activiteiten toevoegen aan doelen in Adobe Workfront](../../workfront-goals/results-and-activities/add-activities-to-goals.md).

* Uitgelijnde onderliggende doelen

  Voor informatie over ouder en kinddoelstellingen, zie [Richt doelstellingen door hen in de Doelen van Adobe Workfront te verbinden](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

  Workfront Goals berekent het werkelijke percentage voltooid met de volgende formule:

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  Als een doel bijvoorbeeld een resultaat heeft dat 20% voltooid is, een handmatige voortgangsbalk die 30% voltooid is, een project dat 10% voltooid is en een kinderdoel dat 40% voltooid is, is het streefpercentage voltooid 25%.

### Verwacht percentage voltooid {#expected-percent-complete}

De Doelen van Workfront berekent automatisch het verwachte percentage volledig van een doel dat op het totale aantal dagen in de duur van het doel evenals op het aantal dagen wordt gebaseerd die sinds de doel begindatum zijn overgegaan.

Workfront Goals berekent het verwachte percentage voltooid met de volgende formule:

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

Als een doel bijvoorbeeld binnen 90 dagen moet worden voltooid en vandaag de 45e dag van die duur is, is het verwachte percentage voltooid 50%.

### Voortgang en toestand {#progress}

De Doelen van Workfront berekent een vooruitgangspercentage en wijst een vooruitgangsetiket aan doelstellingen toe, die op welk percentage van het Verwachte percentage volledig op het huidige tijdstip is bereikt. De kleur van de volledige bar van het doelpercentage verandert om op de vooruitgang van het doel te wijzen.

De voorwaarde van het doel wordt dienovereenkomstig ook bijgewerkt, om erop te wijzen of het doel op doel is op tijd te voltooien, of het achterloopt achterop.

Met de volgende formule wordt het voortgangspercentage van een doel berekend aan de hand van de Workfront-doelen:

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

Als het verwachte percentage voltooid bijvoorbeeld 53% is op het huidige moment en het werkelijke percentage voltooid 30% is, is het percentage van de voortgang van het doel voltooid 56%. Workfront Goals noemt dit doel met de voorwaarde &#39;In Trouble&#39;.

In het volgende diagram ziet u de relatie tussen de voorwaardelabels en het voortgangspercentage:

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

In de onderstaande tabel staan de labels voor de doelvoorwaarde en de percentages voor de voortgang van het doel die aan elk label zijn gekoppeld.

>[!TIP]
>
>De labels voor de voorwaarde van het doel komen overeen met de naam en kleur van de Workfront-projectvoorwaarde.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Naam van voortgang van doel</b></td> 
   <td><b>Definitie van voortgang van het doel</b></td> 
   <td><b>Percentage voortgang van de doelstelling</b></td> 
   <td><b>Kleur van percentage van volledige balk</b></td> 
   <td><b>Voorwaardeindicator, pictogram</b></td> 
  </tr> 
  <tr> 
   <td>Nieuw</td> 
   <td> <p>Het doel is pas gecreëerd en het registreert nog geen vooruitgang. De voortgang van een doel wordt als Nieuw weergegeven totdat iemand de voortgang voor het eerst bijwerkt. </p> <p>Voor informatie over het bijwerken van de voortgang van het doel raadpleegt u <a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Voortgang van Adobe Workfront-doelen bijwerken</a>.</p> </td> 
   <td>Geen percentage</td> 
   <td>Geen balk</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Op doel</span> </p> </td> 
   <td>Het doel presteert zoals verwacht en het is zeer waarschijnlijk dat het op tijd zal worden voltooid. </td> 
   <td>90-100%</td> 
   <td>Groen</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>Risico</span> </p> </td> 
   <td>Het doel loopt achter, maar het kan nog steeds mogelijk zijn om het op tijd af te ronden. </td> 
   <td>70-89,99%</td> 
   <td>Geel</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>In problemen</span> </p> </td> 
   <td> <p>Het is zeer waarschijnlijk dat het doel niet op tijd zal worden bereikt. </p> </td> 
   <td>0-69,99%</td> 
   <td>Rood</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_Probleem_pictogram_voorwaarde.png"></td> 
  </tr> 
 </tbody> 
</table>