---
title: Weergavelogica toevoegen en logica overslaan op een formulier
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5f5dbeb5-b974-489c-8f4d-ebaa00f5e5ba
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '1318'
ht-degree: 0%

---

# Weergavelogica toevoegen en logica overslaan naar een formulier

U kunt bepalen welke secties van een aangepast formulier moeten worden weergegeven of overgeslagen op basis van de keuzes die een gebruiker maakt bij het invullen.

>[!NOTE]
>
>De logica geldt alleen binnen één formulier en kan niet worden gebaseerd op selecties vanuit een ander formulier.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-plan </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>Administratieve toegang tot aangepaste formulieren </td> 
  </tr>  
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Logische pictogrammen weergeven en overslaan

Op aangepaste formulieren worden pictogrammen weergegeven om aan te geven welke logica wordt toegepast op bepaalde velden. Pictogrammen op een veld in de formulierontwerper geven aan dat logica wordt toegepast op het veld.

| Pictogram | Locatie in veld in formulierontwerper | Definitie |
|--- |--- |--- |
| ![ logica van de Vertoning voor doelgebied ](assets/display-logic-bottom-left.png) | Linksonder | Het veld is het doelveld voor de weergavelogica. Als een specifieke selectie is aangebracht op het formulier, wordt dit veld weergegeven. |
| ![ bepalen het pictogram van de vertoningslogica ](assets/display-logic-bottom-right.png) | Rechtsonder | Het veld definieert weergavelogica. Een specifieke selectie of waarde in dit veld geeft het doelveld weer. |
| ![ Skip logica voor doelgebied ](assets/skip-logic-bottom-left.png) | Linksonder | Het veld is het doelveld voor overslaan van logica. Als een specifieke selectie wordt gemaakt op het formulier, slaat het formulier door naar dit veld en worden de tussenliggende velden verborgen. |
| ![ bepaalt overslaan logisch pictogram ](assets/skip-logic-bottom-right.png) | Rechtsonder | In dit veld wordt de logica voor overslaan gedefinieerd. Een specifieke selectie of waarde in dit veld slaat andere velden over en gaat rechtstreeks naar het doelveld. |

![ Logische pictogrammen ](assets/logic-icons-3.png)

Selecteer een veld met toegepaste logica om de bestaande logische regels in de veldinstellingen weer te geven.

![ Logische regels ](assets/form-designer-view-only-logic.png)

## Overwegingen bij het gebruik van weergavelogica en het overslaan van logica

* Als u weergavelogica wilt toevoegen aan een aangepast veld, een widget of een sectie-einde, moet ten minste één meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes) vóór dit veld op het formulier worden geplaatst.
Voor informatie over douanegebieden en widgets in douanevormen, zie [ een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.
* U kunt geen logica overslaan toevoegen aan een widget of sectie-einde. U kunt het alleen toevoegen aan een veld met meerdere keuzen (keuzerondjes, vervolgkeuzelijst of selectievakjes).
* U kunt geen weergave- of overslaan-logica toepassen om de keuzes van een veld met meerdere opties weer te geven of te verbergen. U kunt bijvoorbeeld geen beperkingen instellen voor de opties die worden weergegeven voor een vervolgkeuzelijst, een CheckBox-groep of een keuzerondje op basis van de weergave of de logica van een ander veld overslaan.
* U kunt zowel weergavelogica als logica overslaan aan een aangepast veld toevoegen als het volgende geldt voor het aangepaste veld:

   * Het is een meerkeuzeveld (keuzerondjes, vervolgkeuzelijst of selectievakjes)
   * Voorafgegaan door een veld met meerdere keuzen
   * Het wordt gevolgd door een ander aangepast veld

* Wanneer u formulieren kopieert met logica voor weergave of overslaan, wordt de logica gekopieerd naar het nieuwe aangepaste formulier.
* Wanneer u objecten bulksgewijs bewerkt, worden alle aangepaste velden weergegeven in het vak Objecten bewerken, inclusief de overgeslagen of verborgen velden.
* Houd rekening met het volgende wanneer u een weergaveregel voor een aangepast formulier maakt:

   * Aangepaste velden die niet zijn opgenomen in een logische weergave-instructie, worden standaard weergegeven op een aangepast formulier.
   * U kunt logische instructies voor weergave op meerdere velden maken.
   * Als voor alle velden onder een sectie-einde een weergavelogica is toegepast en alle velden zijn verborgen als gevolg van de logica, wordt de volledige sectie verborgen op het aangepaste formulier.

## Weergavelogica toevoegen aan een aangepast formulier

De logica van de vertoning bepaalt welke douanevelden op de vorm verschijnen wanneer de gebruiker een specifieke waarde op een meerkeuzeveld selecteert. De logica wordt toegevoegd aan het doelveld, dat alleen wordt weergegeven wanneer de waarde is geselecteerd.

{{step-1-to-setup}}

1. Klik **Aangepaste Forms**.
1. Maak een nieuw aangepast formulier of open een bestaand formulier. Zie [ een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) voor details creëren.
1. Voeg zo nodig velden toe aan het formulier. Er moet ten minste één meerkeuzeveld (keuzerondje, vervolgkeuzelijst of selectievakje) worden geplaatst vóór het doelveld dat wordt weergegeven.
1. Selecteer het doelgebied en klik **voegt Logica** op de lagere linkerzijde van het scherm toe.
1. Selecteer de **Logische tabel van de Vertoning**.
1. Klik **toevoegen de Regel van de Vertoning** op de logische bouwer.

   ![ de logische bouwer van de Vertoning ](assets/custom-form-logic-builder-display-blank.png)

1. Voer de onderstaande stappen in de builder uit om de logische instructie te maken.

   1. De eerste optie is het kiezen van het definiërende veld. Dit is het veld met de selectiewaarde waarin het doel wordt weergegeven. Het moet een meerkeuzeveld zijn.
   1. De tweede optie is het kiezen van de selectiewaarde. Alleen de waarden die al voor dat veld zijn gedefinieerd, zijn beschikbaar.
   1. De derde optie is **Geselecteerd** of **niet Geselecteerd**. Het kiezen van **Geselecteerde** betekent dat wanneer de waarde wordt geselecteerd, het doelgebied wordt getoond. Het kiezen van **niet Geselecteerde** betekent dat wanneer een andere waarde op het definiërende gebied wordt geselecteerd, het doelgebied wordt getoond.
   1. Om een **en** regel aan de logische verklaring toe te voegen, klik **voegt Regel** direct onder de regel toe u enkel creeerde. Volg de zelfde herinneringen om de regel te bouwen. Aan alle regels en moet worden voldaan opdat het doelgebied wordt getoond.

      ![ de logische bouwer van de Vertoning ](assets/custom-form-logic-builder-display1.png)

   1. Om een **of** regel aan de logische verklaring toe te voegen, klik **voegt Regel** dichtbij de bodem van de logische bouwer toe. Dan, klik **voeg Regel** binnen toe of gebied en volg de zelfde herinneringen om de regel te bouwen. Wanneer één of regel wordt ontmoet, wordt het doelgebied getoond.

1. Klik **sparen** wanneer u klaar bent bouwend de logische verklaring.

   De pictogrammen voor de weergavelogica worden toegevoegd aan het doelveld en het definiërende veld in de formulierontwerper.

## Logica voor overslaan toevoegen aan een aangepast formulier

De logica Overslaan definieert aangepaste formuliervelden die worden overgeslagen wanneer de gebruiker een specifieke waarde in een veld met meerdere keuzes selecteert. Overgeslagen velden worden verborgen op het formulier. De logica wordt toegepast op het definiërende veld waar de selectie is gemaakt, niet op de velden die worden overgeslagen.

{{step-1-to-setup}}

1. Klik **Aangepaste Forms**.
1. Maak een nieuw aangepast formulier of open een bestaand formulier. Zie [ een douanevorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) voor details creëren.
1. Voeg zo nodig velden toe aan het formulier. Het definiërende gebied voor overslaan logica moet een veelvoudige keuzeveld (radioknoop, dropdown, of controledoos) zijn.
1. Selecteer het definiërende gebied en klik **voegt Logica** op de lagere linkerzijde van het scherm toe.
1. Selecteer **Skip Logische** tabel.
1. Klik **toevoegen Skip Regel** op de logische bouwer.

   ![ Skip logica bouwer ](assets/custom-form-logic-builder-skip-blank.png)

1. Voer de onderstaande stappen in de builder uit om de logische instructie te maken.

   1. Het definiërende gebied wordt getoond op de bouwer. Het is het veld waarop u de logica voor overslaan hebt geselecteerd.
   1. De eerste optie is het kiezen van de selectiewaarde. Alleen de waarden die al voor het veld zijn gedefinieerd, zijn beschikbaar.
   1. De tweede optie is **Geselecteerd** of **niet Geselecteerd**. Het kiezen van **Geselecteerde** betekent dat wanneer de waarde wordt geselecteerd, het doelgebied wordt getoond en de gebieden binnen tussen worden overgeslagen. Het kiezen van **niet Geselecteerde** betekent dat wanneer een andere waarde op het definiërende gebied wordt geselecteerd, het doelgebied wordt getoond en de gebieden binnen tussen worden overgeslagen.
   1. De derde optie is het doelveld, of waar u wilt overslaan. Selecteer een gebiedsnaam of **Eind van vorm**. Mogelijk moet u eerst op het woord &quot;leeg&quot; klikken voordat u een optie selecteert.

      ![ Skip logica bouwer ](assets/custom-form-logic-builder-skip1.png)

   1. Om een **of** regel aan de logische verklaring toe te voegen, klik **voegt Regel** dichtbij de bodem van de logische bouwer toe. Selecteer vervolgens de opties volgens dezelfde aanwijzingen om de regel te maken. Wanneer één **of** regel wordt ontmoet, wordt het doelgebied getoond.

1. Klik **sparen** wanneer u klaar bent bouwend de logische verklaring.

   De pictogrammen voor logicaoverslaan worden toegevoegd aan het doelveld en het definiërende veld in de formulierontwerper.


