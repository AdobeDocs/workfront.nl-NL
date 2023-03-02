---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Gekoppelde kaarten op borden gebruiken
description: U kunt een kaart aan uw bord toevoegen die met bestaande taken en kwesties in Workfront wordt verbonden.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 1817f3b1a5950823ff6ce600b1fef09ff4ca6767
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 0%

---

# Gekoppelde kaarten op borden gebruiken

U kunt een kaart toevoegen aan uw board die is aangesloten op bestaande taken en problemen in [!DNL Workfront].

Wanneer een van de volgende gegevens voor de kaart op de ene locatie wordt bijgewerkt, wordt deze automatisch op de andere locatie bijgewerkt:

* [!UICONTROL Name]
* [!UICONTROL Description]
* [!UICONTROL Assignees]
* [!UICONTROL Status]
* [!UICONTROL Planned completion date]
* [!UICONTROL Estimation] / [!UICONTROL Story Points]

>[!NOTE]
>Eén verbonden taak of uitgave kan slechts eenmaal per board worden toegevoegd. Dezelfde taak of uitgave kan met meerdere borden worden verbonden.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie*</strong></td> 
   <td> <p>[!UICONTROL Request] of hoger</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td>
   <td><p>[!UICONTROL View] of betere toegang tot taken en problemen</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Objectmachtigingen</strong></td>
   <td><p>[!UICONTROL View] of hogere machtigingen voor de Workfront-taak of -uitgave</p></td>
  </tr>
 </tbody> 
</table>

&#42;Neem contact op met uw [!DNL Workfront] beheerder.

## Een aangesloten kaart toevoegen

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **[!UICONTROL Boards]**.
1. Toegang tot een bord. Zie voor meer informatie [Een board maken of bewerken](../../agile/get-started-with-boards/create-edit-board.md).
1. Klik op **[!UICONTROL Add card]>[!UICONTROL Connected card]**.
1. Kies een project en kies vervolgens een taak of uitgave die u als kaart aan de kaart wilt toevoegen.

   U kunt meerdere objecten selecteren en deze worden allemaal als aparte kaarten toegevoegd.

   >[!NOTE]
   >
   >* Alleen objecten waarvoor u machtigingen hebt, zijn beschikbaar in de zoekresultaten. Als een item grijs wordt weergegeven, is het al aan het bord toegevoegd.
   >* Wanneer u filtert op **[!UICONTROL Projects I Own]** of **[!UICONTROL Projects I'm On]**, worden projecten die overeenkomen met de status Voltooid, Dode of Geweigerd niet opgenomen. U kunt nog steeds naar die projecten zoeken met de **[!UICONTROL All]** filter.


1. Klik op **[!UICONTROL Add]**.

   ![Zoeken naar taak of probleem om verbinding te maken](assets/boards-tasksissues-350x94.png)

   De kaart wordt onder aan de linkerkolom toegevoegd. De aangesloten [!DNL Workfront] -object en de bijbehorende toewijzingen worden op de kaart weergegeven.

   >[!NOTE]
   >
   >Indien een verkrijger [!DNL Workfront] de taak of de kwestie is geen lid van de raad van bestuur; zij worden niet aan de kaart toegewezen.

   ![Verbonden kaart](assets/boards-connected-card-first-added.png)

1. Klikken ![Taak of probleem openen](assets/boards-launch-icon.png) om de [!DNL Workfront] taak of probleem op een nieuw browsertabblad.
1. Als u de kaartgegevens wilt bewerken, klikt u op de kaart (niet op de kaartnaam).

   of

   Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) op de kaart en selecteer **[!UICONTROL Edit]**.

1. In de **[!UICONTROL Card Details]** de volgende gegevens toevoegen of bijwerken:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td> <p>Als u de naam wijzigt, verandert ook de naam in de verbonden [!DNL Workfront] object.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td> <p>Als u de beschrijving wijzigt, verandert ook de beschrijving op de verbonden [!DNL Workfront] object.</p> </td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignees]</strong></td>
      <td><p>Als u meer personen of een team aan de kaart wilt toewijzen, typt u een naam in het zoekveld en selecteert u de naam wanneer deze in de lijst wordt weergegeven. U kunt zowel personen als teams toevoegen. Er is slechts één teamtoewijzing toegestaan op een aangesloten kaart.</p>
      <p>De kandidaten moeten lid van de raad zijn of zij zullen niet in de selectielijst verschijnen. Als een team lid is in de raad, kunnen de individuele teamleden aan de kaart worden toegewezen.</p>
      <p>Alle geselecteerde toewijzingen worden ook toegewezen aan de taak of uitgave in [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td><p>Selecteer de kolom voor de kaart.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Selecteer een status voor de kaart. De standaardinstellingen zijn [!UICONTROL New], [!UICONTROL In Progress], en [!UICONTROL Complete], maar alle aangepaste statussen die zijn gedefinieerd voor het item in [!DNL Workfront] zijn ook beschikbaar.</p>
      <p>Als u kolombeleid hebt ingeschakeld voor het bijwerken van veldwaarden, wordt bij het wijzigen van de status op de kaart de kaart automatisch naar de corresponderende kolom verplaatst. Zie "Kolominstellingen en beleid definiëren" in het artikel voor meer informatie <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Bordkolommen beheren</a>.</p>
      <p>Als u op <strong>[!UICONTROL Mark Complete]</strong> boven aan de kaart wordt de status automatisch gewijzigd in Voltooid.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td><p>Als u deze datum wijzigt, wordt ook de geplande voltooiingsdatum op de verbonden [!DNL Workfront] object.</p></td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Het aantal uren dat de kaart moet worden ingevuld.</p><p>Als u de optie Aanmelden voor vroege functies gebruikt [!DNL Workfront] [!UICONTROL Boards]Als u de schatting wijzigt, verandert ook de waarde van de artikelpunten in het verbonden object [!DNL Workfront] object.</p><p>Als u niet kiest in de beginfase van functies, is dit alleen een handmatige invoer en mag de waarde niet meer dan 99 zijn.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Zoek naar en selecteer markeringen voor de kaart.</p>
      <p>Voor informatie over het maken van nieuwe tags raadpleegt u <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Tags toevoegen</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist Items]</strong> </td> 
      <td> <p>Klik op <strong>[!UICONTROL Add checklist item]</strong>. Typ vervolgens de titel van het item en druk op Enter. Er wordt automatisch een ander item toegevoegd. Ga door met titels om meer objecten toe te voegen.</p> <p>De teller boven aan de checklist toont het aantal voltooide items en het totale aantal items.</p> <p>Voor meer informatie over controlelijstitems raadpleegt u <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Controlelijstitems op kaarten beheren</a>.</p></td>
     </tr>
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Close]** om terug te keren naar het bestuur.
Het verbonden object, de toewijzingen, de tags, de vervaldatum, de controlelijstteller, de geschatte uren en de status worden weergegeven op de kaart.

   ![Kaart aan boord toegevoegd](assets/boards-connected-card-details-110922.png)

## Verbinding met een aangesloten kaart verbreken

U kunt een aangesloten kaart loskoppelen van het Workfront-object en de kaart blijft op het bord staan als een ad-hockaart die u kunt bewerken.

Verbinding verbreken op het niveau van het board:

1. Toegang tot het bord.
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) op de aangesloten kaart en selecteer **[!UICONTROL Disconnect]**.
1. Klikken **[!UICONTROL Disconnect]** in het bevestigingsbericht.

Verbinding verbreken op kaartniveau:

1. Open de kaart en open deze.
1. Klik op de knop **[!UICONTROL More]** menu ![Het menu Meer](assets/more-icon-spectrum.png) in het gebied Verbinding van de kaartdetails, en selecteer **[!UICONTROL Disconnect]**.
1. Klikken **[!UICONTROL Disconnect]** in het bevestigingsbericht.

## Een ad-hockaart converteren naar een aangesloten kaart

Nadat u een ad-hockaart hebt gemaakt, kunt u deze converteren naar een aangesloten kaart. Voor meer informatie over ad-hockaarten raadpleegt u [Een ad-hockaart aan een kaart toevoegen](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Open de kaart en open de ad-hockaart.
1. Controleer de naam en beschrijving op de kaart. Ze worden toegevoegd aan de taak of uitgave die u maakt in [!DNL Workfront].
1. In de [!UICONTROL Connection] voor meer informatie over de kaart klikt u op **[!UICONTROL Connect with Workfront]**.
1. Op de [!UICONTROL Connect Card] selecteert u of u een taak of een uitgave maakt.
1. Zoek naar en selecteer een project om de taak of kwestie aan toe te voegen.

   >[!NOTE]
   >
   >* Alleen objecten waarvoor u machtigingen hebt, zijn beschikbaar in de zoekresultaten.
   >* Wanneer u filtert op **[!UICONTROL Projects I Own]** of **[!UICONTROL Projects I'm On]**, projecten die overeenkomen met een [!UICONTROL Complete], [!UICONTROL Dead], of [!UICONTROL Rejected] status worden niet opgenomen. U kunt nog steeds naar die projecten zoeken met de **[!UICONTROL All]** filter.


1. Klik op **[!UICONTROL Connect]**.

   ![Ad-hockaart aansluiten op Workfront](assets/boards-connect-ad-hoc-card.png)

   De projectnaam wordt weergegeven in het gebied Verbinding op de kaartdetails.

1. Klikken **[!UICONTROL Close]** om terug te keren naar het bestuur.

## Uren vastleggen op een aangesloten kaart

>[!NOTE]
>
>Deze functie is alleen beschikbaar via de vroege functie opt-in voor Workfront Boards.

U moet over de juiste machtigingen beschikken om de uren te kunnen vastleggen voor de verbonden taak of uitgave.

De velden voor tijdregistratie worden standaard niet weergegeven op verbonden kaarten. U moet [!UICONTROL **Uren**] in de [!UICONTROL Configure] areaal [!UICONTROL Cards]. Zie voor meer informatie [Aanpassen welke velden worden weergegeven op een kaart](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Voer het aantal uren in voor de taak of uitgave.
1. Selecteer een [!UICONTROL Hour Type] in het keuzemenu als dit een andere instelling is dan de standaardinstelling.
1. Klikken [!UICONTROL **Logtijd**].

   ![Loguren op kaart](assets/log-hours-on-card.png)

   De tijd die op de kaart wordt geregistreerd wordt ook bewaard op de verbonden taak of de kwestie.

De registratietijd op de kaart is hetzelfde als de tijd die u nodig hebt om u aan te melden bij een taak of uitgave. Voor meer informatie, zie &quot;tijd van het Logboek op een project, een taak, of een kwestie&quot;in het artikel [Logtijd](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

