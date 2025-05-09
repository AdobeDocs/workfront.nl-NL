---
title: Overzicht van licentietype bij gebruik van Adobe Workfront-planning
description: De toegang tot Adobe Workfront Planning is afhankelijk van het type licentie en van de machtigingen tot objecten. Niet alle gebruikers in de organisatie hebben de zelfde toegang en de toestemmingen om de Planning van Adobe Workfront te gebruiken. In dit artikel worden de toegangsniveaus beschreven die gebruikers kunnen hebben voor Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---


# Overzicht van licentietype bij gebruik van Adobe Workfront Planning

<span class="preview"> de benadrukte informatie op deze pagina verwijst naar functionaliteit nog niet algemeen beschikbaar. Deze optie is alleen beschikbaar in de voorvertoningsomgeving voor alle klanten. Na de maandelijkse versies aan Productie, zijn de zelfde eigenschappen ook beschikbaar in het milieu van de Productie voor klanten die snelle versies toeliet. </span>

<span class="preview"> voor informatie over snelle versies, zie [ snelle versies voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) toelaten of onbruikbaar maken. </span>

{{planning-important-intro}}

Het Adobe Workfront-licentietype werkt in combinatie met uw Adobe Workfront-planningsbevoegdheden en geeft de volgende toegang:

* De mening, draagt, of beheert werkruimten <span class="preview"> of recordtypes </span> bij
* Weergaven weergeven of beheren.

Voor informatie over toestemmingen aan voorwerpen in de Planning van Workfront, zie [ Overzicht van het delen van toestemmingen in de Planning van Adobe Workfront ](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Voor informatie over toegang tot de Planning van Workfront, zie [ Adobe die toegangsoverzicht van de Planning ](/help/quicksilver/planning/access/access-overview.md) plant.

## De relatie tussen Workfront-licentietypen en Workfront-planningsmachtigingen

In de onderstaande tabel wordt de relatie beschreven tussen het licentietype van een gebruiker in Adobe Workfront en het machtigingsniveau dat u aan deze gebruiker kunt toekennen aan Adobe Workfront-planningsobjecten op basis van die licentie.

Het verlenen van gebruikerstoestemmingen aan een werkruimte verleent hen ook toestemmingen om types, verslagen, en gebieden te registreren.

U moet gebruikers afzonderlijke toestemmingen aan meningen, naast degenen verlenen zij voor werkruimten hebben, om tot meningen toegang te hebben en te leiden.

<div class="preview">

Houd rekening met het volgende wanneer u werkt met bevoegdheden voor recordtypen:

* Gebruikers nemen automatisch machtigingen voor recordtypen over van werkruimten.
* Wanneer een gebruiker beheerdersmachtigingen voor een werkruimte heeft, hebben deze gebruikers geen minder toegang tot een recordtype.
* Gebruikers kunnen niet meer machtigingen voor een recordtype hebben dan voor de werkruimte waartoe het recordtype behoort.
* Als u gebruikersmachtigingen verwijdert van een recordtype, wordt de toegang tot de weergave van de gebruiker tot alle recordtypen in de werkruimte niet verwijderd, omdat hun machtigingen voor de werkruimte dan niet worden verwijderd.

</div>


| Adobe Workfront-licentietype* | Hoogste machtigingen toegestaan in Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standaard | <p>Gebruikers kunnen werkruimten <span class="preview"> , recordtypen </span> en weergaven beheren. Ze kunnen werkruimten, recordtypen, records, velden en weergaven maken, bewerken of verwijderen.</p> <br> <p>Systeembeheerders hebben beheermachtigingen voor alle werkruimten, inclusief de werkruimten die ze niet hebben gemaakt.</p> |
| Licht of medewerker | <p>De gebruikers kunnen de werkruimten bekijken die met hen, evenals de verslagtypes, verslagen, en gebieden van die werkruimten worden gedeeld.</p> <br> <p>Gebruikers kunnen de weergaven bekijken die met hen worden gedeeld, maar ze kunnen hun eigen weergaven niet maken. </p><br> <p>Gebruikers kunnen geen werkruimten, recordtypen, records of velden maken, bewerken of verwijderen.</p> |

*Workfront Planning is niet beschikbaar voor verouderde Workfront-licenties.
Voor meer informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


### Licentietypen en machtigingen voor werkruimten en recordtypen

Slechts kunnen de gebruikers met een Standaardvergunning bijdragen of hebben toestemmingen aan werkruimten <span class="preview"> en verslagtypes </span> leiden. Contribute en leidt toestemmingen aan werkruimten <span class="preview"> en recordtypes </span> ook over naar verslagen en gebieden.

Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor werkruimten <span class="preview"> en recordtypen </span> die met hen worden gedeeld, en voor hun records en velden.

Systeembeheerders kunnen alle werkruimten in het systeem weergeven, inclusief de werkruimten die ze niet hebben gemaakt.

>[!INFO]
>
>**VOORBEELD:**
>
>Medewerkers of gebruikers met een lichtlicentie kunnen geen bijdrage leveren aan werkruimten en hun objecten of deze beheren.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om bij te dragen aan een werkruimte of een werkruimte te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![ Bevoegdheden grayed uit voor contributorgebruiker op werkruimte ](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Typen licenties en machtigingen voor weergaven

Alleen gebruikers met een standaardlicentie kunnen beheermachtigingen voor weergaven hebben. Gebruikers met alle andere licentietypen kunnen weergavemachtigingen hebben voor weergaven die met hen worden gedeeld.

>[!INFO]
>
>**VOORBEELD:**
>
>Medewerkers of gebruikers met een lichtlicentie kunnen geen weergaven beheren. Ze kunnen tijdelijke filters, sorteren of groeperingen toepassen op weergaven waartoe ze toegang hebben.
>
>Er is een aanwijzing in het deelvak dat gebruikers geen machtigingen kunnen worden verleend om een weergave te beheren wanneer zij een licentie op een lager niveau hebben, omdat deze machtigingsniveaus grijs worden weergegeven.
>
>![ Bevoegdheden grayed uit voor lichte gebruiker op meningsaandeel ](assets/permissions-grayed-out-for-light-user.png)
