---
title: Berekende veldformules met AI Assistant herzien
content-type: reference
description: U kunt de Medewerker van AI gebruiken om fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden op te lossen.
author: Becky
feature: Get Started with Workfront
exl-id: 5f144a6f-5c2a-42fc-a961-ab9066432d93
source-git-commit: d261fd9eb9b8b649ebe413e35161543db1db8412
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Berekende veldformules genereren of herzien met AI Assistant

U kunt de Medewerker van AI gebruiken om formules te produceren die op een herinnering worden gebaseerd u verstrekt. U kunt fouten in uw ongeldige douaneuitdrukkingen op berekende gebieden ook oplossen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td><p>Nieuw: Premier of Ultimate</p>
       <p>of</p>
       <p>Huidig: Niet beschikbaar</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Niet beschikbaar</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een berekende veldexpressie genereren

## Een berekende veldexpressie herzien

Wanneer u het berekende veld maakt in de aangepaste formulierbuilder, verschijnt er een foutbericht onder het veld als de formule ongeldig is.

![ Ongeldige uitdrukkingsfout ](assets/invalid-expression.png)

Met AI Assistant kunt u de formule wijzigen in een geldige berekende veldexpressie.

Een ongeldige berekende veldexpressie herzien:

1. Klik het **pictogram AI van de Medewerker ![ AI Medewerker pictogram ](assets/ai-assistant-icon.png) dichtbij de hoger-juiste hoek van het scherm.**
1. Voer een vraag in het gebied met de vraag onder aan het deelvenster AI-assistent in, zoals:
   `Rewrite this formula to remove the invalid expression error`
1. Kopieer de ongeldige expressie uit de aangepaste formulierbuilder en plak deze in het promptiegebied.
1. Pers **gaat** binnen.

   AI Assistant kan enkele ogenblikken duren om de herziene formule te genereren, afhankelijk van hoe groot of complex de formule is.
1. Bekijk de herziene formule in het AI Hulppaneel.
1. (Optioneel) Kopieer de herziene formule uit het deelvenster AI-assistent en plak deze in het berekende veld in de aangepaste formulierbuilder.

>[!NOTE]
>
>Wij adviseren testend het berekende gebied om ervoor te zorgen dat het het verwachte resultaat terugwint.

Voor meer informatie over berekende gebieden in Workfront, zie [ berekende gebieden aan een vorm ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) toevoegen.
