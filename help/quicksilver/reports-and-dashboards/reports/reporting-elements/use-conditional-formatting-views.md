---
product-area: reporting
navigation-topic: reporting-elements
title: Voorwaardelijke opmaak gebruiken in weergaven
description: Als u uw rapporten deelt met andere gebruikers in Adobe Workfront, kunt u overwegen de weergave van de rapporten aan te passen om bepaalde informatie beter leesbaar te maken, of gewoon op te vallen.
author: Lisa
feature: Reports and Dashboards
exl-id: 0ea65b3f-fbcf-40f4-a4d1-4dd91619c349
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1148'
ht-degree: 0%

---

# Voorwaardelijke opmaak gebruiken in weergaven

Als u uw rapporten deelt met andere gebruikers in Adobe Workfront, kunt u overwegen de weergave van de rapporten aan te passen om bepaalde informatie beter leesbaar te maken, of gewoon op te vallen.

U kunt het tabblad Details van uw rapporten aanpassen door speciale of voorwaardelijke opmaak toe te voegen aan de weergave van uw rapporten.

U moet over beheerdersmachtigingen voor het rapport beschikken om het rapport te kunnen bewerken en speciale opmaak aan de weergave toe te voegen.

Zie het artikel voor meer informatie over het maken van rapporten [Een aangepast rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Door kolommen voorwaardelijk in de mening van het rapport te formatteren, kunt u opstellingsregels die de manier beïnvloeden het rapport wordt getoond. Wanneer aan deze voorwaarden of regels is voldaan, wordt de speciale opmaak toegepast.

Als een taak bijvoorbeeld voor minder dan 20 procent is voltooid, kunt u het veld markeren door het percentagenummer weer te geven in vette, rode tekst en een gele achtergrondkleur.

In een voorwaardelijk opgemaakte weergave kunt u:

* Wijzig de koptekst van een kolom.
* Wijzig de waarde van een kolom in aangepaste tekst of een afbeelding.
* Maak de weergave van een veld op door het lettertype, de kleur, de uitlijning of de kleur van de achtergrond te wijzigen.

De veranderingen u in de mening van het rapport aanbrengt worden van kracht slechts op het lusje van Details van het rapport. Deze wijzigingen zijn niet van invloed op de tabbladen Overzicht, Matrix of Diagram van het rapport.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een weergave in een rapport te bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor een rapport beheren om een weergave in een rapport te maken of te bewerken</p> <p>Machtigingen beheren voor een weergave</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Vereisten

U moet een rapport maken voordat u er voorwaardelijke opmaak aan kunt toevoegen.

Voor informatie over het maken van een rapport raadpleegt u [Een rapport maken](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Een weergave met voorwaardelijke opmaak maken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Rapporten**.

1. Klik de naam van een rapport waar u een voorwaardelijk-geformatteerde mening wilt tot stand brengen.

   of

   Klikken **Handelingen rapporteren** en klik vervolgens op **Bewerken**.

1. (Voorwaardelijk) als u een rapport hebt uitgegeven, selecteer een bestaande kolom, of creeer een nieuwe kolom.
1. Klikken **Geavanceerde opties**.

1. Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Aangepast kolomlabel</strong></td> 
      <td> <p>Geef een naam op voor de kolom.</p> <p>Als u een bestaande kolom bewerkt en hier een naam opgeeft, wordt de bestaande kolomnaam gewijzigd.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Veldindeling</strong></td> 
      <td>Kies de indeling waarin de waarde in de kolom wordt weergegeven. Afhankelijk van wat het kolomveld is, kunt u zo instellen hoe datums, getallen of valuta worden weergegeven.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Deze kolom tonen wanneer deze zich op een dashboard bevindt</strong></td> 
      <td>Selecteer dit gebied als u de kolom wilt tonen wanneer het rapport op een dashboard wordt geplaatst. De kolom toont altijd wanneer u het rapport buiten een dashboard bekijkt.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Een regel toevoegen voor deze kolom**.

   <!--
   <note type="note">
   You cannot apply conditional formatting to a User Team ID field. (NOTE: drafted this. Not sure why we have to single out just this one field?)
   </note>
   -->

1. In de **Wanneer:** , stelt u een voorwaardelijke instructie in voor de kolom. Bijvoorbeeld: wanneer het Volledige Percentage van de Taak (Gevoelig Geval) 50 evenaart.
1. In de **Het veld als volgt weergeven:** geeft u op hoe dit veld eruitziet als aan de bovenstaande voorwaarde is voldaan.

   Geef de volgende informatie op:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Tekstkleur</strong></td> 
      <td> <p>Selecteer de kleur waarin de tekst wordt weergegeven. Er zijn 8 kleuren beschikbaar.</p> <p>Opmerking: Als het veld een hyperlink bevat, worden de tekstkleurselecties niet toegepast op dit veld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tekstindeling</strong></td> 
      <td>Selecteer of tekst vet of cursief moet worden weergegeven.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tekstuitlijning</strong></td> 
      <td>Selecteer of de tekst rechts, midden of links in de kolom moet worden uitgelijnd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Achtergrond</strong></td> 
      <td>Selecteer de kleur van de achtergrond voor de tekst. Er zijn 8 kleuren beschikbaar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pictogram tonen</strong></td> 
      <td>Selecteer een van de 16 pictogrammen als u een pictogram wilt weergeven in plaats van de werkelijke waarde voor deze kolom.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Tekst tonen</strong></td> 
      <td> <p>Selecteer deze optie om een aangepast label voor deze kolom weer te geven in plaats van de werkelijke waarde ervan. Geef de tekst op die u wilt weergeven in plaats van de waarde in het opgegeven veld.</p> <p>Belangrijk: Selecteren <strong>Tekst tonen</strong> Hiermee schakelt u de mogelijkheid uit om de tekst in deze kolom inline te bewerken.<br>Ook, kunt u niet de waarde van een kolom veranderen van de Voorganger omdat het ingebouwde logica bevat.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Toepassen op de hele rij</strong></td> 
      <td>Selecteer deze optie om instellingen toe te passen op de hele rij in plaats van alleen de geselecteerde kolom instellingen toe te passen.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Regel toevoegen**.\
   U kunt extra regels toevoegen aan dezelfde kolom of regels toevoegen aan andere kolommen.

   Regels worden toegepast in de volgorde waarin ze zijn gemaakt. Zij worden gecombineerd maar beschrijven elkaar niet, hoewel een kolomregel belangrijkheid over een rijregel op de zelfde cel neemt.

   Voorbeeld 1: U kunt eerst een regel maken die aangeeft dat de tekstkleur paars en vet is wanneer de projectstatus aan het bouwen is. Vervolgens maakt u een tweede regel die aangeeft wanneer de taaknaam niet leeg is, de tekstkleur rood en cursief is en de achtergrondkleur groen. In dit voorbeeld gebeurt het volgende:

   * De taken waarvan de Status van het Project de Bouw is worden getoond in paarse en gewaagde teksten. Als de taaknaam niet leeg is, hebben taken ook een groene achtergrond.
   * De taken waarvan de Status van het Project om het even wat buiten de Bouw (en de Naam van de Taak is niet leeg) is worden getoond in een rode en cursieve tekst met een groene achtergrond.

   Voorbeeld 2: Creeer een regel op het Geplande Datum van de Voltooiing van het Project die de volledige rij beïnvloedt, die de achtergrond grijs draaien als het project wordt geannuleerd (Status = &quot;Dead&quot;). Maak vervolgens een kolomregel die de achtergrond rood maakt wanneer de geplande Voltooiingsdatum van het project lager is dan vandaag (wat betekent dat het project te laat is). In dit voorbeeld geldt dat als een geannuleerd project een late voltooiingsdatum heeft, die cel rood wordt weergegeven, ook al zijn de andere cellen in de rij grijs. Deze opmaak corrigeren:

   * Bewerk de opmaak voor de geplande voltooiingsdatum en verwijder de kolomregel voor de rode achtergrond op late projecten.
   * Voeg een kolomregel toe met de zelfde het formatteren zoals de rijregel (grijze achtergrond wanneer de Status van het Project = &quot;Dead.&quot;)
   * Voeg opnieuw de kolomregel voor de rode achtergrond op late projecten toe.
   * Wanneer u de regels en de weergave opslaat, wordt de rode achtergrond niet toegepast op een geannuleerd project.


1. Klikken **Gereed**.
1. Klikken **Opslaan + Sluiten**.\
   In het rapport zien gebruikers wijzigingen in de indeling als aan de opgegeven voorwaarden is voldaan.
