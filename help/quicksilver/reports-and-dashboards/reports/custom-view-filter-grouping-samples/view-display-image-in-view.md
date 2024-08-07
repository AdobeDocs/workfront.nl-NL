---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Weergave: een afbeelding weergeven in plaats van een tekenreeks in een kolom'
description: U kunt de naam van een object in een weergave vervangen door een afbeelding in de tekstmodus. U kunt ook een koppeling naar de afbeelding toevoegen waarmee het object dat wordt vervangen, kan worden geopend.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Weergave: een afbeelding weergeven in plaats van een tekenreeks in een kolom

U kunt de naam van een object in een weergave vervangen door een afbeelding in de tekstmodus. U kunt ook een koppeling naar de afbeelding toevoegen waarmee het object dat wordt vervangen, kan worden geopend.

>[!NOTE]
>
>Afbeeldingen worden weergegeven in de werkelijke resolutie, dus probeer kleine afbeeldingen te gebruiken.

![](assets/replace-project-name-with-image-and-link-350x125.png)

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Verzoek om een weergave te wijzigen </p>
   <p>Plan om een rapport te wijzigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een rapport te wijzigen</p> <p>Toegang tot filters, weergaven en groepen bewerken om een weergave te wijzigen</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen beheren voor een rapport</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

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

1. Ga naar een project, klik **Meer** menu ![](assets/more-icon-45x33.png) naast de naam van het project, dan klik **uitgeven**.

1. Op het **URL** gebied, voeg de verbinding aan het beeld toe.
1. Navigeer naar een projectweergave in een lijst of rapport en pas de weergave aan.
1. Klik de kopbal van de kolom voor de **Naam van het Project**, dan klik **Schakelaar aan de Wijze van de Tekst**.

1. Voeg de volgende code aan de kolom aan de bestaande code toe:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   Het geselecteerde beeld vervangt de Naam van het Project in de projectweergave en het beeld is een verbinding aan het project.

1. Klik **sparen Mening**.
