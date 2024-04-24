---
title: Een formulier ordenen en een voorbeeld ervan bekijken met Form Designer
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier ordenen met de formulierontwerper.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 1bad65ff741cdd4273c07893044d42d6b8c826e0
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Een formulier organiseren en een voorbeeld bekijken met de formulierontwerper

U kunt een aangepast formulier organiseren met de formulierontwerper en er een voorbeeld van bekijken om te controleren of het correct is ingesteld.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>
   <p>Nieuw abonnement: standaard</p>
   <p>of</p>
   <p>Huidig plan: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

## Sectie-einde toevoegen

U kunt aangepaste velden en widgets in een aangepast formulier groeperen in secties met koppen. Dit is handig als u gebruikers die het formulier invullen, een geordende ervaring wilt laten zien. Ook, als u toegang tot bepaalde douanegebieden en widgets aan bepaalde gebruikers moet beperken, kunt u hen in een sectie plaatsen en dan toegang tot de sectie verlenen aan slechts die gebruikers.

Als u bijvoorbeeld gevoelige informatie wilt bijhouden die alleen systeembeheerders mogen weergeven of bewerken, kunt u een sectie-einde maken met de machtiging Alleen beheerder en de gevoelige velden in die sectie plaatsen.

De toegangsinstellingen die u voor een sectie selecteert, zijn rechtstreeks gekoppeld aan de machtigingen die gebruikers hebben voor het Workfront-object waaraan het aangepaste formulier is gekoppeld. U kunt een sectie verbergen of weergeven op basis van het feit of de gebruiker toegang heeft tot het object, een bijdrage levert aan dat object of dat object beheert. U kunt ook een sectie alleen instellen op Beheerder, zodat alleen gebruikers met een toegangsniveau van de systeembeheerder toegang hebben tot de sectie.

Zie voor informatie over machtigingen voor objecten [Overzicht van het delen van machtigingen voor objecten](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Zie voor informatie over aangepaste velden en widgets in aangepaste formulieren [Een formulier ontwerpen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Toegang voor een sectie in een aangepast formulier maken en configureren

1. Beginnen met het maken of bewerken van een aangepast formulier en velden toevoegen, zoals beschreven in [Een formulier ontwerpen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klikken **Sectie-einde** en sleep het naar de gewenste positie op het canvas.

1. In het juiste paneel, vorm de opties u voor de sectie wilt:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de sectie wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b>BELANGRIJK</b>: Gebruik geen speciale tekens in dit label. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ tekst als u aan gebruikers wilt uitleggen waarvoor de sectie is bedoeld. Dit wordt weergegeven onder het label van de sectie op het aangepaste formulier.</td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Add Logic</td> 
      <td>Use display logic to specify whether the section should display on the form, based on selections users make in multi-choice custom fields when they fill out the form. For more information, see <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Add display logic and skip logic to a custom form</a>.</td> 
     </tr> -->
     <tr> 
      <td role="rowheader"> <p>Toegang verlenen</p> </td> 
      <td> <p> Selecteer de machtigingen die gebruikers nodig hebben voor een object waaraan het aangepaste formulier is gekoppeld, om deze sectie weer te geven en de veldwaarden ervan te bewerken. 
       <p>De volgende machtigingen zijn beschikbaar onder <b>Gebruikers met deze toegang tot het object kunnen veldwaarden weergeven</b>:</p> 
         <ul>
          <li><strong>Weergave</strong>: Machtigingen voor het object weergeven</li>
          <li><p><b>Beperkte bewerking</b>: (Alleen beschikbaar als het object een project, taak, uitgave of gebruiker is):</p> 
          <p>Staat gebruikers toe om aan het voorwerp bij te dragen als het een project, een taak, of een kwestie is.</p>
          <p>Staat gebruikers toe om het profiel uit te geven of de profieltoestemming te bezitten aan het voorwerp als het een gebruiker is.</p></li> 
          <li><b>Bewerken</b>: Rechten voor het object beheren </li> 
          <li><b>Alleen beheerder</b>: Toegangsniveau voor systeembeheerder</li> 
         </ul> </li> 
        <p>De volgende machtigingen zijn beschikbaar onder <b>Gebruikers met deze toegang tot het object kunnen veldwaarden bewerken</b>: </p> 
         <ul> 
          <li> <p><b>Beperkte bewerking</b>: (Alleen beschikbaar als het object een project, taak, uitgave of gebruiker is):</p> 
           <p>Als het voorwerp een project, een taak, of een kwestie, deze toestemming gebruikers toestaat om aan het voorwerp bij te dragen</p>
          <p>Als het object een gebruiker is, kunnen gebruikers met deze machtiging het profiel bewerken of eigenaar zijn van de profielmachtiging voor het object.</p> 
          <li><b>Bewerken</b>: Rechten voor het object beheren </li> 
          <li><b>Alleen beheerder</b>: Toegangsniveau voor systeembeheerder</li> 
         </ul> </li> 
       </ul> 
       <p>Zie voor informatie over machtigingen voor objecten <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Overzicht van het delen van machtigingen voor objecten</a>.</p> 
       <p><b>OPMERKING</b>:  
       <ul> 
       <li> <p>Gebruikers zonder de machtigingen die u hier opgeeft, kunnen de aangepaste velden en widgets niet zien in de sectie. </p> <p>Dit is ook het geval als u de waarden van de velden in rapporten weergeeft of deze in berekende velden gebruikt in tekstmodusrapportage.</p> </li> 
       <li><p>Aangepaste formulieren aanvragen/uitgeven: als toegang weergeven nodig is om de velden in het sectie-einde te zien, maar beheerderstoegang nodig is om de velden te bewerken, zijn de sectie en alle velden niet zichtbaar voor niet-beheerders wanneer zij het formulier invullen. Zodra het verzoek is gecreeerd, dan kunnen de gebruikers met de toegang van de Mening de gebieden in de sectie bekijken.</p></li>
       <li> <p>Als u meerdere objecttypen aan uw formulier koppelt, kunt u de weergave- en bewerkingsmachtigingen wijzigen die in deze stappen beschikbaar zijn. Zie voor meer informatie <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Hoe meerdere objecttypen de machtigingen voor secties in een aangepast formulier kunnen beïnvloeden</a> in dit artikel.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Logica toevoegen</p></td> 
      <td><p>Gebruik weergaverelogica om op te geven of de sectie op het formulier moet worden weergegeven, op basis van selecties die gebruikers in meerkeuzevelden maken wanneer ze het formulier invullen.</p><p><strong>OPMERKING:</strong> Als op alle afzonderlijke velden onder een sectie-einde de weergavelogica is toegepast en alle velden als gevolg van de logica zijn verborgen, wordt de volledige sectie verborgen op het aangepaste formulier. Dit gebeurt ook als de weergaverelogica niet wordt toegepast op het sectie-einde.</p><p>Zie voor meer informatie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Weergavelogica toevoegen en logica overslaan met de formulierontwerper</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Sleep of voeg minstens één aangepast veld of widget toe aan de nieuwe sectie. Dit is vereist voordat u de sectie opslaat.

1. Klikken **Gereed**.

   >[!TIP]
   >
   >U kunt op **Toepassen** op elk gewenst moment tijdens het maken van een aangepast formulier om uw wijzigingen op te slaan en het formulier open te houden.

### Hoe meerdere objecttypen de machtigingen voor secties kunnen beïnvloeden {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

De beperkte machtiging Bewerken voor afbrekingen van aangepaste formuliersecties is alleen beschikbaar voor de typen projecten, taken, problemen en gebruikersobjecten.

Als u in een aangepast formulier met een sectie-einde dat is geconfigureerd met de machtiging Beperkte bewerking, een van de andere objecttypen aan het formulier toevoegt (Portfolio, Programma, Document, Bedrijf, Factureringsrecord, Iteratie, Kosten of Groep), wordt u gevraagd om over te schakelen naar de machtiging Bewerken. Deze is compatibel met zowel dat objecttype als de bestaande objecttypen op het formulier.

>[!INFO]
>
>**Voorbeeld:** In een douaneformulier verbonden aan het de objecten van het Project type, wordt een sectieonderbreking gevormd met de Beperkte Edit toestemming.
>
>U voegt het objecttype Portfolio aan het formulier toe. Dit betekent dat de optie Beperkte bewerking niet meer beschikbaar is voor het sectie-einde in het formulier.
>
>Een bericht op het scherm zet u ertoe aan om op de Edit toestemming over te schakelen, die het minste niveau van toestemmingen compatibel met zowel het de objecten van het Project type als het Portfolio objecten type is.


## Aangepaste velden en widgets in een aangepast formulier plaatsen


1. Beginnen met het maken of bewerken van een aangepast formulier, zoals beschreven in [Een formulier ontwerpen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Als u aangepaste velden en widgets op dezelfde rij wilt plaatsen, sleept u een naast elkaar totdat er een lijn tussen de velden en widgets wordt weergegeven.

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* U kunt de **Voorvertoning** in de rechterbovenhoek om een idee te krijgen van hoe de aangepaste velden en widgets in het formulier worden weergegeven.
>* Aangepaste velden en widgets geven het formulier mogelijk niet altijd op dezelfde manier weer, afhankelijk van hoeveel schermruimte beschikbaar is wanneer een gebruiker het formulier bekijkt. Het derde veld in een rij velden kan bijvoorbeeld omlopen naar de volgende rij velden als de horizontale ruimte beperkt is.

1. (Optioneel) Als u een aangepast veld of een aangepaste widget boven of onder een ander veld of een andere widget wilt plaatsen, sleept u het onder of boven totdat er een horizontale blauwe lijn tussen de items wordt weergegeven.

1. Als u de wijzigingen wilt opslaan, klikt u op **Toepassen**

   of

   Klikken **Opslaan en sluiten**.

## Een voorbeeld van een aangepast formulier bekijken

1. Beginnen met het maken of bewerken van een aangepast formulier en velden toevoegen, zoals beschreven in [Een formulier ontwerpen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klikken **Voorvertoning** in de rechterbovenhoek om te zien hoe het formulier eruitziet wanneer het wordt gebruikt, klikt u op **Voorvertoning beëindigen** om terug te keren naar het bewerken van het formulier.
