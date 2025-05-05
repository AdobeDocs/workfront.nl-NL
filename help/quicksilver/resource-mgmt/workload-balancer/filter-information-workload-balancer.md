---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Informatie over filters in de werklastverdeling
description: We raden u ten zeerste aan filters te gebruiken in Workload Balancer om werkitems efficiënt te zoeken en u te concentreren op de gebruikers of items die u beheert.
author: Lisa
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 23c6d9335b0adcafc4e2ecdd8ef2d0ab09709fa8
workflow-type: tm+mt
source-wordcount: '2518'
ht-degree: 0%

---

# Gegevens in de werklastbalans filteren

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Als middelmanager, kunt u de Balancer van de Werkbelasting gebruiken om de werkbelasting van uw gebruikers te bekijken en te beheren. Zie de volgende artikelen voor meer algemene informatie over de werklastbalans:

* [ Overzicht van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navigeren door werklastbalans](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>We raden u ten zeerste aan filters te gebruiken in Workload Balancer om werkitems efficiënt te zoeken en u te concentreren op de gebruikers of items die u beheert. Hierdoor kunt u de juiste informatie weergeven voordat u de toewijzingen van uw bronnen gaat beheren.
>
>Wanneer u een nieuw filter opslaat en toepast, navigeert u weg van de Werklastbalans, blijft het filter behouden, zelfs nadat u zich hebt afgemeld en weer hebt aangemeld.

Dit artikel bevat informatie over filters in Workload Balancer. Voor informatie over filters in Workfront, zie [ Overzicht van Filters ](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan, wanneer het gebruiken van de Balancer van de Werkbelasting in het gebied van de Middelen;</br>
       Het werk, wanneer het gebruiken van de Balancer van de Werkbelasting van een team of een project</p></td>
  </tr>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot het volgende weergeven of vergroten:</p> 
    <ul> 
     <li>Bronbeheer</li> 
     <li>Projecten</li> 
     <li>Taken</li> 
     <li>Problemen</li>
     <li>Filters, Weergaven en Groepen</li>
    </ul>
    <p>Toegang tot filters, weergaven en groepen bewerken tijdens het maken of bewerken van filters </p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>De toestemmingen van de mening of hoger aan de projecten, taken, kwesties</p>
   <p>Rechten beheren voor de filters die u wilt bewerken of verwijderen</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Overzicht van filters in de werklastverdeler

Houd rekening met het volgende wanneer u werkt met filters in Workload Balancer:

* Afhankelijk van waar u tot de Balancer van de Werkbelasting van toegang hebt, zou Workfront de informatie voor u reeds kunnen filtreren. Voor informatie over vooraf toegepaste filters, zie de sectie [ vooraf toegepaste filters in de Balancer van de Werkbelasting ](#pre-applied-filters-in-the-workload-balancer) in dit artikel.
* U kunt een filter maken en toepassen zonder het op te slaan, of u kunt een filter opslaan om later opnieuw te gebruiken.
* Wanneer u een filter toepast zonder het op te slaan, kunt u terugkeren naar de originele lijsten door de pagina te vernieuwen.
* U kunt filters bekijken die u hebt gemaakt of filters die andere gebruikers hebben gemaakt en met u hebben gedeeld.
* Wanneer u een gedeeld filter verwijdert of bewerkt, wordt het filter ook verwijderd of bewerkt voor iedereen met wie het wordt gedeeld.
* Wanneer u in één gebied filters maakt in de werklastbalans, zijn deze niet beschikbaar in andere gebieden.

  Bijvoorbeeld, zijn de filters die in het gebied van de Middelen worden gecreeerd niet beschikbaar in de Balancer van de Werkbelasting van een project of een team.

  Voor informatie over waar te om van de Balancer van de Werklast de plaats te bepalen, zie [ plaats van de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* U kunt alleen de items weergeven die overeenkomen met de geselecteerde filters die ook overeenkomen met de datums in de tijdlijn die op het scherm van Workload Balancer wordt weergegeven.

## Vooraf toegepaste filters in de werklastverdeler {#pre-applied-filters-in-the-workload-balancer}

De werklastbalans geeft informatie in twee afzonderlijke gebieden weer:

* **het Niet toegewezen gebied van het Werk**: het werkpunten die nog niet aan gebruikers worden toegewezen.
* **het Toegewezen gebied van het Werk**: het werkpunten die aan gebruikers worden toegewezen.

  Voor informatie over wat vertoningen in elk van de gebieden, zie [ de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

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
   <td><b> Punten die in het Niet toegewezen gebied van het Werk door gebrek </b> tonen </td> 
   <td><b> Punten die op het Toegewezen gebied van het Werk door gebrek </b> tonen </td> 
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
   <td> <p>De gebruikers die aan minstens één het werkpunt op het geselecteerde project en hun het werkpunten op het project worden toegewezen wanneer de het werkpunten van het systeemgebrek <b> van dit project </b> wordt geselecteerd. </p>

<p>Wanneer het systeemstandaardfilter <b> de het werkpunten van dit project </b> wordt geschrapt, toont het Toegewezen gebied van het Werk van een project alle het werkpunten van de gebruikers die aan minstens één punt op het geselecteerde project worden toegewezen.  </p> Dit filter is standaard uitgeschakeld.

<b> NOTA </b>
<p>U kunt de optie Alle gebruikers tonen inschakelen in de werklastverdeling van een project om alle gebruikers in het systeem weer te geven. Voor meer informatie, zie <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref"> de Balancer van de Werkbelasting </a> navigeren</p>

</td> 
  </tr> 
 </tbody> 
</table>

## Werklastverdelingsfilters maken

Het proces voor het maken van filters voor de niet-toegewezen werkgebieden en toegewezen werkgebieden in Workload Balancer is identiek, ongeacht waar u de Workload Balancer opent. Voor informatie over het lokaliseren van de Balancer van de Werkbelasting, zie [ plaats de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

U kunt een geheel nieuw filter maken of een van de vooraf gedefinieerde filters bewerken. Voor informatie over bestaande filters die u kunt uitgeven, zie [ een bestaand filter in de 1&rbrace; sectie van de Balancer van de Werkbelasting &lbrace;in dit artikel uitgeven.](#edit-an-existing-filter-in-the-workload-balancer)

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [ de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

1. Klik het **pictogram van de Filter ![ ](assets/filter-icon.png) pictogram van de Filter** &lbrace;in de hoger-juiste hoek van of het **Niet toegewezen Werk** of de **Toegewezen gebieden van het Werk**.

   De doos van de filterbouwer toont op het recht. De naam van het gebied waarvoor u het filter maakt, wordt weergegeven in de koptekst van het vak.

   ![ lijst van Filters ](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Optioneel en voorwaardelijk) Als u de werklastbalans opent in het gebied Bronnen, is het mogelijk dat het vooraf gedefinieerde standaardfilter al wordt toegepast op het gebied Toegewezen werk. U kunt een kopie van het filter Standaard bewerken en opslaan.

   >[!TIP]
   >
   >Met het filter Standaard worden gebruikers weergegeven die tot een van uw teams behoren en hun werkitems. U kunt een kopie van dit filter bewerken.

   Als u [!UICONTROL Workload Balancer] van een project toegang hebt, zou &quot;[!UICONTROL This project's work items]&quot;filter reeds kunnen worden toegepast. Dit toont slechts het werkpunten die aan gebruikers in dit project worden toegewezen. U kunt een kopie van dit filter dupliceren en opslaan.

   Door gebrek, [!UICONTROL Workload Balancer] van een project toont alle het werkpunten die aan alle gebruikers op het project worden toegewezen.


1. Klik **Nieuwe filter.**

1. Ga als volgt te werk om een filter te maken:

   1. Selecteer een gebiedsnaam in het eerste drop-down menu of klik **doorbladert gebieden** beginnen de naam van een gebied te typen dat niet door gebrek toont.

      >[!IMPORTANT]
      >
      >Wanneer u naar aangepaste velden verwijst, moet u de veldnaam en niet het veldlabel typen. Het veldlabel wordt weergegeven op een aangepast formulier dat is gekoppeld aan een object. Voor informatie over het verschil tussen het etiket en de naam van een douanegebied, zie [ een douaneformulier ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) creëren.

   1. (Voorwaardelijk) als u **klikte doorbladert gebieden**, typ de naam van een gebied op het **3&rbrace; gebied van het Onderzoek &lbrace;en selecteer het wanneer het in de lijst toont.**

      ![ Onderzoek naar een gebied ](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >U kunt een veld selecteren uit de volgende secties:
      >
      >* **Recente selecties**: de gebieden u onlangs voor hebt gefilterd.
      >* **stelde** voor: de gebieden het meest meestal gebruikt.


   1. Selecteer een bepaling van het tweede drop-down menu. Voor informatie over de filterbepalingen van Workfront, zie [ Filters en voorwaardenbepalingen ](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Selecteer of typ een waarde voor het veld waarvoor u filtert.

      >[!NOTE]
      >
      > Wanneer u werkobjecten uit een bepaald portfolio wilt weergeven, kunt u het volgende filter toepassen: &quot;Portfolio-id is gelijk aan &lt; de naam van het portfolio >.&quot;
      >
      >![ de verklaring van de naamfilter van Portfolio ](assets/portfolio-name-filter-statement-wb-350x262.png)
      >
      >Om projecten in een status van Op Greep uit te sluiten, moet u het volgende filter toepassen: &quot;Project: De status is niet gelijk aan Op Greep.&quot; Dit verhindert het werkpunten op de projecten van de Greep in de Balancer van de Werklast te tonen.
      >
      >![ de verklaring van de de statusfilter van het Project ](assets/project-status-filter-statement-wb.png)

   1. (Facultatief) klik het **pictogram van de Schrapping** pictogram ![ pictogram van de Schrapping ](assets/delete.png) om een filtercriteria te verwijderen.

1. (Facultatief) klik **filter** toevoegen om een andere filtercriteria toe te voegen, dan de acties van stap 4 herhalen.

   <!--(NOTE: ensure this stays correct)-->

1. Klik **toepassen** om de resultaten van de filter op het geselecteerde gebied van de Balancer van de Werkbelasting toe te passen zonder het te bewaren.

   De lijst met werkitems wordt links bijgewerkt.

   >[!IMPORTANT]
   >
   >De resultaten worden weergegeven in Workload Balancer wanneer alle filterinstructies die u hebt toegevoegd, tegelijkertijd true zijn.

   Het filter blijft behouden totdat u de pagina vernieuwt.

   **pas** toe knoop wordt vervangen met a **sparen als nieuwe** knoop.

1. Klik **sparen als nieuw** om de filter voor toekomstig gebruik te bewaren.

   ![ filter sparen als ](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Het klikken **annuleert** op elk ogenblik, neemt u terug naar het gebied van de filterbouw.

1. Klik binnen het **Naamloze gebied van de Filter**, en ga de naam van de nieuwe filter in.
1. (Optioneel) Selecteer een pictogram voor het nieuwe filter in het vervolgkeuzemenu **Pictogram** .

   ![ Uitgezochte pictogram ](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Optioneel) Voeg een beschrijving van het filter toe om aan te geven wat er uniek aan is. De beschrijving wordt onder de filternaam in de lijst met filters weergegeven.
1. Klik **sparen**.

   Opgeslagen filters worden weergegeven in het gedeelte Mijn filters van het filtervak.

   Voor informatie over het toepassen van bewaarde filters, zie de sectie [ een bewaarde filter in de Balancer van de Werkbelasting ](#delete-a-saved-filter-in-the-workload-balancer) in dit artikel schrappen.

1. (Voorwaardelijk) Muis over het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-icon.png) in de hoger-juiste hoek van het **Niet toegewezen Werk** of de **Toegewezen gebieden van het Werk** om tooltip met de naam of het aantal filters te tonen die momenteel worden toegepast.

   ![ pictogram van de Filter met naam van filter ](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Een filter dupliceren

U kunt een filter dupliceren en bewerken om een nieuw filter te maken.

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [ de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

1. Klik het **pictogram van de Filter ![ ](assets/filter-icon.png) pictogram van de Filter** &lbrace;in de hoger-juiste hoek van of het **Niet toegewezen Werk** of de **Toegewezen gebieden van het Werk**.

   De doos van de filterbouwer toont aan het recht. De naam van het gebied waarvoor u het filter maakt, wordt weergegeven in de koptekst van het vak.

1. De muis over een bestaand filter, klikt **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Dupliceert**.

   ![ Filter meer menuopties ](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Terwijl het uitgeven van een filter, kunt u het **Meer** menu in de laag-linkerhoek van de Edit doos van de Filter klikken dan **Dupliceert**.

1. Bewerk de volgende informatie voor het gedupliceerde filter:

   * Naam

     De nieuwe filternaam is standaard &quot;(oorspronkelijke filternaam) Kopiëren&quot;.

   * Pictogram
   * Beschrijving
   * Een van de velden, modifiers of waarden.

1. (Facultatief) klik **filter** toevoegen om meer verklaringen aan de gedupliceerde filter toe te voegen.
1. Klik **sparen** om de gedupliceerde filter in het **Mijn filters** gebied te bewaren.

   Het oorspronkelijke filter blijft ongewijzigd en het gedupliceerde filter wordt opgeslagen als een nieuw filter.

## Een bestaand filter bewerken in het deelvenster Werklastbalans {#edit-an-existing-filter-in-the-workload-balancer}

U kunt een opgeslagen filter bewerken in Workload Balancer.

>[!TIP]
>
>Wanneer u een filter bewerkt dat met anderen wordt gedeeld, worden ook de wijzigingen weergegeven die u aanbrengt.

1. Ga naar Werklastverdeling.

   Voor informatie over de toegang tot van de Balancer van de Werkbelasting, zie [ de Balancer van de Werkbelasting ](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) navigeren.

1. Klik het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-icon.png) in de hoger-juiste hoek van de **Niet toegewezen** of **toegewezen gebieden van het Werk**.\
   Aan de rechterkant wordt de filterbuilder weergegeven.

1. De muis over de filter u wilt uitgeven, dan klikken **geeft** ![ uit geeft filterpictogram ](assets/wb-edit-filter-icon.png) uit.

   ![ Filter Meer menu ](assets/filter-more-menu-options-wb.png)

1. Voer een van de volgende handelingen uit:

   * Wijzig om het even welke filterverklaringen
   * Klik **filter** toevoegen om nieuwe filterverklaringen toe te voegen
   * Klik het **pictogram van de Schrapping** pictogram ![ pictogram van de Schrapping ](assets/delete.png) om bestaande filterverklaringen te verwijderen.

1. (Optioneel) Klik op **Toepassen** .

   De resultaten worden bijgewerkt in Workload Balancer aan de linkerkant om de wijzigingen aan te tonen die u in het filter hebt aangebracht.

1. Klik **sparen.**

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
1. Klik het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-icon.png) in de hoger-juiste hoek van het **Niet toegewezen Werk** of **Toegewezen Gebieden van het Werk**.\
   De doos van de filterbouwer toont op het recht.

1. De muis over een filter, klikt dan **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Schrapping**.
   ![ Filter Meer menu ](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Terwijl het uitgeven van een filter, kunt u het **Meer** menu in de laag-linkerhoek van de Edit doos van de Filter klikken dan **Schrapping**.

1. (Facultatief) klik **annuleert** om de schrapping te vermijden en aan de lijst van filters terug te keren.
1. Klik **Schrapping** om de schrapping te bevestigen.

   Het filter wordt verwijderd voor u en alle gebruikers die hiervoor machtigingen hadden.

## Een filter delen in Workload Balancer

U kunt een filter delen dat u hebt gemaakt of dat met u is gedeeld door andere gebruikers.

Houd rekening met het volgende wanneer u filters deelt in Workload Balancer:

* U kunt filters delen met actieve gebruikers, teams, rollen en bedrijven of u kunt ze zichtbaar maken voor iedereen in uw Workfront-instantie.
* Filters die u deelt in het gebied Bronnen zijn niet zichtbaar in de taakverdeler van een project of een team.
* Werklastverdelingsfilters die u met anderen deelt, zijn niet zichtbaar in andere gebieden van Workfront.

Een filter delen:

1. Naar werklastverdeling
1. Klik het **pictogram van de Filter** ![ pictogram van de Filter ](assets/filter-icon.png) in de hoger-juiste hoek van het **Niet toegewezen Werk** of **Toegewezen Gebieden van het Werk**.\
   De doos van de filterbouwer toont op het recht.

1. De muis over een filter, klikt dan het **Meer** menu ![ Meer menu ](assets/more-menu.png), dan klik **Aandeel.**

   ![ Filter Meer menu ](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Terwijl het uitgeven van een filter, kunt u het **Meer** menu in de laag-linkerhoek van de Edit doos van de Filter klikken dan **Aandeel**.

   Het dialoogvenster Filter delen wordt weergegeven.

1. Laat het **systeem-brede Mening** plaatsen toe. Dit geeft iedereen in Workfront toestemming om het filter te bekijken.

   of

   Begin de namen van gebruikers, teams, rollen, groepen, of bedrijven te typen die u de filter met in **wilt delen geef toegang tot** gebied.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Facultatief) klik de juist-richt pijl naast de naam van een entiteit om hun toestemmingen aan de filter uit te geven, dan of toelaten de **Mening** of **leiden** optie.

   ![ toestemmingen van de Filter ](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Optioneel) Schakel de aanvullende machtigingen voor een entiteit in of uit door een van de volgende handelingen uit te voeren:

   1. Klik **Mening** en maak de **optie van het Aandeel** onbruikbaar. Deze optie is standaard ingeschakeld.

   1. Klik **leiden** en maak of het **Aandeel** of de **Schrapping** optie onbruikbaar. Deze zijn standaard ingeschakeld.

   >[!TIP]
   >
   >Gebruikers kunnen geen hogere machtigingen ontvangen dan hun toegangsniveau. Als zij geen toegang tot Edit filters in hun toegangsniveau hebben, kunnen zij geen toestemmingen ontvangen om een filter te beheren. Workfront schakelt de optie Beheren voor deze gebruikers uit en de optie is grijs.

1. Klik **Aandeel**. Het filter wordt gedeeld met de entiteiten u specificeerde.

   De filters u vertoning in **deelde met me** gebied van de filterdoos.

   ![ Gedeeld met me ](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![Filter icon](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![Favorites icon](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
