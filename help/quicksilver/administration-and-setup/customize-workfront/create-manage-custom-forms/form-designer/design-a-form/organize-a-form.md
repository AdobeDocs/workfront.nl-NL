---
title: Een formulier ordenen en een voorbeeld ervan bekijken
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier organiseren met het formulier Designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '1318'
ht-degree: 0%

---

# Een formulier ordenen en een voorbeeld ervan bekijken

U kunt een aangepast formulier organiseren met de formulierontwerper en er een voorbeeld van bekijken om te controleren of het correct is ingesteld.

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

## Sectie-einde toevoegen

U kunt aangepaste velden en widgets in een aangepast formulier groeperen in secties met koppen. Dit is handig als u gebruikers die het formulier invullen, een geordende ervaring wilt laten zien. Ook, als u toegang tot bepaalde douanegebieden en widgets aan bepaalde gebruikers moet beperken, kunt u hen in een sectie plaatsen en dan toegang tot de sectie verlenen aan slechts die gebruikers.

Als u bijvoorbeeld gevoelige informatie wilt bijhouden die alleen systeembeheerders mogen weergeven of bewerken, kunt u een sectie-einde maken met de machtiging Alleen beheerder en de gevoelige velden in die sectie plaatsen.

De toegangsinstellingen die u voor een sectie selecteert, zijn rechtstreeks gekoppeld aan de machtigingen die gebruikers hebben voor het Workfront-object waaraan het aangepaste formulier is gekoppeld. U kunt een sectie verbergen of weergeven op basis van het feit of de gebruiker toegang heeft tot het object, een bijdrage levert aan dat object of dat object beheert. U kunt ook een sectie alleen instellen op Beheerder, zodat alleen gebruikers met een toegangsniveau van de systeembeheerder toegang hebben tot de sectie.

Voor informatie over toestemmingen op voorwerpen, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Voor informatie over douanegebieden en widgets in douanevormen, zie [&#x200B; een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

### Toegang voor een sectie in een aangepast formulier maken en configureren

1. Begin creërend of het uitgeven van een douanevorm en het toevoegen van gebieden, zoals die in [&#x200B; worden beschreven creeer een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klik **de onderbreking van de Sectie** en sleep het in de gewenste positie op het canvas.

1. In het juiste paneel, vorm de opties u voor de sectie wilt:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Label</td> 
      <td> <p>(Vereist) Typ een beschrijvend label dat boven de sectie wordt weergegeven. U kunt het label op elk gewenst moment wijzigen.</p> <p><b> BELANGRIJK </b>: Gebruik geen speciale karakters in dit etiket. Ze worden niet correct weergegeven in rapporten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschrijving</td> 
      <td>Typ tekst als u aan gebruikers wilt uitleggen waarvoor de sectie is bedoeld. Dit wordt weergegeven onder het label van de sectie op het aangepaste formulier.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Toegang verlenen</p> </td> 
      <td> <p> Selecteer de machtigingen die gebruikers nodig hebben voor een object waaraan het aangepaste formulier is gekoppeld, om deze sectie weer te geven en de veldwaarden ervan te bewerken. 
       <p>De volgende toestemmingen zijn beschikbaar onder <b> Gebruikers met deze toegang tot het voorwerp kunnen gebiedswaarden </b> bekijken:</p> 
         <ul>
          <li><strong> Mening </strong>: De toestemmingen van de mening aan het voorwerp</li>
          <li><p><b> Beperkte geef </b> uit: (Beschikbaar slechts als het voorwerp een project, een taak, een kwestie, of een gebruiker is):</p> 
          <p>Staat gebruikers toe om aan het voorwerp bij te dragen als het een project, een taak, of een kwestie is.</p>
          <p>Staat gebruikers toe om het profiel uit te geven of de profieltoestemming te bezitten aan het voorwerp als het een gebruiker is.</p></li> 
          <li><b> geeft </b> uit: Beheer toestemmingen aan het voorwerp uit </li> 
          <li><b> slechts Admin </b>: Het toegangsniveau van de Beheerder van het systeem</li> 
         </ul> </li> 
        <p>De volgende toestemmingen zijn beschikbaar onder <b> Gebruikers met deze toegang tot het voorwerp kunnen gebiedswaarden </b> uitgeven: </p> 
         <ul> 
          <li> <p><b> Beperkte geef </b> uit: (Beschikbaar slechts als het voorwerp een project, een taak, een kwestie, of een gebruiker is):</p> 
           <p>Als het voorwerp een project, een taak, of een kwestie, deze toestemming gebruikers toestaat om aan het voorwerp bij te dragen</p>
          <p>Als het object een gebruiker is, kunnen gebruikers met deze machtiging het profiel bewerken of eigenaar zijn van de profielmachtiging voor het object.</p> 
          <li><b> geeft </b> uit: Beheer toestemmingen aan het voorwerp uit </li> 
          <li><b> slechts Admin </b>: Het toegangsniveau van de Beheerder van het systeem</li> 
         </ul> </li> 
       </ul> 
       <p>Voor informatie over toestemmingen op voorwerpen, zie <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref"> Overzicht van het delen van toestemmingen op voorwerpen </a>.</p> 
       <p><b> NOTA </b>:  
       <ul> 
       <li> <p>Gebruikers zonder de machtigingen die u hier opgeeft, kunnen de aangepaste velden en widgets niet zien in de sectie. </p> <p>Dit is ook het geval als u de waarden van de velden in rapporten weergeeft of deze in berekende velden gebruikt in tekstmodusrapportage.</p> </li> 
       <li><p>Aangepaste formulieren aanvragen/uitgeven: als toegang weergeven nodig is om de velden in het sectie-einde te zien, maar beheerderstoegang nodig is om de velden te bewerken, zijn de sectie en alle velden niet zichtbaar voor niet-beheerders wanneer zij het formulier invullen. Zodra het verzoek is gecreeerd, dan kunnen de gebruikers met de toegang van de Mening de gebieden in de sectie bekijken.</p></li>
       <li> <p>Als u meerdere objecttypen aan uw formulier koppelt, kunt u de weergave- en bewerkingsmachtigingen wijzigen die in deze stappen beschikbaar zijn. Voor meer informatie, zie <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref"> hoe de veelvoudige objecten types sectie kunnen beïnvloeden toestemmingen in een douanevorm </a> in dit artikel.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Logica toevoegen</p></td> 
      <td><p>Gebruik weergaverelogica om op te geven of de sectie op het formulier moet worden weergegeven, op basis van selecties die gebruikers in meerkeuzevelden maken wanneer ze het formulier invullen.</p><p><strong> NOTA:</strong> als alle individuele gebieden onder een sectieonderbreking vertoningslogica hebben die op hen wordt toegepast en zij allen als resultaat van de logica verborgen zijn, zal de volledige sectie op de douanevorm worden verborgen. Dit gebeurt ook als de weergaverelogica niet wordt toegepast op het sectie-einde.</p><p>Voor meer informatie, zie <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref"> vertoningslogica toevoegen en logica met de vormontwerper </a> overslaan.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Sleep of voeg minstens één aangepast veld of widget toe aan de nieuwe sectie. Dit is vereist voordat u de sectie opslaat.

1. Klik **Gedaan**.

   >[!TIP]
   >
   >U kunt **klikken toepast** op om het even welk punt terwijl u een douaneformulier creeert om uw veranderingen te bewaren en de vorm open te houden.

### Hoe meerdere objecttypen de machtigingen voor secties kunnen beïnvloeden {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

De beperkte machtiging Bewerken voor afbrekingen van aangepaste formuliersecties is alleen beschikbaar voor de typen projecten, taken, problemen en gebruikersobjecten.

Als u in een aangepast formulier met een sectie-einde dat is geconfigureerd met de machtiging Beperkte bewerking, een van de andere objecttypen aan het formulier toevoegt (Portfolio, Programma, Document, Bedrijf, Factureringsrecord, Interventie, Kosten of Groep), wordt u gevraagd om over te schakelen naar de machtiging Bewerken. Deze is compatibel met zowel dat objecttype als de bestaande objecttypen op het formulier.

>[!INFO]
>
>**Voorbeeld:** in een douanevorm verbonden aan het de objecten van het Project type, wordt een sectieonderbreking gevormd met de Beperkte Edit toestemming.
>
>U voegt het Portfolio-objecttype aan het formulier toe. Dit betekent dat de optie Beperkte bewerking niet langer beschikbaar is voor het sectie-einde in het formulier.
>
>In een bericht op het scherm wordt u gevraagd om over te schakelen naar de machtiging Bewerken. Dit is het laagste niveau van bevoegdheden dat compatibel is met zowel het objecttype Project als het Portfolio-objecttype.


## Aangepaste velden en widgets in een aangepast formulier plaatsen


1. Beginnen creërend of het uitgeven van een douanevorm, zoals die in [&#x200B; wordt beschreven creeer een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Als u aangepaste velden en widgets op dezelfde rij wilt plaatsen, sleept u een naast elkaar totdat er een lijn tussen de velden en widgets wordt weergegeven.

   >[!NOTE]
   >
   >* U kunt de **knoop van de Voorproef** in de hoger-juiste hoek gebruiken om een idee van te krijgen hoe de douanegebieden en widgets in de vorm zullen tonen.
   >* Aangepaste velden en widgets geven het formulier mogelijk niet altijd op dezelfde manier weer, afhankelijk van hoeveel schermruimte beschikbaar is wanneer een gebruiker het formulier bekijkt. Het derde veld in een rij velden kan bijvoorbeeld omlopen naar de volgende rij velden als de horizontale ruimte beperkt is.

1. (Optioneel) Als u een aangepast veld of een aangepaste widget boven of onder een ander veld of een andere widget wilt plaatsen, sleept u het onder of boven totdat er een horizontale blauwe lijn tussen de items wordt weergegeven.

1. Om een douanegebied naar een andere sectie op de vorm te bewegen, kunt u het slepen en laten vallen in plaats, of de **Beweging aan** pictogram op het gebied klikken en de sectie selecteren om het te bewegen naar.

   ![&#x200B; gebied van de beweging aan een sectie &#x200B;](assets/move-field-to-section.png)

1. Om uw veranderingen te bewaren, klik **toepassen**

   of

   Klik **sparen en Sluiten**.

## Een voorbeeld van een aangepast formulier bekijken

1. Begin creërend of het uitgeven van een douanevorm en het toevoegen van gebieden, zoals die in [&#x200B; worden beschreven creeer een douanevorm &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klik **Voorproef** in de hoger-juiste hoek om te zien hoe de vorm wanneer wordt gebruikt zal kijken, dan klik **Voorproef van het Eind** om op het uitgeven van de vorm terug te keren.

   >[!NOTE]
   >
   >Geavanceerde logica wordt niet ondersteund in de voorbeeldmodus van de formulierontwerper.


