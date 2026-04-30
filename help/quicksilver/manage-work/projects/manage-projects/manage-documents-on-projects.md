---
product-area: projects
navigation-topic: manage-projects
title: Overzicht documentbeheer voor projecten en verwante objecten
description: Afhankelijk van of uw Workfront-beheerder ervoor kiest uw opslagvoorkeur standaard in te stellen, kunt u documenten opslaan op verouderde Workfront-opslagsystemen of op Adobe Enterprise-opslagsystemen. In dit artikel wordt beschreven hoe u documenten voor projecten, portfolio's, programma's, sjablonen, taken en problemen kunt beheren.
author: Alina
feature: Work Management
exl-id: 5623157e-946e-4475-9df3-b1888a2a0934
source-git-commit: 5c4ffeabf710374b14a2335b47342be4c393a7c8
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Overzicht van documentbeheer voor projecten en verwante objecten

Uw Adobe Workfront-beheerder kan de standaardinstelling voor de opslagvoorkeur van uw organisatie definiëren om aan te geven waar documenten in Workfront moeten worden opgeslagen.

De Workfront-beheerder kan een van de volgende opties kiezen:

* Workfront-opslag
* Adobe Enterprise-opslag

Met deze voorkeur kunt u documenten die aan Workfront-objecten zijn gekoppeld, automatisch opslaan op een van de beschikbare opslaglocaties.

>[!IMPORTANT]
>
>Niet alle klanten hebben toegang tot zowel Workfront- als Adobe-opslag. Sommige klanten hebben alleen toegang tot Workfront en andere hebben standaard alleen toegang tot Adobe Enterprise-opslag. Er is geen configuratie nodig voor klanten zonder toegang tot Workfront-opslag.

De Workfront-beheerder kan het volgende doen:

* Kies een van de twee opslagopties als standaard voor uw organisatie
* U kunt kiezen welke opslag u wilt gebruiken wanneer u een van de volgende objecten maakt:

   * Projecten
   * Portfolio&#39;s
   * Sjablonen

Voor informatie over het plaatsen van opslagvoorkeur voor Workfront, zie [ de ondernemingsopslag van Adobe voor uw organisatie ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md) toelaten.

In dit artikel wordt beschreven hoe u documenten voor projecten, portfolio&#39;s, programma&#39;s, taken, uitgaven, sjablonen en sjabloontaken kunt beheren.

<!--

Not sure we need these since this became an overview article: 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Light or higher</p>
   <p>Review or higher</p>
   
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to the objects you want to add documents to:</p>
   <ul><li>Projects</li>
   <li>Portfolios</li>
<li>Programs</li>
<li>Templates</li> 
<li>Tasks</li> 
<li>Issues</li> </ul>  
   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the objects you want to add documents to:</p>

<ul><li>A project</li>
   <li>A portfolio</li>
<li>A program</li>
<li>A template</li> 
<li>A task</li> 
<li>An issue</li> </ul>    
   
</td> 
  </tr> 
 </tbody> 
</table>

*For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

-->

## Overzicht van documentopslag

Klanten hebben mogelijk toegang tot een van de volgende opslagmogelijkheden voor documenten:

* Alleen Workfront-opslag. Het gedeelte Opslagvoorkeuren in Systeemvoorkeuren bestaat niet.
* Alleen Adobe Enterprise-opslag. Het gedeelte Opslagvoorkeuren in Systeemvoorkeuren bestaat niet.
* Zowel Workfront Storage als Adobe Enterprise storage. De Workfront-beheerder kan kiezen uit:

   * Hiermee selecteert u een standaardopslagomgeving voor de verwerking van documenten in de toekomst.
   * Hiermee kunnen gebruikers kiezen welke opslag ze kiezen wanneer ze de volgende objecten maken:

      * Projecten
      * Portfolio&#39;s
      * Sjablonen

  >[!NOTE]
  >
  >* De taken en de kwesties erven het type van opslag van het project.
  >* Sjabloontaken nemen het type opslag over van de sjabloon
  >* De programma&#39;s erven het type van opslag van de portefeuille.


Documenten die zijn opgeslagen op objecten in Workfront-opslag, worden anders beheerd dan opslagruimten in Adobe Enterprise Storage.

Voor meer informatie, zie [ overzicht van de ondernemingsopslag van Adobe ](/help/quicksilver/review-and-approve-work/esm-overview.md).

In de volgende secties wordt beschreven hoe documentopslag werkt voor Workfront-objecten wanneer zowel Workfront- als Adobe-opslagopties voor ondernemingen zijn ingesteld.

### Documentbeheer voor projecten

Houd rekening met het volgende wanneer u met projecten werkt:

* Als u een Adobe Enterprise-Storage-project maakt, maakt Workfront een map in de sectie Documenten van het project waarin documenten worden opgeslagen. De mapnaam is dezelfde naam als het project. U kunt de map niet verwijderen of handmatig hernoemen. De naam van de map wordt gewijzigd als u de naam van het project wijzigt zodat deze overeenkomt met de nieuwe naam van het project.
* Wanneer u een opslagproject voor Adobe-Enterprise maakt of verplaatst naar een verouderd Workfront-opslagportfolio of -programma, wordt het portfolio of programma automatisch omgezet naar een Adobe Enterprise-storage-object.
* U kunt geen Workfront-opslagproject maken voor een Adobe-portfolio of -programma voor bedrijfsopslag.

### Documentbeheer voor portfolio&#39;s

Houd rekening met het volgende wanneer u met portfolio&#39;s werkt:

* Als u een Adobe-portfolio voor bedrijfsopslag maakt, maakt Workfront een map in de sectie Documenten van het portfolio waarin documenten worden opgeslagen. De mapnaam is dezelfde naam als het portfolio. U kunt de map niet verwijderen of handmatig hernoemen. De naam van de map wordt gewijzigd als u de naam van het portfolio wijzigt zodat deze overeenkomt met de nieuwe naam van het portfolio.
* Wanneer u een opslagproject voor Adobe-Enterprise maakt of verplaatst naar een verouderd Workfront-opslagportfolio, wordt het portfolio automatisch geconverteerd naar een Adobe Enterprise-storage-object.
* Als er eerder documenten waren gekoppeld aan het omgezette portfolio, blijven deze opgeslagen in Workfront-opslag. Nieuwe documenten worden ook opgeslagen in Workfront.
* Als er geen documenten in Workfront-opslag zijn gekoppeld aan het geconverteerde portfolio, worden nieuwe documenten opgeslagen in Adobe Enterprise storage.

### Documentbeheer voor programma&#39;s

Houd rekening met het volgende wanneer u werkt met programma&#39;s:

* Als u een Adobe Enterprise-Storage-programma maakt, maakt Workfront een map in de sectie Documenten van het programma waarin documenten worden opgeslagen. De mapnaam is dezelfde naam als het programma. U kunt de map niet verwijderen of handmatig hernoemen. De naam van de map wordt gewijzigd als u de naam van het programma wijzigt, zodat deze overeenkomt met de nieuwe naam van het programma.
* Wanneer u een opslagproject voor Adobe-Enterprise maakt of verplaatst naar een verouderd Workfront-opslagportfolio, wordt het portfolio automatisch geconverteerd naar een Adobe Enterprise-storage-object.
* Als er eerder documenten waren gekoppeld aan het omgezette programma, blijven deze opgeslagen in Workfront-opslag. Nieuwe documenten worden ook opgeslagen in Workfront.
* Als voor het omgezette programma geen documenten in Workfront-opslag zijn gekoppeld, worden nieuwe documenten opgeslagen in Adobe Enterprise storage.

### Documentbeheer voor taken

Houd rekening met het volgende wanneer u met taken werkt:

* De taken erven het opslagtype van projecten.
* Wanneer u een document uploadt naar een taak in een Adobe-opslagproject, maakt Workfront automatisch een map in de sectie Documenten van de taak. De mapnaam is hetzelfde als de taak.
* U kunt de naam van de documentmap wijzigen en deze verwijderen uit de Adobe-taak voor bedrijfsopslag, waarmee ook de documenten in de map worden verwijderd. Nadat u nieuwe documenten aan de taak hebt toegevoegd, wordt de map automatisch opnieuw gemaakt. Verwijderde documenten worden niet opnieuw in de map geplaatst.
* Voor Adobe-projecten voor bedrijfsopslag wordt de documentmap op een taak weergegeven als een submap in de documentenmap die automatisch voor het project wordt gemaakt.
* U kunt een taak niet kopiëren of verplaatsen van een Workfront-opslagproject naar een Adobe-opslagproject. Het omgekeerde is ook niet mogelijk.

### Documentbeheer voor problemen

Houd rekening met het volgende wanneer u met problemen werkt:

* De kwesties erven het opslagtype van projecten.
* Wanneer u een document uploadt naar een uitgave in een Adobe-opslagproject, maakt Workfront automatisch een map in de sectie Documenten van de uitgave. De mapnaam is gelijk aan de naam van de uitgave.
* U kunt de naam van de documentmap wijzigen en deze verwijderen uit de Adobe Enterprise-storage-uitgave. Hierdoor worden ook de documenten in de map verwijderd. Nadat u nieuwe documenten aan de uitgave hebt toegevoegd, wordt de map automatisch opnieuw gemaakt. Verwijderde documenten worden niet opnieuw in de map geplaatst.
* Voor Adobe-projecten voor bedrijfsopslag wordt de documentmap op een uitgave weergegeven als een submap in de documentenmap die automatisch voor het project wordt gemaakt.
* U kunt een uitgave niet kopiëren of verplaatsen van een Workfront-opslagproject naar een Adobe-opslagproject. Het omgekeerde is ook niet mogelijk.

### Documentbeheer voor projectsjablonen

Houd rekening met het volgende wanneer u werkt met sjablonen:

* Als u een Adobe-sjabloon voor bedrijfsopslag maakt, maakt Workfront een map in de sectie Documenten van de sjabloon waarin documenten worden opgeslagen. De mapnaam is dezelfde naam als het programma. U kunt de map niet verwijderen of handmatig hernoemen. De naam van de map wordt gewijzigd als u de naam van de sjabloon wijzigt, zodat deze overeenkomt met de nieuwe naam van de sjabloon.
* U kunt een Workfront-opslagsjabloon gebruiken om Workfront-opslagprojecten te maken; u kunt een Adobe-opslagsjabloon gebruiken om een Adobe-opslagproject te maken.
* U kunt een Workfront-opslagmalplaatje aan een Adobe-opslagproject vastmaken en dit verandert niet de opslagplaats van het project.
* U kunt een Adobe-opslagmalplaatje aan een Workfront-opslagproject vastmaken en dit verandert niet de opslagplaats voor het project.

### Documentbeheer voor sjabloontaken

Houd rekening met het volgende wanneer u met sjabloontaken werkt:

* Sjabloontaken nemen het opslagtype over van sjablonen.
* Als u een document uploadt naar een sjabloontaak op een Adobe-opslagsjabloon, maakt Workfront automatisch een map in de sectie Documenten van de sjabloontaak. De mapnaam is gelijk aan de sjabloontaak.
* U kunt de naam van de documentmap wijzigen en deze verwijderen uit de Adobe-sjabloontaak voor bedrijfsopslag, waarmee ook de documenten in de map worden verwijderd. Nadat u nieuwe documenten aan de sjabloontaak hebt toegevoegd, wordt de map automatisch opnieuw gemaakt. Verwijderde documenten worden niet opnieuw in de map geplaatst.
* Voor Adobe-sjablonen voor bedrijfsopslag wordt de documentmap op een sjabloontaak weergegeven als een submap in de documentmap die automatisch voor de sjabloon wordt gemaakt.
* U kunt een sjabloontaak niet kopiëren of verplaatsen van een Workfront-opslagsjabloon naar een Adobe-opslagsjabloon. Het omgekeerde is ook niet mogelijk.
* Als u een document koppelt aan een uitgave die u verzendt naar een aanvraagwachtrij die is gekoppeld aan Adobe-opslag, wordt een map gemaakt voor elke verzonden uitgave waarin de documenten zijn opgeslagen. De map wordt ook als een submap toegevoegd aan de automatisch gemaakte projectmap in de aanvraagwachtrij.
