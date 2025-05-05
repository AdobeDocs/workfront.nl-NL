---
product-area: reporting
navigation-topic: reporting-elements
title: Weergaven maken of bewerken in Adobe Workfront
description: U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. In Adobe Workfront kunt u verschillende typen weergaven gebruiken.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: d98998627ac5161fd12bb2d86f65555550c82a48
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 0%

---

# Weergaven maken of bewerken in Adobe Workfront

<!-- Audited: 11/2024 -->

U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. In Adobe Workfront kunt u verschillende typen weergaven gebruiken.

In dit artikel wordt beschreven hoe u standaardweergaven voor lijsten en rapporten maakt en bewerkt, en hoe u flexibele weergaven maakt. Voor meer informatie, zie [ Overzicht van Meningen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> 
      <p>Nieuw:</p>
         <ul>
         <li><p>Medewerker of hoger</p></li>
         </ul>
      <p>Huidige:</p>
         <ul>
         <li><p>Aanvraag of hoger</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een weergave in een rapport te maken</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen*</strong></td> 
   <td> <p>Rechten voor een rapport beheren om een weergave in een rapport te maken of te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*For informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een weergave maken of aanpassen

Het proces voor het maken of aanpassen van een weergave is afhankelijk van het feit of u een standaardweergave of een blokweergave maakt of aanpast.

* [ creeer of pas een standaardmening ](#create-or-customize-a-standard-view) aan
* [Een eenvoudige weergave maken of aanpassen](#create-or-customize-an-agile-view)

### Een standaardweergave maken of aanpassen {#create-or-customize-a-standard-view}

U kunt een nieuwe standaardweergave maken of een bestaande standaardweergave aanpassen die u eerder hebt gemaakt.

1. Klik het **drop-down menu van de Mening** op om het even welke lijst waar u een mening tot stand wilt brengen of aanpassen.

1. Klik op de knop **+ Nieuwe weergave** om een nieuwe weergave te maken.
of
Klik **uitgeven** pictogram ![ geeft pictogram ](assets/edit-icon.png) uit dat op muis over rechts van een bestaande mening verschijnt u wilt uitgeven.
**past de vertoningen van de de dialoogdoos van de Mening** aan.

1. In de **sectie van de Voorproef van de Kolom**, doe om het even welke volgend:

   * Wijzig de waarde van om het even welke kolom door de kolomtitel te klikken en dan een nieuw gebied te selecteren.
   * Voeg een kolom toe door **te klikken voeg Kolom** toe, begin typend de naam van de kolom die u wilt toevoegen, dan het klikken wanneer het in de drop-down lijst verschijnt.
   * Pas de volgorde van de kolommen aan door de kolomtitel naar een nieuwe locatie te slepen.

   * In het **gebied van de Montages van de Kolom**, klik **vat deze kolom door** samen, en kies hoe u de gegevens in de kolom wilt tonen. Deze optie is beschikbaar voor de volgende kolomtypen:

     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Datumvelden</strong></td> 
           <td><ul>
           <li>Maximum</li>
         <li>Minimaal</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Valutamarkten</strong></td> 
           <td><ul>
           <li>Aantal</li>
         <li>Som</li>
           <li>Gemiddeld</li>
         <li>Maximum</li>
           <li>Minimaal</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Tekenreeks- en Booleaanse velden</strong></td> 
           <td><ul><li>Aantal</li></ul>
           <p>Opmerking: Workfront raadt doorgaans niet aan een booleaans veld op aantal samen te vatten, omdat de waarde altijd true/false is.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >De volgende uitzonderingen zijn van toepassing op bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvat voor de volgende velden in groepen:
     >   
     > * In alle velden voor getallen en valuta&#39;s, met uitzondering van werkelijke uren (bijvoorbeeld geplande/werkelijke loonkosten, geplande/werkelijke kosten, geplande/werkelijke kosten, geplande uren) wordt een overzicht gegeven van de waarden voor alleen kindertaken en zelfstandige taken. Zij vatten de waarden voor de oudertaken of de ouders van ouders niet samen.
     > * Werkelijke uren geeft een overzicht van de waarden voor de hoofdbovenliggende taken en de zelfstandige taken; deze geven geen overzicht van de getallen voor de bovenliggende taken of de onderliggende taken.
     > * De gegevensgebieden van de douane voor aantal en muntwaarden vatten alle taken samen: ouders, kinderen, ouders van ouders, en standalone taken.
     >
     >Voor meer informatie over het gebruiken van groeperingen in een rapport, zie het artikel [ overzicht van Groepen in Adobe Workfront ](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Facultatief) klik **Geavanceerde Opties** om de volgende informatie voor de kolom te specificeren:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Aangepast kolomlabel</strong></td> 
           <td><p>Geef een aangepast label voor de kolom op. Dit label vervangt het standaardlabel. We raden u aan alleen UTF-8-tekens te gebruiken om compatibiliteitsproblemen te voorkomen.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Veldindeling</strong></td> 
           <td>Selecteer de indeling waarin u de waarden voor de velden in de kolom wilt weergeven.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Deze kolom tonen wanneer deze zich op een dashboard bevindt</strong></td> 
           <td><p>Selecteer deze optie om deze kolom op een dashboard te tonen, wanneer het rapport naast elkaar met een ander rapport wordt getoond. Als deze optie is uitgeschakeld, wordt deze kolom niet weergegeven wanneer u het rapport weergeeft op een dashboard waar rapporten naast elkaar worden weergegeven.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Kolomregels</strong></td> 
           <td><p>Klik <strong>+ voeg een Regel voor deze Kolom </strong> toe om een regel voor de kolom te bepalen. Nadat u een regel hebt toegevoegd, kunt u veld- en tekststijlen definiëren voor de weergave van velden die overeenkomen met die regel. Klik <strong> toevoegen Regel </strong> nadat u het bepalen van de regel hebt gebeëindigd.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Voor meer informatie over voorwaardelijk het formatteren van meningen in rapporten, zie het artikel [ Voorwaardelijke het formatteren van het Gebruik in de Wijze van de Tekst ](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Voorwaardelijk) als u **Geavanceerde Opties** klikte, klik **Gedaan**.

1. Klik **sparen Mening** om een nieuwe mening tot stand te brengen of de huidige mening met uw veranderingen te vervangen.\
   of\
   Klik **sparen als Nieuwe Mening** om uw veranderingen als nieuwe mening te bewaren.

   >[!TIP]
   >
   >**sparen als Nieuwe Mening** is de enige beschikbare optie wanneer u een ingebouwde mening van Workfront aanpast.

   Uw toegang bepaalt hoe de weergave wordt opgeslagen. Als u de weergave hebt gemaakt, kunt u de wijzigingen opslaan. Als u dit niet doet, wordt u gevraagd een versie op te slaan. Houd er rekening mee dat wijzigingen die u aanbrengt in de weergave van invloed zijn op gebruikers met wie de weergave is gedeeld.

### Een eenvoudige weergave maken of aanpassen {#create-or-customize-an-agile-view}

U kunt een flexibele weergave maken of een bestaande, flexibele weergave aanpassen die u eerder hebt gemaakt.

>[!IMPORTANT]
>
>Gegraveerde weergaven zijn alleen beschikbaar wanneer u een project weergeeft.

Voor meer informatie over de Gelijke meningen, zie het artikel [ een project in de Gelijke Mening ](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md) leiden.

>[!NOTE]
>
>Deze procedure is alleen van toepassing op de oudere Agile-weergave, niet op de bestuursweergave van een project.

U kunt als volgt een eenvoudige weergave maken of aanpassen:

1. Ga naar de lijst met taken in een project.
1. Klik het **pictogram van de Raad ![ raad ](assets/board-icon-for-agile-view.png), en klik dan** erfenis van het Gebruik &lbrace;**op de boordmening.**

1. (Voorwaardelijk) U kunt als volgt een bestaande beoordelingsweergave aanpassen:

   1. Klik het **drop-down menu van de Mening**, dan selecteer de Gelijke mening u wilt aanpassen.\
      U kunt de standaardweergave Gelijk niet aanpassen.

   1. Klik opnieuw het **drop-down menu van de Mening**, dan klik **aanpassen Mening**.\
      ![ pas mening ](assets/view-agile-customize.png) aan

1. (Voorwaardelijk) om een nieuwe Gelijke mening tot stand te brengen, klik **Nieuwe Mening**.\
   Het **&#x200B;**&#x200B;de dialoogvakje van de Mening van de Gelijkheid aanpassen.

1. In **pas de dialoogdoos van de Mening van de Gelijkheid aan**, specificeer een naam voor de Gelijke mening.\
   We raden u aan het woord &#39;Gelijk&#39; op te nemen in de weergavenaam, zodat gebruikers weten dat dit een Gegale weergave is.\
   Deze naam wordt getoond in het **drop-down menu van de Mening** wanneer het selecteren van een mening.

1. Definieer de statuskolommen die u wilt weergeven op het artikelbord in de Tegelweergave. Dit zijn de taakstatussen die door de beheerder van Workfront worden bepaald, zoals die in [ wordt beschreven creeer of geef een status ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) uit.

   Alleen de systeemstatussen zijn beschikbaar voor gebruik op het artikel. Als een status alleen beschikbaar is voor een afzonderlijke groep waarvan u lid bent, is de status niet beschikbaar op de agile-artikelkaart. Bovendien zijn taken die zich in een status bevinden die alleen voor een aangepaste groep beschikbaar is, niet zichtbaar wanneer u het project in een georiënteerde weergave bekijkt.

   Gebruikers kunnen artikelen over deze statuskolommen verplaatsen op het artikel in het artikel.\
   Wanneer u statuskolommen definieert, kunt u het volgende doen:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> herschikt statuskolommen:</strong> </td> 
      <td> Sleep een statuskolom naar de volgorde waarin u deze wilt weergeven.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> verwijder statuskolommen:</strong> </td> 
      <td>Klik op het pictogram (x) in de kolom die u wilt verwijderen.<br> u kunt niet de "Nieuwe"status verwijderen tenzij een douanestatus aan de mening is toegevoegd en die douanestatus met "Nieuw."evenaart<br> voor informatie over het creëren van een douanestatus, zie <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref"> creeer of geef een status </a> uit.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> voeg statuskolommen toe:</strong> </td> 
      <td> <p>Klik <strong> plus </strong> pictogram, dan selecteer de status u wilt toevoegen.<br> Alle standaardsysteemstatussen worden getoond, evenals om het even welke douanestatus die met u zijn gedeeld.<br> u kunt tot 10 statussen aan vertoning vormen.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. In het **Geassocieerde Kleur van de Kaart aan** gebied, selecteer van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong> Artikel:</strong> </td> 
      <td>Eventuele subtaken komen overeen met de kleur van de bovenliggende taak, zodat de kleuren van alle artikelen in een bepaalde sjabloon gelijk zijn.<br> de Kleuren worden willekeurig toegewezen aan taken wanneer zij worden gecreeerd als de taak geen subtaken heeft of geen oudertaak heeft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Vrije Vorm:</strong> </td> 
      <td> Alle kaarten worden getoond als blauw door gebrek tot een gebruiker de kleur manueel verandert, zoals die in het artikel <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref"> wordt beschreven Categoriseer verhalen door kleur op het board van het Trommel </a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Prioriteit:</strong> </td> 
      <td> <p> Kleuren worden als volgt gekoppeld aan de prioriteit van het artikel:</p> 
       <ul> 
        <li>Hoog = rood</li> 
        <li>Medium = geel</li> 
        <li>Laag = Groen <br> als uw beheerder van Workfront douaneprioriteiten voor uw systeem van Workfront heeft gevormd, is de hoogste prioriteit rood, het tweede hoogste is geel, en het resterende is groen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Eigenaar van de Taak:</strong> </td> 
      <td> Alle artikelen met dezelfde primaire toewijzing hebben dezelfde kleur.<br> de primaire ontvanger is de gebruiker die eerst aan de taak werd toegewezen. </td> 
     </tr> 
    </tbody> 
   </table>

1. Op het **Extra Gebieden** gebied, klik **voegt Gebied** toe, dan selecteer het gebied u aan verhaalkaarten wilt toevoegen. (Dit zijn de zelfde gebieden u kunt toevoegen wanneer het creëren van het aanpassen van een mening of het creëren van kolommen voor een rapport.)\
   Herhaal dit proces om maximaal drie extra velden aan de artikelkaarten toe te voegen.\
   Wanneer u velden toevoegt aan artikelkaarten, zijn velden alleen-weergeven en alleen weergeven wanneer het veld is gevuld.

   Standaard worden de volgende gegevenstypen weergegeven op de artikelkaart:

   * Artikelnaam met een koppeling die rechtstreeks naar de taak verwijst
   * De projectnaam met een verbinding direct aan het project\
     Deze koppeling wordt alleen weergegeven wanneer de Tegelweergave op een herhaling wordt gebruikt. De koppeling wordt niet weergegeven wanneer u een flexibele weergave op een project gebruikt.
   * De taakbeschrijving
   * Huidige verplichting
   * Het percentage voltooide bewerkingen weergeven en bewerken door het percentage aan te passen dat is voltooid of door het aantal punten of uren aan te passen dat is voltooid
   * Toegewezen gebruikers

   U kunt aanvullende gegevens (inclusief aangepaste gegevens) weergeven op artikelkaarten. U wilt mogelijk om een aantal redenen extra velden weergeven op artikelkaarten. Bijvoorbeeld, zou u identiteitskaart van de Klant kunnen willen tonen als u aan verhalen voor veelvoudige klanten binnen het project werkt, of u zou de Datum van het Begin van de Taak kunnen willen tonen.

1. Klik **sparen**.\
   Uw toegang bepaalt hoe de weergave wordt opgeslagen. Als u de weergave hebt gemaakt, kunt u de wijzigingen opslaan. Als u dit niet doet, wordt u gevraagd een versie op te slaan. Houd er rekening mee dat wijzigingen die u aanbrengt in de weergave van invloed zijn op gebruikers met wie de weergave is gedeeld.

1. (Facultatief) klik het **pictogram van de Lijst** om aan de lijst van taken terug te keren.
