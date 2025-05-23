---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: een afbeelding weergeven in plaats van een tekenreeks in een kolom'
description: U kunt de naam van een object in een weergave vervangen door een afbeelding in de tekstmodus. U kunt ook een koppeling naar de afbeelding toevoegen waarmee het object dat wordt vervangen, kan worden geopend.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Weergave: een afbeelding weergeven in plaats van een tekenreeks in een kolom

<!--Audited: 11/2024-->

U kunt de naam van een object in een weergave vervangen door een afbeelding in de tekstmodus. U kunt ook een koppeling naar de afbeelding toevoegen waarmee het object dat wordt vervangen, kan worden geopend.

>[!NOTE]
>
>Afbeeldingen worden weergegeven in de werkelijke resolutie, dus probeer kleine afbeeldingen te gebruiken.

![ vervang projectnaam met beeld en verbinding ](assets/replace-project-name-with-image-and-link-350x125.png)

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> 
    <p>Nieuw:</p>
   <ul><li><p>Medewerker om een filter te wijzigen </p></li>
   <li><p>Standaard voor het wijzigen van een rapport</p></li> </ul>

<p>Huidige:</p>
   <ul><li><p>Verzoek om een filter te wijzigen </p></li>
   <li><p>Plan om een rapport te wijzigen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een filter te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voorbeeld: vervang de naam van een project in een projectweergave door een afbeelding:

1. Upload een afbeelding naar een website of server buiten Adobe Workfront. U moet de afbeelding kunnen openen met uw webbrowser.

   >[!TIP]
   >
   >* Elk browsertype is anders, maar alle browsers kunnen URL&#39;s weergeven.
   >* Gebruik geen afbeeldingen die naar Workfront zijn geüpload. Aangezien afbeeldingen die in Workfront zijn opgeslagen, niet openbaar beschikbaar zijn en een toegangstoets hebben die na een bepaalde periode vervalt, worden deze afbeeldingen niet meer in de weergave weergegeven.
   >* Een afbeelding die op uw computer is opgeslagen, heeft geen inherente URL. Zoek een site die beeldhosting biedt en host uw afbeelding daar. Uw organisatie heeft een dergelijke site mogelijk al.

1. Ga in uw webbrowser naar de afbeelding die u hebt opgeslagen.
1. Verkrijg URL van het beeld door het volgende te doen:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Klik met de rechtermuisknop en selecteer **het beeldplaats van het Exemplaar**, of **krijg verbinding**, afhankelijk van uw browser. U hebt nu de URL voor die specifieke afbeelding en kunt deze plakken vanaf het klembord.
   1. Zorg ervoor dat iedereen met die verbinding toestemmingen heeft om het beeld te bekijken door enkel naar de verbinding te gaan en zij hebben geen login nodig om tot het toegang te hebben.

1. Ga naar een project, klik **Meer** menu ![ Meer pictogram ](assets/more-icon-45x33.png) naast de naam van het project, dan klik **uitgeven**.

1. Op het **URL** gebied, voeg de verbinding aan het beeld toe.
1. Ga naar een projectmening in een lijst van projecten.
1. Klik het **drop-down menu van de Mening**, dan klik **Nieuwe Mening**.
1. Klik de kopbal van de kolom voor de **Naam van het Project**, dan klik **Schakelaar aan de Wijze van de Tekst**.

1. Voeg de volgende code aan de kolom aan de bestaande code toe:

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Klik **Gedaan** > **sparen Mening**.
Het geselecteerde beeld vervangt de Naam van het Project in de projectweergave en het beeld is een verbinding aan het project.
