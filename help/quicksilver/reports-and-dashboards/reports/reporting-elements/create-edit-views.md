---
product-area: reporting
navigation-topic: reporting-elements
title: Weergaven maken of bewerken in Adobe Workfront
description: U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. U kunt verschillende typen weergaven gebruiken in Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 0%

---

# Weergaven maken of bewerken in Adobe Workfront

U kunt het type informatie aanpassen dat u op het scherm weergeeft met behulp van weergaven. U kunt verschillende typen weergaven gebruiken in Adobe Workfront.

In dit artikel wordt beschreven hoe u standaardweergaven voor lijsten en rapporten maakt en bewerkt, en hoe u flexibele weergaven maakt. Zie voor meer informatie [Overzicht van weergaven in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>Toegang tot filters, weergaven, groepen bewerken</p> <p>Toegang tot rapporten, dashboards, kalenders bewerken om een weergave in een rapport te maken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Rechten voor een rapport beheren om een weergave in een rapport te maken of te bewerken</p> <p>Machtigingen beheren voor een weergave om deze te bewerken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Een weergave maken of aanpassen

Het proces voor het maken of aanpassen van een weergave is afhankelijk van het feit of u een standaardweergave of een blokweergave maakt of aanpast.

* [Een standaardweergave maken of aanpassen](#create-or-customize-a-standard-view)
* [Een eenvoudige weergave maken of aanpassen](#create-or-customize-an-agile-view)

### Een standaardweergave maken of aanpassen {#create-or-customize-a-standard-view}

U kunt een nieuwe standaardweergave maken of een bestaande standaardweergave aanpassen die u eerder hebt gemaakt.

1. Klik op de knop **Weergave** vervolgkeuzemenu in een lijst waarin u een weergave wilt maken of aanpassen.
1. (Optioneel) Als u een bestaande weergave wilt aanpassen, selecteert u de standaardweergave die u wilt aanpassen.\
   De standaardmeningen zijn beschikbaar op om het even welk type van lijst in Workfront, zoals een rapport, een projectlijst, of een taaklijst.
1. Klik op de knop **Weergave** vervolgkeuzemenu en vervolgens op **Weergave aanpassen** of **Nieuwe weergave**.\
   De **Weergave aanpassen** wordt weergegeven.

1. In de **Kolomvoorvertoning** in, voert u een van de volgende handelingen uit:

   * Wijzig de waarde van een kolom door op de kolomtitel te klikken en vervolgens een nieuw veld te selecteren.
   * Een kolom toevoegen door te klikken op **Kolom toevoegen** typt u eerst de naam van de kolom die u wilt toevoegen en klikt u erop wanneer deze kolom in de vervolgkeuzelijst wordt weergegeven.
   * Pas de volgorde van de kolommen aan door de kolomtitel naar een nieuwe locatie te slepen.

      * (Optioneel) In het dialoogvenster **Kolominstellingen** gebied, klikt u op **Deze kolom samenvatten met** selecteert u een van de beschikbare opties voor het samenvatten van de gegevens. Wanneer u deze optie kiest, wordt de informatie in uw kolom samengevoegd in de groepen van het rapport.\
         Voor datumvelden kunt u de waarden als volgt samenvatten:

         * Maximum
         * Minimaal

         Voor getal- en valutavelden kunt u de waarden als volgt samenvatten:

         * Aantal
         * Som
         * Gemiddeld
         * Maximum
         * Minimaal

         >[!NOTE]
         >
         >De volgende uitzonderingen gelden voor bovenliggende objecten (bijvoorbeeld bovenliggende taken) wanneer u waarden samenvoegt voor de volgende velden in groepen:
         >   
         >   * Alle getallen en valutavelden behalve Werkelijke uren (bijvoorbeeld Geplande/Werkelijke loonkosten, Geplande/Werkelijke kosten, Geplande/Werkelijke kosten, Geplande/Geplande uren) tellen alleen de waarden voor de kindertaken en standalone taken samen. De waarden voor de bovenliggende taken of ouders van ouders worden niet samengevoegd.
         >   * Werkelijke uren tellen de waarden voor de hoofdouder en de standalone taken samen; zij tellen niet de aantallen voor de ouders van oudertaken of de kindtaken samen.
         >   * Aangepaste gegevensvelden voor getal- en valutawaarden voegen alle taken samen: ouders, kinderen, ouders van ouders en zelfstandige taken.


         Zie het artikel voor meer informatie over het gebruik van groepen in een rapport [Overzicht van groepen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Optioneel) Klik op **Geavanceerde opties** om de volgende informatie voor de kolom te specificeren:

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Aangepast kolomlabel</strong></td> 
           <td><p>Geef een aangepast label voor de kolom op. Dit label vervangt het standaardlabel.</p></td> 
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
           <td><p>Klikken <strong>Een regel toevoegen voor deze kolom</strong> om een regel voor de kolom te definiëren. Nadat u een regel hebt toegevoegd, kunt u veld- en tekststijlen definiëren voor de weergave van velden die overeenkomen met die regel. Klikken <strong>Regel toevoegen</strong> nadat u klaar bent met het definiëren van de regel.</p></td> 
          </tr> 
         </tbody> 
        </table>

         Zie het artikel voor meer informatie over het voorwaardelijk opmaken van weergaven in rapporten [Voorwaardelijke opmaak gebruiken in tekstmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. (Voorwaardelijk) Als u hebt geklikt **Geavanceerde opties**, klikt u op **Gereed**.

1. Klikken **Weergave opslaan** om een nieuwe weergave te maken of om de huidige weergave te vervangen door uw wijzigingen.\
   of\
   Klikken **Opslaan als nieuwe weergave** om uw wijzigingen als een nieuwe weergave op te slaan.

   >[!TIP]
   >
   >De **Opslaan als nieuwe weergave** is de enige beschikbare optie wanneer u een ingebouwde weergave van Workfront aanpast.

   Uw toegang bepaalt hoe de weergave wordt opgeslagen. Als u de weergave oorspronkelijk hebt gemaakt, kunt u de wijzigingen opslaan. anders, wordt u ertoe aangezet om een versie te bewaren. Houd er rekening mee dat wijzigingen die u aanbrengt in de weergave van invloed zijn op gebruikers met wie de weergave is gedeeld.

### Een eenvoudige weergave maken of aanpassen {#create-or-customize-an-agile-view}

U kunt een nieuwe Google-weergave maken of een bestaande, flexibele weergave aanpassen die u eerder hebt gemaakt.

>[!IMPORTANT]
>
>Gelijke weergaven zijn alleen beschikbaar wanneer u een project weergeeft.

Raadpleeg het artikel voor meer informatie over de Google-weergaven [Een project beheren in de Google-weergave](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

U kunt als volgt een eenvoudige weergave maken of aanpassen:

1. Ga naar de lijst met taken in een project.
1. Klik op de knop **Agile Storyboard** pictogram ![](assets/agile-storyboard-nwe.png).

1. (Voorwaardelijk) U kunt als volgt een bestaande beoordelingsweergave aanpassen:

   1. Klik op de knop **Weergave** en selecteert u vervolgens de apparaatweergave die u wilt aanpassen.\
      U kunt de standaardweergave Gelijk niet aanpassen.

   1. Klik op de knop **Weergave** vervolgkeuzemenu nogmaals, en klik vervolgens op **Weergave aanpassen**.\
      ![](assets/view-agile-customize.png)

1. (Voorwaardelijk) Als u een nieuwe beoordelingsweergave wilt maken, klikt u op **Nieuwe weergave**.\
   De **Gelijkmatige weergave aanpassen** wordt weergegeven.

1. In de **Gelijkmatige weergave aanpassen** geeft u een naam op voor de weergave Gelijk.\
   We raden u aan het woord &#39;Gelijk&#39; op te nemen in de weergavenaam, zodat gebruikers weten dat dit een Gegale weergave is.\
   Deze naam wordt weergegeven in het dialoogvenster **Weergave** vervolgkeuzelijst wanneer u een weergave selecteert.

1. Definieer de statuskolommen die u wilt weergeven op het artikelbord in de Tegelweergave. Dit zijn de taakstatussen die door de beheerder van Workfront worden bepaald, zoals die in [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Alleen de systeemstatussen zijn beschikbaar voor gebruik op het artikel. Als een status alleen beschikbaar is voor een afzonderlijke groep waarvan u lid bent, is de status niet beschikbaar op de agile-artikelkaart. Bovendien zijn taken die zich in een status bevinden die alleen voor een aangepaste groep beschikbaar is, niet zichtbaar wanneer u het project in een georiënteerde weergave bekijkt.

   Gebruikers kunnen artikelen over deze statuskolommen verplaatsen op het artikel in het artikel.\
   Wanneer u statuskolommen definieert, kunt u het volgende doen:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Statuskolommen opnieuw ordenen:</strong> </td> 
      <td> Sleep een statuskolom naar de volgorde waarin u deze wilt weergeven.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statuskolommen verwijderen:</strong> </td> 
      <td>Klik op het pictogram (x) in de kolom die u wilt verwijderen.<br>U kunt de status 'Nieuw' alleen verwijderen als er een aangepaste status is toegevoegd aan de weergave en die aangepaste status overeenkomt met 'Nieuw'.<br>Voor informatie over het maken van een aangepaste status raadpleegt u <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Een status maken of bewerken</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Statuskolommen toevoegen:</strong> </td> 
      <td> <p>Klik op de knop <strong>Plus</strong> en selecteert u vervolgens de status die u wilt toevoegen.<br>Alle standaardsysteemstatussen worden weergegeven, evenals eventuele aangepaste statussen die met u zijn gedeeld.<br>U kunt maximaal 10 statussen configureren voor weergave.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. In de **Kaartkleur koppelen aan** selecteert u een van de volgende opties:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Artikel:</strong> </td> 
      <td>Eventuele subtaken komen overeen met de kleur van de bovenliggende taak, zodat de kleuren van alle artikelen in een bepaalde sjabloon gelijk zijn.<br>De kleuren worden willekeurig toegewezen aan taken wanneer zij worden gecreeerd als de taak geen subtaken heeft of geen oudertaak heeft.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Vrije vorm:</strong> </td> 
      <td> Alle kaarten worden standaard als blauw weergegeven totdat een gebruiker de kleur handmatig wijzigt, zoals in het artikel wordt beschreven <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Artikelen op kleur categoriseren op het scrollbord</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioriteit:</strong> </td> 
      <td> <p> Kleuren worden als volgt gekoppeld aan de prioriteit van het artikel:</p> 
       <ul> 
        <li>Hoog = rood</li> 
        <li>Normaal = geel</li> 
        <li>Laag = groen<br>Als uw Workfront-beheerder aangepaste prioriteiten voor uw Workfront-systeem heeft geconfigureerd, heeft de hoogste prioriteit rood, is de op één na hoogste geel en zijn de resterende prioriteiten groen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Taakeigenaar:</strong> </td> 
      <td> Alle artikelen met dezelfde primaire toewijzing hebben dezelfde kleur.<br>De primaire ontvanger is de gebruiker die voor het eerst aan de taak is toegewezen. </td> 
     </tr> 
    </tbody> 
   </table>

1. In de **Agile** in de **Aanvullende velden** gebied, klikken **Veld toevoegen** Selecteer vervolgens het veld dat u aan artikelkaarten wilt toevoegen. (Dit zijn de zelfde gebieden u kunt toevoegen wanneer het creëren van het aanpassen van een mening of het creëren van kolommen voor een rapport.)\
   Herhaal dit proces om maximaal drie extra velden aan de artikelkaarten toe te voegen.\
   Wanneer u velden toevoegt aan artikelkaarten, zijn velden alleen-weergeven en alleen weergeven wanneer het veld is gevuld.

   Standaard worden de volgende gegevenstypen weergegeven op de artikelkaart:

   * Artikelnaam met een koppeling die rechtstreeks naar de taak verwijst
   * De projectnaam met een verbinding direct aan het project\
      Deze koppeling wordt alleen weergegeven wanneer de schakelweergave op een herhaling wordt gebruikt. wordt niet weergegeven wanneer u een mobiele weergave gebruikt voor een project.
   * De taakbeschrijving
   * Huidige verplichting
   * Het percentage voltooide bewerkingen weergeven en bewerken door het percentage aan te passen dat is voltooid of door het aantal punten of uren aan te passen dat is voltooid
   * Toegewezen gebruikers

   U kunt aanvullende gegevens (inclusief aangepaste gegevens) weergeven op artikelkaarten. U wilt mogelijk om een aantal redenen extra velden weergeven op artikelkaarten. Bijvoorbeeld, zou u identiteitskaart van de Klant kunnen willen tonen als u aan verhalen voor veelvoudige klanten binnen het project werkt, of u zou de Datum van het Begin van de Taak kunnen willen tonen.

1. Klikken **Opslaan**.\
   Uw toegang bepaalt hoe de weergave wordt opgeslagen. Als u de weergave oorspronkelijk hebt gemaakt, kunt u de wijzigingen opslaan. anders, wordt u ertoe aangezet om een versie te bewaren. Houd er rekening mee dat wijzigingen die u aanbrengt in de weergave van invloed zijn op gebruikers met wie de weergave is gedeeld.

1. (Optioneel) Klik op de knop **Lijstweergave** pictogram ![](assets/list-view-in-agile-view-for-tasks.png) om terug te keren naar de takenlijst.
