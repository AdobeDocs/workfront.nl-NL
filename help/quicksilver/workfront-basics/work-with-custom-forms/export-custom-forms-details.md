---
title: Aangepaste formulieren en objectdetails exporteren
description: Aangepaste formulieren en objectdetails exporteren
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 0%

---

# Aangepaste formulieren en objectdetails exporteren

U kunt het overzicht en de informatie van de douaneformulier van de sectie van Details van een voorwerp naar een dossier van de PDF uitvoeren. U kunt de PDF vervolgens afdrukken of delen met andere gebruikers.

Deze functionaliteit wordt ondersteund voor de volgende objecten:

* Projecten
* Taken
* Problemen
* Portfolio
* Programma&#39;s

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>De velden in de sectie Details die uw Workfront of groepsbeheerder heeft verwijderd met een lay-outsjabloon, worden niet weergegeven.

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-licentie*</p> </td> 
   <td> <p>Aanvraag of hoger voor problemen</p> <p>Controle of hoger voor projecten en taken</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong> het niveauconfiguraties van de Toegang* </strong> </td> 
   <td> <p>Weergave of hoger voor projecten, taken en problemen</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objectmachtigingen</p> </td> 
   <td> <p>Geef meer of meer machtigingen weer voor het project, de taak of de uitgave waarvan u het formulier wilt exporteren</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Vereisten

Voordat u begint, moet u beschikken over alle volgende opties:

1. Er is een aangepast formulier gemaakt voor een specifiek object waaruit u het wilt exporteren.
1. Het aangepaste formulier aan het object laten koppelen

   of

   U hebt de juiste toegang om een aangepast formulier toe te voegen en de gegevens op het formulier te bewerken.

Voor informatie over het creëren van douaneformulieren, zie [ een douaneformulier ](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) creëren of uitgeven.

Voor informatie over het vastmaken van vormen aan voorwerpen, zie [ een douanevorm aan een voorwerp ](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) toevoegen.

## Informatie exporteren in de sectie Details

Informatie exporteren uit de sectie Details van een object is identiek voor alle objecten waarvoor dit wordt ondersteund.

1. Ga naar een project, een taak, een portefeuille, een programma, of een kwestie waarvoor u minstens de toestemmingen van de Mening hebt.
1. Klik het **&quot;Details&quot;punt** op het linkerpaneel, zoals **Details van de Taak**.
1. (Facultatief) als er geen douaneformulier in bijlage aan het voorwerp is, begin de naam van een douaneformulier in **te typen voeg douanevormgebied** toe, dan het te klikken wanneer het in de lijst verschijnt.

   U kunt maximaal 10 formulieren toevoegen.

1. (Facultatief) de informatie van de update in de sectie van Details, dan klik **sparen Veranderingen**.
1. Klik het **drop-down menu van de Uitvoer** in de hoger-juiste hoek, uitgezocht **Overzicht**, of de vormen u wilt uitvoeren, dan klik **Uitvoer**.

   U kunt **selecteren allen** ook selecteren als u het gebied van het Overzicht en alle douaneformulieren wilt uitvoeren.

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >De volgende scenario&#39;s kunnen bestaan:
   >
   >   
   >   
   >   * Wanneer uw groep of Workfront-beheerder de selectie van alle velden in het gebied Overzicht opheft en voor het object aangepaste formulieren zijn gekoppeld, wordt de sectie Overzicht niet weergegeven.
   >   * Wanneer uw groep of Workfront-beheerder de selectie van alle velden in het gebied Overzicht opheft en er geen aangepaste formulieren zijn gekoppeld voor het object, is het vervolgkeuzemenu Exporteren niet zichtbaar.
   >   * Als voor het object geen aangepaste formulieren zijn gekoppeld, kunt u alleen het gebied Overzicht exporteren.
   >   * Aangepaste velden die achter logica staan en niet zichtbaar zijn op het formulier, worden niet geëxporteerd. Voor informatie over het toevoegen van logica aan een douanevorm, zie [ vertoningslogica toevoegen en logica overslaan aan een douanevorm ](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).
   >   
   >

   Er wordt een PDF-bestand gemaakt en naar de computer gedownload. Het PDF-bestand bevat de volgende informatie:

   * De naam van het object waaraan het formulier is gekoppeld
   * De naam van de gebruiker die de PDF heeft geëxporteerd
   * De datum en het tijdstip waarop de PDF is geproduceerd
   * De naam van de geëxporteerde formulieren
   * Informatie uit de velden die op het formulier zijn ingevuld
