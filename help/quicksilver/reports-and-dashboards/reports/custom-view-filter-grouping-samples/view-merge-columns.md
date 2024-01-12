---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom'
description: U kunt de informatie die in veelvoudige afzonderlijke kolommen wordt getoond samenvoegen en het tonen in één gedeelde kolom.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 8382b69e6a55af69397dd8f566395143f3c1dcd3
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 0%

---

# Weergave: gegevens uit meerdere kolommen samenvoegen in één gedeelde kolom

<!-- Audited: 1/2024 -->

U kunt de informatie die in veelvoudige afzonderlijke kolommen wordt getoond samenvoegen en het tonen in één gedeelde kolom.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p> Huidige: 
   <ul>
   <li>Verzoek om een weergave te wijzigen</li> 
   <li>Plan om een rapport te wijzigen</li>
   </ul>
     </p>
     <p> Nieuw: 
   <ul>
   <li>Medewerker om een weergave te wijzigen</li> 
   <li>Standaard voor het wijzigen van een rapport</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Overwegingen bij het delen of samenvoegen van kolommen

* U kunt twee aangrenzende kolommen samenvoegen en de informatie van elke kolom tonen die door een lijnonderbreking wordt gescheiden, of u kunt de informatie in twee aangrenzende kolommen zonder scheidingsteken tussen de informatie van elke kolom samenvoegen.
* U kunt de informatie uit meer dan twee kolommen samenvoegen door dezelfde syntaxis toe te passen die in dit artikel wordt beschreven op een reeds gedeelde kolom en een aangrenzende kolom.
* De `valueformat=HTML` regel is verplicht in een gedeelde kolom. Anders bevatten de kolommen geen informatie (ze worden leeg weergegeven) wanneer het rapport uit Adobe Workfront wordt geëxporteerd.
* Voorwaardelijke opmaak wordt mogelijk niet ondersteund in samengevoegde kolommen.

  De volgende uitzonderingen bestaan:

   * Wanneer u informatie in Workfront weergeeft, blijft de opmaak van de eerste kolom behouden en wordt de opmaak van alle andere kolommen genegeerd als de kolommen waaruit een samengevoegde kolom bestaat, een andere opmaak hebben.
   * Bij het exporteren van de weergave naar een PDF-bestand wordt voorwaardelijke opmaak toegepast op de eerste kolom in een samengevoegde kolom.
   * Wanneer u de weergave naar een Excel-bestand exporteert, worden samengevoegde kolommen weergegeven als afzonderlijke kolommen. De afzonderlijke kolommen geven ook hun respectievelijke voorwaardelijke opmaakregels weer.

* Kolommen met de **viewalias** kan de hoeveelheid kolommen beperken die u kunt samenvoegen. Als u deze limieten wilt vermijden, vermijdt u het **viewalias** kenmerk. Als u de opdracht **viewalias** in een kolom, zorg ervoor dat het het laatste punt is dat in de kolom wordt vermeld.

* Als u een lijst met gedeelde kolommen naar een formaat van Excel of van het Lusje Gescheiden uitvoert, worden deze kolommen gescheiden uit in het uitgevoerde dossier.

* Wanneer een of beide kolommen een `tile` tekstveld, wordt automatisch een geforceerd regeleinde ingevoegd in de samengevoegde kolom. Tekstvelden met opmaak zijn bijvoorbeeld `tile` tekstvelden. In dit geval is er een regelcode van `type=tile` wanneer u de kolommen in de tekstmodus weergeeft.

## Gegevens uit twee kolommen samenvoegen zonder een regeleinde

U kunt de gegevens van meerdere afzonderlijke kolommen samenvoegen en deze weergeven in één kolom zonder einden of spaties tussen de waarden van elke kolom.

>[!TIP]
>
>Deze benadering wordt aanbevolen wanneer u twee kolommen samenvoegt die nooit een waarde voor dezelfde record tegelijk kunnen weergeven. Bijvoorbeeld, in een rapport van het Punt van het Werk, kunnen de kolommen van de Naam van de Uitgave en van de Naam van de Taak zonder een lijnonderbreking tussen hen worden samengevoegd omdat een Punt van het Werk nooit een Naam van de Uitgave en een Naam van de Taak tezelfdertijd kan hebben. Een werkitem kan een probleem of een taak in Workfront zijn.

Gegevens van twee kolommen samenvoegen zonder een regeleinde:

1. Als u de tekstmodus voor een weergave gebruikt, voegt u de volgende tekst toe aan de eerste kolom die u wilt samenvoegen:

   `sharecol=true`

   Wanneer u de eerste twee kolommen van een lijst of rapport samenvoegt, gaat Workfront voor elke tekstregel die informatie over het object in de eerste kolom bevat, met `column.0.` en de tekstregels die informatie bevatten over de tweede kolom met `column.1.` .

   U moet het kolomaantal van de eerste kolom met het aantal van die kolom voorafgaan. Kolom tellen begint altijd met de meest linkse kolom van de lijst of het rapport met het label `column.0.`.

   Als u meer dan één kolom deelt, zorg ervoor u het kolomaantal in de lijnen van code toevoegt die de het delen informatie voor elke kolom bevatten.

   **Voorbeeld:** Hier volgt de code in de tekstmodus voor een samengevoegde kolom die drie aparte kolommen bevat, te beginnen met de tweede kolom van de lijst. De samengevoegde waarden zijn Projectnaam, Geplande Begindatum en de naam van de eigenaar van het project en er is geen onderbreking tussen de drie waarden:

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. Klikken **Opslaan** vervolgens **Weergave opslaan**.

## Gegevens uit twee kolommen samenvoegen met een regeleinde

Ga als volgt te werk om de gegevens van meerdere kolommen samen te voegen en weer te geven in één gemeenschappelijke kolom met een regeleinde tussen de waarden van elke kolom:

1. Voeg een derde kolom toe tussen de twee kolommen die u wilt samenvoegen.

   >[!TIP]
   >
   >* De kolommen die u wilt samenvoegen, moeten aan elkaar grenzen.
   >* Klik op de eerste kolom die u wilt samenvoegen.

1. Klikken **Overschakelen naar tekstmodus** en voeg de volgende code toe in de middelste kolom die u in stap 1 hebt toegevoegd:

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. Klik op de eerste kolom en klik **Overschakelen naar tekstmodus** Voeg vervolgens de volgende tekst toe aan de kolom:

   `sharecol=true`

   Wanneer u de eerste twee kolommen van een lijst of rapport samenvoegt, gaat Workfront voor elke tekstregel die informatie over het object in de eerste kolom bevat, met `column.0.`, de kolom met de delende informatie met `column.1.`en de tekstregels die informatie bevatten over de tweede kolom met `column.2.`.

   Als de gecombineerde kolom zich in het midden van de weergave bevindt, worden de kolommen genummerd op basis van hun plaats in de weergave. Kolom tellen begint altijd met de meest linkse kolom van de lijst of het rapport met het label `column.0.`.

   Als u meer dan één kolom deelt, zorg ervoor u het kolomaantal in de lijnen van code toevoegt die de het delen informatie bevatten.

   **Voorbeeld:** Hier volgt de code van de tekstmodus voor een gedeelde kolom die de projectnaam, de geplande begindatum en de naam van de eigenaar van het project met een regeleinde bevat. De gedeelde kolom is de tweede kolom van een projectweergave.


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. Klikken **Opslaan** vervolgens **Weergave opslaan**.
