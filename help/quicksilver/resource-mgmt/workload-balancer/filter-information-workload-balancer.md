---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Gegevens in de werklastbalans filteren
description: We raden u ten zeerste aan filters te gebruiken in Workload Balancer om werkitems efficiënt te zoeken en u te concentreren op de gebruikers of items die u beheert.
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: c3cb97a36c29b90bbc9d8438d8811cc23266d894
workflow-type: tm+mt
source-wordcount: '2488'
ht-degree: 0%

---

# Gegevens in de werklastbalans filteren

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Als middelmanager, kunt u de Balancer van de Werkbelasting gebruiken om de werkbelasting van uw gebruikers te bekijken en te beheren. Zie de volgende artikelen voor meer algemene informatie over de werklastbalans:

* [Overzicht van werklastbalans](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>We raden u ten zeerste aan filters te gebruiken in Workload Balancer om werkitems efficiënt te zoeken en u te concentreren op de gebruikers of items die u beheert. Hierdoor kunt u de juiste informatie weergeven voordat u de toewijzingen van uw bronnen gaat beheren.
>
>Wanneer u een nieuw filter opslaat en toepast, navigeert u weg van de Werklastbalans, blijft het filter behouden, zelfs nadat u zich hebt afgemeld en weer hebt aangemeld.

Dit artikel bevat informatie over filters in Workload Balancer. Voor informatie over filters in Workfront raadpleegt u [Overzicht van filters](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Toegangsvereisten

U moet het volgende hebben:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Elk abonnement</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan, wanneer het gebruiken van de Balancer van de Werkbelasting in het gebied van de Middelen</p>
   <p>Het werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een team of een project</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>Toegang tot het volgende weergeven of vergroten:</p> 
    <ul> 
     <li> <p>Bronbeheer</p> </li> 
     <li> <p>Projecten</p> </li> 
     <li> <p>Taken</p> </li> 
     <li> <p>Problemen</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filters, Weergaven en Groepen</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Toegang tot filters, weergaven en groepen bewerken tijdens het maken of bewerken van filters</span> </p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan de projecten, taken, kwesties</p>
   <p>Rechten beheren voor de filters die u wilt bewerken of verwijderen</p>
     </p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Overzicht van filters in de werklastverdeler

Houd rekening met het volgende wanneer u werkt met filters in Workload Balancer:

* Afhankelijk van waar u tot de Balancer van de Werkbelasting van toegang hebt, zou Workfront de informatie voor u reeds kunnen filtreren. Zie de sectie voor informatie over vooraf toegepaste filters [Vooraf toegepaste filters in de werklastverdeler](#pre-applied-filters-in-the-workload-balancer) in dit artikel.
* U kunt een filter maken en toepassen zonder het op te slaan, of u kunt een filter opslaan om later opnieuw te gebruiken.
* Wanneer u een filter toepast zonder het op te slaan, kunt u terugkeren naar de originele lijsten door de pagina te vernieuwen.
* U kunt filters bekijken die u hebt gemaakt of filters die andere gebruikers hebben gemaakt en met u hebben gedeeld.
* Wanneer u een gedeeld filter verwijdert of bewerkt, wordt het filter ook verwijderd of bewerkt voor iedereen met wie het wordt gedeeld.
* Wanneer u in één gebied filters maakt in de werklastbalans, zijn deze niet beschikbaar in andere gebieden.

  Bijvoorbeeld, zijn de filters die in het gebied van de Middelen worden gecreeerd niet beschikbaar in de Balancer van de Werkbelasting van een project of een team.

  Voor informatie over waar te om van de Balancer van de Werkbelasting de plaats te bepalen, zie [De werklastbalans zoeken](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* U kunt alleen de items weergeven die overeenkomen met de geselecteerde filters die ook overeenkomen met de datums in de tijdlijn die op het scherm van Workload Balancer wordt weergegeven.

## Vooraf toegepaste filters in de werklastverdeler {#pre-applied-filters-in-the-workload-balancer}

De werklastbalans geeft informatie in twee afzonderlijke gebieden weer:

* **Het niet toegewezen werkgebied**: werkitems die nog niet aan gebruikers zijn toegewezen.
* **Het toegewezen werkgebied**: de werkpunten die aan gebruikers worden toegewezen.

  Voor informatie over wat in elk van de gebieden toont, zie [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Elk gebied van de werklastbalans heeft een eigen set filters die onafhankelijk van elkaar werken. U moet beide filters configureren om aan te geven welke informatie u in elk gebied wilt zien.

Met Werklastbalans worden gebruikers en hun werkitems weergegeven.
De aan de gebruikers toegewezen werkitems worden alleen weergegeven wanneer de datums van de items overeenkomen met het tijdframe dat op het scherm wordt weergegeven.

Afhankelijk van waar u tot de Balancer van de Werkbelasting toegang hebt, worden de Niet toegewezen en Toegewezen gebieden reeds gefiltreerd door bepaalde criteria, zoals die in de volgende lijst worden beschreven:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Workfront-gebied waar u de werklastbalans kunt openen</strong></td> 
   <td><b>Items die standaard worden weergegeven in het gedeelte Niet toegewezen werk</b> </td> 
   <td><b>Items die standaard worden weergegeven in het gebied Toegewezen werk</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Het gebied met hulpbronnen</td> 
   <td>Er worden hier standaard geen items weergegeven. U moet filters aanpassen om werkitems in dit gebied weer te geven.</td> 
   <td>Gebruikers die lid zijn van een van uw teams en hun werkitems. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een team</td> 
   <td>De punten van het werk die aan het team of het team en een baanrol worden toegewezen. </td> 
   <td> <p>Gebruikers die lid zijn van het geselecteerde team en hun werkitems.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Een project</td> 
   <td> <p>Niet toegewezen het werkpunten of punten die aan teams of baanrollen in de geselecteerde projectvertoning in dit gebied worden toegewezen.</p> </td> 
   <td> <p>De gebruikers die aan minstens één het werkpunt op het geselecteerde project en hun het werkpunten op het project worden toegewezen wanneer het systeem standaardfilter <b>Werkonderdelen van dit project</b> is geselecteerd. </p>

<p>Wanneer het standaardfilter van het systeem <b>Werkonderdelen van dit project</b> is geschrapt, toont het Toegewezen gebied van het Werk van een project alle het werkpunten van de gebruikers die aan minstens één punt op het geselecteerde project worden toegewezen.  </p> Dit filter is standaard uitgeschakeld.

<b>OPMERKING</b>
<p>U kunt de optie Alle gebruikers tonen inschakelen in de werklastverdeling van een project om alle gebruikers in het systeem weer te geven. Zie voor meer informatie <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigeren door werklastbalans</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Werklastverdelingsfilters maken

Het proces voor het maken van filters voor de niet-toegewezen werkgebieden en toegewezen werkgebieden in Workload Balancer is identiek, ongeacht waar u de Workload Balancer opent. Voor informatie over het zoeken naar de werklastbalans raadpleegt u [De werklastbalans zoeken](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

U kunt een geheel nieuw filter maken of een van de vooraf gedefinieerde filters bewerken. Zie voor informatie over bestaande filters die u kunt bewerken de [Een bestaand filter bewerken in het deelvenster Werklastbalans](#edit-an-existing-filter-in-the-workload-balancer) in dit artikel.

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klik op de knop **Filter** pictogram ![](assets/filter-icon.png) in de rechterbovenhoek van een van de **Niet toegewezen werk** of de **Toegewezen werk** gebieden.

   De doos van de filterbouwer toont op het recht. De naam van het gebied waarvoor u het filter maakt, wordt weergegeven in de koptekst van het vak.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Optioneel en voorwaardelijk) Als u de werklastbalans opent in het gebied Bronnen, is het mogelijk dat het vooraf gedefinieerde standaardfilter al wordt toegepast op het gebied Toegewezen werk. U kunt een kopie van het filter Standaard bewerken en opslaan.

   >[!TIP]
   >
   >Met het filter Standaard worden gebruikers weergegeven die tot een van uw teams behoren en hun werkitems. U kunt een kopie van dit filter bewerken.

   Als u toegang hebt tot [!UICONTROL Workload Balancer] van een project[!UICONTROL This project's work items]Het is mogelijk dat het filter al is toegepast. Dit toont slechts het werkpunten die aan gebruikers in dit project worden toegewezen. U kunt een kopie van dit filter dupliceren en opslaan.

   Standaard worden de [!UICONTROL Workload Balancer] van een project toont alle het werkpunten die aan alle gebruikers op het project worden toegewezen.


1. Klikken **Nieuw filter.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Ga als volgt te werk om een filter te maken:

   1. Selecteer een veldnaam in het eerste vervolgkeuzemenu of klik op **Bladeren door velden** om de naam te typen van een veld dat niet standaard wordt weergegeven.

      >[!IMPORTANT]
      >
      >Wanneer u naar aangepaste velden verwijst, moet u de veldnaam en niet het veldlabel typen. Het veldlabel wordt weergegeven op een aangepast formulier dat is gekoppeld aan een object. Zie voor informatie over het verschil tussen het label en de naam van een aangepast veld [Een aangepast formulier maken of bewerken](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Voorwaardelijk) Als u hebt geklikt **Bladeren door velden** typt u de naam van een veld in het dialoogvenster **Zoeken** en selecteert u deze wanneer deze in de lijst wordt weergegeven.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >U kunt een veld selecteren uit de volgende secties:
      >
      >* **Recente selecties**: de velden waarvoor u onlangs hebt gefilterd.
      >* **Voorgestelde velden**: de velden die het meest worden gebruikt.


   1. Selecteer een bepaling van het tweede drop-down menu. Zie voor informatie over Workfront-filtermodifiers [Filters en voorwaardelijke modifiers](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Selecteer of typ een waarde voor het veld waarvoor u filtert.

      >[!NOTE]
      >
      > Wanneer u werkobjecten uit een bepaald portfolio wilt weergeven, kunt u het volgende filter toepassen: &quot;Naam van Portfolio bevat marketing.&quot; Dit toont het werkpunten die tot om het even welke portefeuille behoren die &quot;marketing&quot;in de naam bevat.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

      >[!NOTE]
      >
      >Om projecten in een status van Op Greep uit te sluiten, moet u het volgende filter toepassen: &quot;Project: De status is niet gelijk aan Op Greep.&quot; Dit verhindert het werkpunten op de projecten van de Greep in de Balancer van de Werklast te tonen.

   1. (Optioneel) Klik op de knop **Verwijderen** pictogram ![](assets/delete.png) om filtercriteria te verwijderen.

1. (Optioneel) Klik op **Filter toevoegen** als u nog een filtercriterium wilt toevoegen, herhaalt u de handelingen uit stap 4.

   <!--(NOTE: ensure this stays correct)-->

1. Klikken **Toepassen** om de resultaten van het filter toe te passen op het geselecteerde gebied van de Balans van de Werkbelasting zonder het te bewaren.

   De lijst met werkitems wordt links bijgewerkt.

   >[!IMPORTANT]
   >
   >De resultaten worden weergegeven in Workload Balancer wanneer alle filterinstructies die u hebt toegevoegd, tegelijkertijd true zijn.

   Het filter blijft behouden totdat u de pagina vernieuwt.

   De **Toepassen** knop wordt vervangen door een **Opslaan als nieuw** knop.

1. Klikken **Opslaan als nieuw** om het filter op te slaan voor toekomstig gebruik.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Klikken **Annuleren** neemt u op elk gewenst moment terug naar het gedeelte van het filtergebouw.

1. Selecteren **Naamloos filter** en voer in plaats daarvan de naam van het nieuwe filter in.
1. Selecteer een pictogram voor het nieuwe filter in het menu **Pictogram** vervolgkeuzelijst.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Optioneel) Voeg een beschrijving van het filter toe om aan te geven wat er uniek aan is. De beschrijving wordt onder de filternaam in de lijst met filters weergegeven.
1. Klikken **Opslaan**.

   Opgeslagen filters worden weergegeven in het gedeelte Mijn filters van het filtervak.

   Zie de sectie voor informatie over het toepassen van opgeslagen filters [Een opgeslagen filter verwijderen in Workload Balancer](#delete-a-saved-filter-in-the-workload-balancer) in dit artikel.

1. (Voorwaardelijk) Plaats de muis boven de **Filterpictogram** ![](assets/filter-icon.png) in de rechterbovenhoek van het **Niet toegewezen werk** of de **Toegewezen werk** gebieden om knopinfo weer te geven met de naam of het aantal filters dat momenteel wordt toegepast.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Een filter dupliceren

U kunt een filter dupliceren en bewerken om een nieuw filter te maken.

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klik op de knop **Filter** pictogram ![](assets/filter-icon.png) in de rechterbovenhoek van een van de **Niet toegewezen werk** of de **Toegewezen werk** gebieden.

   De doos van de filterbouwer toont aan het recht. De naam van het gebied waarvoor u het filter maakt, wordt weergegeven in de koptekst van het vak.

1. Klik met de muis op een bestaand filter **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Dupliceren**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Tijdens het bewerken van een filter kunt u op de knop **Meer** in de linkerbenedenhoek van het vak Filter bewerken klikt u op **Dupliceren**.

1. Bewerk de volgende informatie voor het gedupliceerde filter:

   * Naam

     De nieuwe filternaam is standaard &quot;(oorspronkelijke filternaam) Kopiëren&quot;.

   * Pictogram
   * Beschrijving
   * Een van de velden, modifiers of waarden.

1. (Optioneel) Klik op **Filter toevoegen** om meer instructies toe te voegen aan het gedupliceerde filter.
1. Klikken **Opslaan** om het gedupliceerde filter op te slaan in het dialoogvenster **Mijn filters** gebied.

   Het oorspronkelijke filter blijft ongewijzigd en het gedupliceerde filter wordt opgeslagen als een nieuw filter.

## Een bestaand filter bewerken in het deelvenster Werklastbalans {#edit-an-existing-filter-in-the-workload-balancer}

U kunt een opgeslagen filter bewerken in Workload Balancer.

>[!TIP]
>
>Wanneer u een filter bewerkt dat met anderen wordt gedeeld, worden ook de wijzigingen weergegeven die u aanbrengt.

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klik op de knop **Filterpictogram** ![](assets/filter-icon.png) in de rechterbovenhoek van het **Niet toegewezen** of **Toegewezen werk** gebieden.\
   Aan de rechterkant wordt de filterbuilder weergegeven.

1. Plaats de muis boven het filter dat u wilt bewerken en klik op het pictogram **Bewerken** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Voer een van de volgende handelingen uit:

   * Wijzig om het even welke filterverklaringen
   * Klikken **Filter toevoegen** om nieuwe filterinstructies toe te voegen
   * Klik op de knop **Verwijderen** pictogram ![](assets/delete.png) om bestaande filterinstructies te verwijderen.

1. (Optioneel) Klik op **Toepassen**.

   De resultaten worden bijgewerkt in Workload Balancer aan de linkerkant om de wijzigingen aan te tonen die u in het filter hebt aangebracht.

1. Klikken **Opslaan.**

   De resultaten worden bijgewerkt in Workload Balancer aan de linkerkant en het filter wordt bijgewerkt met de nieuwe informatie die u hebt geselecteerd.

## Een opgeslagen filter verwijderen in Workload Balancer {#delete-a-saved-filter-in-the-workload-balancer}

Overweeg het volgende voordat u een filter verwijdert:

* U kunt verwijderde filters niet herstellen.
* Vooraf gedefinieerde filters kunt u niet verwijderen.
* U kunt een niet-opgeslagen filter niet verwijderen. Ze worden automatisch verwijderd nadat ze zijn afgemeld en opnieuw zijn aangemeld bij Workfront.
* Wanneer u een gedeeld filter verwijdert, wordt het ook verwijderd voor alle gebruikers waarmee het wordt gedeeld.
* Nadat u alle opgeslagen filters hebt verwijderd, wordt de werklastbalans weergegeven volgens de oorspronkelijke standaardwaarden.

>[!NOTE]
>
>Wanneer u een filter verwijdert dat met anderen wordt gedeeld, wordt het filter ook voor hen verwijderd.

1. Naar werklastverdeling
1. Klik op de knop **Filterpictogram** ![](assets/filter-icon.png) in de rechterbovenhoek van het **Niet toegewezen werk** of **Toegewezen werk** gebieden.\
   De doos van de filterbouwer toont op het recht.

1. Plaats de muis boven een filter en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Verwijderen**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Tijdens het bewerken van een filter kunt u op de knop **Meer** in de linkerbenedenhoek van het vak Filter bewerken klikt u op **Verwijderen**.

1. (Optioneel) Klik op **Annuleren** om te voorkomen dat de filters worden verwijderd en naar de lijst van filters worden teruggestuurd.
1. Klikken **Verwijderen** om de schrapping te bevestigen.

   Het filter wordt verwijderd voor u en alle gebruikers die hiervoor machtigingen hadden.

## Een filter delen in Workload Balancer

U kunt een filter delen dat u hebt gemaakt of dat met u is gedeeld door andere gebruikers.

Houd rekening met het volgende wanneer u filters deelt in Workload Balancer:

* U kunt filters delen met actieve gebruikers, teams, rollen en bedrijven of u kunt ze zichtbaar maken voor iedereen in uw Workfront-instantie.
* Filters die u deelt in het gebied Bronnen zijn niet zichtbaar in de taakverdeler van een project of een team.
* Werklastverdelingsfilters die u met anderen deelt, zijn niet zichtbaar in andere gebieden van Workfront.

Een filter delen:

1. Naar werklastverdeling
1. Klik op de knop **Filterpictogram** ![](assets/filter-icon.png) in de rechterbovenhoek van het **Niet toegewezen werk** of **Toegewezen werk** gebieden.\
   De doos van de filterbouwer toont op het recht.

1. Plaats de muis boven een filter en klik vervolgens op de knop **Meer** menu ![](assets/more-menu.png)en klik vervolgens op **Delen.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Tijdens het bewerken van een filter kunt u op de knop **Meer** in de linkerbenedenhoek van het vak Filter bewerken klikt u op **Delen**.

   Het dialoogvenster Filter delen wordt weergegeven.

1. De optie **Systeembrede weergave** instellen. Dit geeft iedereen in Workfront toestemming om het filter te bekijken.

   of

   Begin de namen van gebruikers, teams, rollen, groepen, of bedrijven te typen u de filter met in wilt delen **Toegang verlenen aan** veld.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Optioneel) Klik op de pijl naar rechts naast de naam van een entiteit om de machtigingen voor het filter te bewerken en schakel vervolgens de optie **Weergave** of **Beheren** -optie.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Optioneel) Schakel de aanvullende machtigingen voor een entiteit in of uit door een van de volgende handelingen uit te voeren:

   1. Klikken **Weergave** en schakelt u de **Delen** -optie. Deze optie is standaard ingeschakeld.

   1. Klikken **Beheren** en schakelt u **Delen** of de **Verwijderen** -optie. Deze zijn standaard ingeschakeld.

   >[!TIP]
   >
   >Gebruikers kunnen geen hogere machtigingen ontvangen dan hun toegangsniveau. Als zij geen toegang tot Edit filters in hun toegangsniveau hebben, kunnen zij geen toestemmingen ontvangen om een filter te beheren. Workfront schakelt de optie Beheren voor deze gebruikers uit en de optie is grijs.

1. Klikken **Delen**. Het filter wordt gedeeld met de entiteiten u specificeerde.

   De filters die u in de **Gedeeld met mij** gebied van het filtervak.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
