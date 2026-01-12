---
title: Voorbeelden van Advanced Logic in Custom Forms
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Dit artikel bevat voorbeelden van expressies die worden gebruikt om geavanceerde logica op aangepaste velden samen te stellen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: caf889d6-08a3-4186-9d9c-3cea3a0e4548
source-git-commit: 2e8801d08e3cf14f08435389c128068e2d38caba
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Voorbeelden van geavanceerde logica in aangepaste formulieren

Met logische regels kunt u de velden op een aangepast formulier verder aanpassen.

Dit artikel bevat voorbeelden van expressies die worden gebruikt om geavanceerde logica op aangepaste velden samen te stellen.

Voor meer informatie over het toevoegen van logica aan een douaneformulier, zie [&#x200B; logische regels aan douaneformulieren en gebieden &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) toevoegen.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> </td> 
  </tr>  
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voorbeelden van validatielogica

Validatielogica wordt samengesteld met behulp van formules en u kunt de logica zo eenvoudig of zo complex maken als u nodig hebt. De validatie kan worden gebaseerd op de waarden van andere velden of de status van objecten. U kunt een foutbericht weergeven wanneer de validatie mislukt.

Als het veld met de toegepaste logica voldoet aan de gedefinieerde validatievoorwaarden wanneer een gebruiker het aangepaste formulier invult, wordt het veld gemarkeerd en wordt het foutbericht weergegeven.

U kunt validatielogica toepassen op de volgende veldtypen: tekst op één regel, alinea, vervolgkeuzelijst met één regel, vervolgkeuzelijst met meerdere selecties, externe zoekopdracht, typekop, datum, groep selectievakjes en keuzerondjes.

### Alleen eigenaar van project toestaan om &quot;Rush&quot; SLA te selecteren

In dit voorbeeld heeft een eenmalig vervolgkeuzeveld keuzemogelijkheden voor de SLA Standard - 14 dagen, Priority - 7 dagen en Rush - 2 dagen.

Validatie-expressie:

```
IF({ownerID}!=$$USER&&{DE:DV - Dropdown - Control Dates}="2",CONCAT("Only ",{owner}.{name}," may select X Rush"))
```

Wanneer iedereen die niet de projecteigenaar (met inbegrip van de systeembeheerder) is probeert om **X Rusland** te selecteren, wordt een fout getoond:

![&#x200B; slechts de projecteigenaar Claire Stevens kan X Rush &#x200B;](assets/sla-xrush.png) selecteren

### Datumvalidatie gebaseerd op keuze in vorige veld

Als u doorgaat met het SLA-voorbeeld, kunt u een datumveld toevoegen dat wordt gevalideerd op basis van de instellingen van het vorige vervolgkeuzeveld.

Validatie-expressie:

```
IF(
    DATEDIFF({DE:DV - Date - Dropdown SLA}, 
        ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates})) < 0, 
    CONCAT("Earliest: ", 
        ADDDAYS($$TODAY,{DE:DV - Dropdown - Control Dates})))
```

Als de gebruiker een datum selecteert die voorafgaat aan de toegestane datum, wordt in het bericht de vroegste datum weergegeven die ze kunnen selecteren:

![&#x200B; Geselecteerde datum is Maart 28 maar de vroegste beschikbare datum is 3 April &#x200B;](assets/date-validation-based-on-previous-choice.png)

### Minimum aantal tekens met de optie om te overschrijven

In dit voorbeeld wordt een minimum aantal tekens afgedwongen op een tekstveld, waarbij het aantal tekens wordt weergegeven. Bovendien wordt een afzonderlijk selectievakje ingesteld om de validatie voor het aantal tekens uit te schakelen.

Validatie-expressie:

```
IF({DE:DV - Override}!="Disable Validation"&&LEN({DE:DV - Text - Min Length})<"7",CONCAT(LEN({DE:DV - Text - Min Length})," characters / ",("7"-LEN({DE:DV - Text - Min Length}))," remaining"))
```

De handhaving van de bevestiging kan worden met voeten getreden door de controledoos te selecteren:

![&#x200B; doos van de Controle om bevestiging &#x200B;](assets/disable-validation-checkbox.png) onbruikbaar te maken

Er wordt een lopend aantal tekens in het tekstveld opgenomen:

![&#x200B; Aantal van het Karakter van 5 beschikbare, 2 resterende &#x200B;](assets/running-character-count.png)

### Een veld vergrendelen zodat alleen de eigenaar het kan bewerken

In dit voorbeeld kan een veld alleen worden bewerkt door de eigenaar van het project. Zelfs de systeembeheerder kan het veld niet bewerken.

Validatie-expressie:

```
IF({ownerID}!=$$USER,IF(ISBLANK({ownerID}),"Project Owner will provide this.",CONCAT("Only ",{owner}.{name}," can edit this.")))
```

Als een gebruiker die niet de projecteigenaar is op het gebied probeert te typen, zien zij een bericht verklarend dat slechts de projecteigenaar het gebied kan uitgeven.

![&#x200B; slechts Claire Stevens kan dit gebied &#x200B;](assets/only-project-owner-can-edit.png) uitgeven

### Met Typeahead kunnen waarden worden toegestaan of geweigerd op basis van andere veldwaarden

In dit voorbeeld staat of verwerpt een typekopveld dynamisch waarden toe op basis van de waarde die in een ander veld op het formulier is ingevoerd.

Validatie-expressie:

```
IF({DE:DV - Text - Budget}>"10000",
   IF({DE:DV - TA User - by Budget}.{role}!="Director","Requires Director Approver")
)
```

Als de waarde op het begrotingsgebied meer dan $10.000 is, dan slechts kunnen de gebruikers met een rol van de Directeur van typeahead worden geselecteerd, zelfs als er geen rolfilter op de typeahead configuratie wordt toegelaten.

![&#x200B; het bedrag van de Begroting vereist Directeur goedkeuring &#x200B;](assets/budget-director.png)

### Waarden die minder dan tien dagen na de ingangsdatum liggen, niet toestaan

In dit voorbeeld staat de validatie alleen waarden toe die 10 dagen in de toekomst vanaf de ingangsdatum zijn. De optie om de validatie te overschrijven (in een afzonderlijk veld voor selectievakjes) wordt ook opgenomen in de formule en het toestaan dat het datumveld leeg is.

Validatie-expressie:

```
IF({DE:DV - Override}!="Disable Validation"&&ISBLANK({DE:DV - Date - Deadline})!="true"&&{DE:DV - Date - Deadline}<ADDDAYS({entryDate},"10"),CONCAT("Earliest: ",ADDDAYS({entryDate},"10")))
```

Een waarde die minder dan 10 dagen na de ingangsdatum ligt, activeert de validatie:

![&#x200B; Geselecteerde datum is Maart 28 maar de vroegste beschikbare datum is 4 April &#x200B;](assets/earliest-deadline-date.png)

Een lege waarde activeert het validatiebericht niet:

![&#x200B; Lege waarde voor datum &#x200B;](assets/blank-date-allowed.png)

### Nauwkeurige/minimale/maximale selecties afdwingen in een veld met meerdere selecties

In dit voorbeeld vereist een veld voor meerdere selecties, zoals een groep selectievakjes, dat de gebruiker een bepaald aantal opties kiest.

Validatie-expressie (exact twee selecteren):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick exactly 2},","))!="2","Pick Exactly 2 Options")
```

Validatie-expressie (ten minste twee selecteren):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick at least 2},","))<"2","Pick at least 2 choices")
```

Validatie-expressie (maximaal twee opties selecteren):

```
IF({DE:DV - Override}!="Disable Validation"&&ARRAYLENGTH(ARRAY({DE:DV - Checkbox - Pick no more than 2},","))>"2","Pick no more than 2 choices")
```

De gebruiker ziet validatiefouten als hij of zij niet het juiste aantal opties selecteert.

![&#x200B; de foutenvoorbeelden van de Bevestiging &#x200B;](assets/min-max-selections.png)
