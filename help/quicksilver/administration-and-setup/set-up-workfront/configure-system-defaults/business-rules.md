---
user-type: administrator
product-area: system-administration
navigation-topic: business rules
title: Zakelijke regels maken en bewerken
description: Met een bedrijfsregel kunt u validatie toepassen op Workfront-objecten en voorkomen dat gebruikers een object maken, bewerken of verwijderen als aan bepaalde voorwaarden is voldaan. De bedrijfsregels helpen gegevenskwaliteit en operationele efficiency te verbeteren door acties te verhinderen die gegevensintegriteit in gevaar zouden kunnen brengen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 780c996c-5cf1-42fe-898d-2cc208bbae7b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b190de6b6ef9ce53e96475d426a4d39cfbd4df4
workflow-type: tm+mt
source-wordcount: '1864'
ht-degree: 0%

---

# Zakelijke regels maken en bewerken

Met een bedrijfsregel kunt u validatie toepassen op Workfront-objecten en voorkomen dat gebruikers een object maken, bewerken of verwijderen als aan bepaalde voorwaarden is voldaan. De bevestiging van bedrijfsregels helpt om gegevenskwaliteit en operationele efficiency te verbeteren door acties te verhinderen die gegevensintegriteit in gevaar zouden kunnen brengen.

Organisaties die beschikken over het Workflow Ultimate-pakket kunnen ook bedrijfsregels configureren om handelingen voor het gemaakte, bewerkte of gewijzigde object te automatiseren als aan bepaalde voorwaarden is voldaan. Tot de beschikbare acties behoren het delen van het object of het koppelen van een aangepast formulier aan het object.


Eén bedrijfsregel kan slechts aan één object worden toegewezen. Bijvoorbeeld, als u een bedrijfsregel creeert voor het niet uitgeven van projecten onder bepaalde voorwaarden, kunt u niet de zelfde regel op taken toepassen. U zou een afzonderlijke bedrijfsregel met de zelfde voorwaarden voor taken moeten tot stand brengen.

Toegangsniveaus en het delen van objecten hebben een hogere prioriteit dan bedrijfsregels wanneer een gebruiker met een voorwerp in wisselwerking staat. Bijvoorbeeld, als een gebruiker een toegangsniveau of een toestemming heeft die het uitgeven van een project niet toestaat, dan zouden die belangrijkheid over een bedrijfsregel nemen die het uitgeven van een project onder bepaalde voorwaarden toestaat.

Wanneer meer dan één bedrijfsregel op een voorwerp van toepassing is, dan worden de regels allen gevolgd maar niet in een bepaalde orde toegepast. U hebt bijvoorbeeld twee bedrijfsregels. Eén beperkt het maken van kosten in de maand februari. Het tweede verhindert het uitgeven van een project wanneer de projectstatus Voltooid is. Als een gebruiker probeert om een uitgave aan een voltooid project in juni toe te voegen, kan de uitgave niet worden toegevoegd omdat het de tweede regel heeft teweeggebracht.

De bedrijfsregels zijn van toepassing op het creëren van, het uitgeven van, en het schrappen van voorwerpen door API evenals in de interface van Workfront.

>[!NOTE]
>
>Omdat de bedrijfsregels bepaalde acties blokkeren, zou u uw bedrijfsregels eerst in een zandbak of voorproefmilieu moeten vormen en hen grondig testen alvorens hen in productie toe te laten.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr>
   <td>Adobe Workfront-pakket
   </td>
   <td> <p>Validatie van bedrijfsregels:<ul><li><p>Ultimate</p></li><li>
    <p>Workflow Ultimate</p></li></ul></p><p>Automatisering van bedrijfsregels:<ul><li>
    <p>Workflow Ultimate</p></li><ul></p>
   </td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>Systeembeheerder</td> 
  </tr>  
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Scenario&#39;s voor bedrijfsregels

* [Scenario&#39;s voor validatie van bedrijfsregels](#scenarios-for-business-rule-validation)
* [Scenario&#39;s voor bedrijfsregelautomatisering](#scenarios-for-business-rule-automation)

### Scenario&#39;s voor validatie van bedrijfsregels

De indeling van een validatie van een bedrijfsregel is &quot;ALS aan de gedefinieerde voorwaarde is voldaan, kan de gebruiker de actie op het object niet uitvoeren en wordt het bericht weergegeven.&quot;

De syntaxis voor de eigenschappen en andere functies in een bedrijfsregel is hetzelfde als de syntaxis voor een berekend veld in een aangepast formulier. Voor meer informatie over de syntaxis, zie [&#x200B; berekende gebieden met de vormontwerper &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.

Voor informatie over IF- verklaringen, zie [&#x200B; &quot;IF&quot;verklaringenoverzicht &#x200B;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/if-statements-overview.md) en [&#x200B; de exploitanten van de Voorwaarde in berekende douanevelden &#x200B;](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/condition-operators-calculated-custom-expressions.md).

Voor informatie over op gebruiker-gebaseerde vervangingen, zie [&#x200B; Op gebruiker-gebaseerde vervangingen van het Gebruik om rapporten &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md) te generaliseren.

Voor informatie over op datum-gebaseerde vervangingen, zie [&#x200B; Op datum-gebaseerde vervangingen van het Gebruik om rapporten &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md) te generaliseren.

Een API-jokerteken is ook beschikbaar in bedrijfsregels. Gebruik `$$ISAPI` om de regel alleen in de API te activeren. Gebruik `!$$ISAPI` om de regel alleen in de gebruikersinterface af te dwingen en gebruikers toe te staan de regel via de API te omzeilen.

* Deze regel verbiedt gebruikers bijvoorbeeld voltooide projecten te bewerken via de API. Als het jokerteken niet werd gebruikt, zou de regel de actie in zowel het gebruikersinterface als API blokkeren.

  ```
  IF({status} = "CPL" && $$ISAPI, "You cannot edit completed projects through the API.")
  ```

De jokertekens `$$BEFORE_STATE` en `$$AFTER_STATE` worden in expressies gebruikt om de veldwaarden van het object te benaderen voor en na elke bewerking.

* Deze jokertekens zijn beide beschikbaar voor de bewerktrigger. De standaardstatus voor de bewerktrigger (als er geen status is opgenomen in de expressie) is `$$AFTER_STATE` .
* De trigger voor het maken van objecten staat alleen de instructie `$$AFTER_STATE` toe, omdat de status before niet bestaat.
* De trigger voor het verwijderen van objecten staat alleen de instructie `$$BEFORE_STATE` toe, omdat de status after niet bestaat.

Sommige eenvoudige bedrijfsregelscenario&#39;s zijn:

* De gebruikers kunnen geen nieuwe uitgaven tijdens de laatste week van Februari toevoegen. Deze formule kan als volgt worden omschreven:

  ```
  IF(MONTH($$TODAY) = 2 && DAYOFMONTH($$TODAY) >= 22, "You cannot add new expenses during the last week of February.")
  ```

* De gebruikers kunnen niet de projectnaam van een project in Volledige status uitgeven. Deze formule kan als volgt worden omschreven:

  ```
  IF({status} = "CPL" && {name} != $$BEFORE_STATE.{name}, "You cannot edit the project name.")
  ```

Het systeem staat één bedrijfsregel per voorwerp per trekker toe. Bijvoorbeeld, wordt één uitgeeft trekkerregel toegestaan voor kwesties. U kunt echter meerdere regels opnemen in een formule met geneste IF-instructies.

Een scenario met geneste IF-instructies is:

De gebruikers kunnen voltooide projecten niet uitgeven en kunnen geen projecten met een Geplande Datum van de Voltooiing in Maart uitgeven. Deze formule kan als volgt worden omschreven:

```
IF(
    $$AFTER_STATE.{status}="CPL",
    "You cannot edit a completed project",
    IF(
        MONTH({plannedCompletionDate})=3,
        "You cannot edit a project with a planned completion date in March")
)
```

### Lokalisatie inschakelen in een bedrijfsregel

Als uw organisatie aangepaste lokalisatie gebruikt, moet u vertaling van een bedrijfsregelbericht in de bedrijfsregel inschakelen. Als vertaling niet wordt toegelaten, verschijnt het bericht aan de lezer in het Engels, zelfs als de berichttekst in de Localization lijst is en browser van de gebruiker aan de aangewezen taal wordt geplaatst.

Wanneer het vormen van de regel, neem het woord TRANSLATE vóór het bericht op, en sluit het bericht tussen haakjes in.

>[!BEGINSHADEBOX]

Voorbeeld:

In dit voorbeeld wordt ervan uitgegaan dat het bericht &quot;U kunt voltooide projecten niet bewerken&quot; is opgenomen in het lokalisatiegebied van Setup en dat de browser van de gebruiker is ingesteld op de gelokaliseerde taal.

* `IF({status} = "CPL", "You cannot edit completed projects.") `
Het bericht wordt in het Engels weergegeven.
* `IF({status} = "CPL", TRANSLATE("You cannot edit completed projects."))`
Het bericht wordt weergegeven in de gelokaliseerde taal.

>[!ENDSHADEBOX]

Voor informatie over douanelokalisatie, zie [&#x200B; douanelokalisatie &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-custom-localization.md) vormen.

## Scenario&#39;s voor bedrijfsregelautomatisering

>[!NOTE]
>
>Uw organisatie moet beschikken over een Workflow Ultimate-pakket om bedrijfsregelautomatisering te kunnen gebruiken.

De indeling van een bedrijfsregelautomatisering is &quot;ALS aan de gedefinieerde voorwaarde is voldaan, wordt de geselecteerde automatisering geactiveerd.&quot;

Voor automatiseringsformules voor bedrijfsregels is geen foutbericht vereist

Gebruik de volgende formule om ervoor te zorgen dat een automatisering wordt uitgevoerd wanneer het geselecteerde object en de geselecteerde actie plaatsvinden, bijvoorbeeld wanneer een project wordt gemaakt:

```
IF(true, true)
```

Om een project te delen slechts als dat project is goedgekeurd, gebruik een formule als het volgende:

```
IF({status} = "APR", true)
```

U kunt vervangingen in de acties van de bedrijfsregel gebruiken, zoals die in de sectie [&#x200B; Scenario&#39;s voor de bevestiging van de bedrijfsregel &#x200B;](#scenarios-for-business-rule-validation) worden beschreven.


## Voeg een nieuwe bedrijfsregel toe

{{step-1-to-setup}}

1. Klik **BedrijfsRegels** in het linkerpaneel.
1. Klik **Nieuwe bedrijfsregel**.

1. Typ de **Naam** voor de bedrijfsregel op de dialoog van de regelbouwer.
1. Op **is Actief** gebied, selecteer of de regel actief zou moeten zijn wanneer u het bewaart.

   Als u **Nr** selecteert, wordt de regel bewaard als inactief, en u kunt het later activeren.

1. (Facultatief) ga a **Beschrijving** van de bedrijfsregel in en wat gebeurt wanneer het wordt toegepast.


1. Selecteer het objecttype waaraan u de bedrijfsregel wilt toewijzen.

   ![&#x200B; Uitgezocht een voorwerp &#x200B;](assets/object-for-business-rule4.png)

   U kunt bedrijfsregels toepassen op de volgende objecten:

   * Project
   * Taak
   * Uitgave/verzoek
   * Portfolio
   * Document
   * Programma
   * Kosten
   * Bedrijf
   * Iteratie
   * Factureringsrecord
   * Groep
   * Bron voor niet-arbeid
   * Risico
   * Creditcard
   * Toewijzing
   * Gebruiker
   * Rol
   * Uur
   * Sjabloon
   * Tijd uit
   * Bronpool
   * Functie
   * Broncategorie voor niet-arbeid
   * Bronpool
   * Tijd uit
   * Uur
   * Personeelsformatie
   * Sjabloon
   * Personeelsformatie
<!--
   * <span class="preview">Team</span>
-->

1. Typ de **Naam** voor de bedrijfsregel op de dialoog van de regelbouwer.
1. Op **is Actief** gebied, selecteer of de regel actief zou moeten zijn wanneer u het bewaart.

   Als u **Nr** selecteert, wordt de regel bewaard als inactief, en u kunt het later activeren.

1. Selecteer a **Trekker** voor de bedrijfsregel. De opties zijn:

   * **creeerde** de regel wordt toegepast wanneer een gebruiker probeert om een voorwerp tot stand te brengen.
   * **Bewerkte** de regel wordt toegepast wanneer een gebruiker probeert om een voorwerp uit te geven.
   * **schrapte** de regel wordt toegepast wanneer een gebruiker probeert om een voorwerp te schrappen.

1. Bouw de formule in de formules redacteur, in het centrum van de dialoog van de bedrijfsregel.

   De indeling van een bedrijfsregel is &quot;ALS aan de gedefinieerde voorwaarde is voldaan, is de gebruiker niet in staat tot de actie op het object en wordt het bericht weergegeven.&quot;

   In het formuleringsgebied, zijn de delen van de bedrijfsregel u bouwt de voorwaarde, en het bericht dat in Workfront toont wanneer aan de voorwaarde wordt voldaan.

   * Het &quot;object&quot; is het objecttype dat u hebt geselecteerd bij het maken van de bedrijfsregel. Deze wordt weergegeven in de kop van het dialoogvenster.
   * De &quot;actie&quot; is de trigger die u voor de regel hebt geselecteerd: maak, bewerk of verwijder het object.
   * Omdat het object en de actie al zijn gedefinieerd, neemt u ze niet op in de formule.
   * Het aangepaste foutbericht wordt alleen opgenomen als de regel voor validatie is en aan de gebruiker wordt getoond wanneer deze de bedrijfsregel activeert. Het zou duidelijke instructies moeten geven over wat er mis ging en hoe de kwestie te verhelpen.

     U kunt een statische URL in het foutbericht opnemen om een koppeling te maken naar documentatie of andere nuttige pagina&#39;s om de gebruiker te begeleiden bij het wijzigen van de handeling binnen de beperking van de regel.

     In dit voorbeeld wordt &quot;Meer informatie&quot; gekoppeld aan de URL. `"You are not allowed to add a new project in November.[Learn more](http://url)"` De URL moet tussen haakjes staan, maar koppelingstekst tussen haakjes is niet vereist. U kunt de volledige URL weergeven en het wordt een klikbare koppeling.

   ![&#x200B; voeg bedrijfsregeldialoog &#x200B;](assets/add-business-rule-new.png) toe

   Dit voorbeeld is een bedrijfsregel voor projecten. Als de huidige maand November is, dan worden de gebruikers toegelaten om geen nieuwe projecten tot stand te brengen, en het bericht verklaart dit.

   Voor meer voorbeelden van bedrijfsregels, zie [&#x200B; Scenario&#39;s voor bedrijfsregels &#x200B;](#scenarios-for-business-rules) in dit artikel.

1. (Facultatief) gebruik de formule **Uitdrukkingen** en **Gebieden** in het juiste paneel om bij de bouw van de regel bij te wonen.

   Zoeken naar een expressie of veld om de lijst met beschikbare items te beperken.

   De lijst met beschikbare velden is beperkt tot velden die betrekking hebben op het objecttype voor de bedrijfsregel.

1. (Voorwaardelijk) als u de actie bevestigt, als uw organisatie op het pakket van Workfront Ultimate, op het toen gebied is, selecteer **bevestigen het voorwerp**.

   Voor andere pakketten is deze optie vooraf geselecteerd.

1. (Voorwaardelijk) Als u een andere handeling wilt automatiseren, selecteert u de handeling.

   Voor details op deze acties, zie de sectie [&#x200B; opties van de de regelautomatisering &#x200B;](#business-rule-automation-options) in dit artikel.

   >[!NOTE]
   >
   >Uw organisatie moet zich op het Ultimate-pakket van het Werkschema bevinden om acties naast bevestiging te gebruiken. Als u deze andere opties niet ziet, staat uw organisatie niet in het Workflow Ultimate-pakket.

1. Klik **sparen** wanneer u klaar bent met het bouwen van de bedrijfsregel.

>[!NOTE]
>
>Nadat u een bedrijfsregel hebt toegevoegd, moet u deze testen door het bijbehorende object toe te voegen, te bewerken of te verwijderen om ervoor te zorgen dat de regel correct wordt toegepast.

### Automatiseringsopties voor bedrijfsregels

>[!NOTE]
>
>Uw organisatie moet zich op het Ultimate-pakket van het Werkschema bevinden om acties naast bevestiging te gebruiken. Als u deze andere opties niet ziet, staat uw organisatie niet in het Workflow Ultimate-pakket.

U kunt deze acties plaatsen om te automatiseren wanneer de bedrijfsregel wordt teweeggebracht. Welke acties beschikbaar zijn, is afhankelijk van het geselecteerde objecttype.

| Automatisering | Aanvullende configuratie |
|---|---|
| Een aangepast formulier bijvoegen | Selecteer het aangepaste formulier dat u wilt toevoegen |
| Het object delen | Selecteer de personen, rollen, groepen, bedrijven of toegangsniveaus waarmee u het object wilt delen. |

## Een bedrijfsregel activeren

Wanneer een bedrijfsregel inactief is, is Actief gebied in de lijst van bedrijfsregels vals toont. U kunt de status van de regel niet bijwerken in de lijstweergave.

Een bedrijfsregel activeren:

1. Selecteer de bedrijfsregel in de lijst van regels en klik het Edit pictogram.
1. Selecteer **ja** voor **is Actief** in de dialoog van de bedrijfsregel.
1. Klik **sparen**.

