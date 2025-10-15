---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Een inlaatkolom aan een kaart toevoegen
description: U kunt desgewenst een inlaatkolom toevoegen aan uw board die taken en problemen automatisch ophaalt als verbonden kaarten wanneer deze worden toegevoegd in Workfront, op basis van filters die u definieert.
author: Courtney
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '1004'
ht-degree: 0%

---

# Een inlaatkolom aan een bord toevoegen

<!-- Audited: 5/2025 -->

U kunt desgewenst een inlaatkolom aan uw board toevoegen die taken en problemen automatisch ophaalt als verbonden kaarten wanneer deze worden toegevoegd in [!DNL Workfront] op basis van filters die u definieert. De innamekolom kan als backlogkolom voor een team Kanban, een innamelocatie voor een steunteam dienen om kwesties te zien aangezien zij aan een verzoekrij, of een ander doel worden toegevoegd u wenst.

Er is slechts één inlaatkolom toegestaan op een bord en deze wordt altijd weergegeven als de meest linkse kolom.

De inlaatkolom is niet beschikbaar op een dynamisch bord. U kunt echter wel de filters bijwerken waarmee wordt gedefinieerd welke kaarten op een dynamische kaart worden geplaatst. Wanneer u deze filters wijzigt op een dynamisch bord, worden de kaartinstellingen die geen deel uitmaken van de Workfront-taak of -uitgave (zoals codes), opnieuw ingesteld.

>[!NOTE]
>
>Om veiligheidsredenen kan alleen de eigenaar van een board de bordfilters wijzigen in het deelvenster Configureren.

De inlaatkolom is beperkt tot 300 taken en 300 problemen. De standaardvolgorde van items in de inlaatkolom is als volgt:

Taken:

* Primaire bestelling: Projectnaam
* Secundaire volgorde: structuur van werkverdeling

Problemen:

* Primaire bestelling: Projectnaam
* Secundaire volgorde: Referentienummer

>[!IMPORTANT]
>
>Het wordt aanbevolen om het bord regelmatig te vernieuwen als meerdere gebruikers tegelijkertijd aan het bord werken. Door de pagina te vernieuwen, kunt u de visuele wijzigingen op het bord up-to-date houden en voorkomen dat problemen zoals dubbele kaarten uit de inlaatkolom naar het bord worden verplaatst.
>
>Als u wilt synchroniseren met Workfront en nieuwe taken en problemen wilt overbrengen naar het board of de inlaatkolom, klikt u op het menu Meer ![[!UICONTROL More menu]](assets/more-menu.png) naast de naam van het board en selecteert u de optie Gekoppelde items synchroniseren.

Voor meer informatie over kolommen, zie [&#x200B; de kolommen van het Comité beheren &#x200B;](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Voor informatie over verbonden kaarten, zie [&#x200B; Gebruik verbonden kaarten op raad &#x200B;](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> 
   <p>Medewerker of hoger</p> 
   <p>Aanvraag of hoger</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Een inlaatkolom maken met eenvoudige filters

{{step1-to-boards}}

1. Selecteer een board op het dashboard.
1. Klik **vormen** op het recht van de raad om **te openen** paneel vormt.
1. Selecteer de **raad** sectie. Er worden nieuwe velden weergegeven.
1. Zet **dynamisch innamepunten aan raad** aan. De lege inlaatkolom wordt aan de linkerkant van het bord weergegeven.

   ![&#x200B; de kolom van de Inname eenvoudige filteropties &#x200B;](assets/board-section.png)

1. (Facultatief) Onderzoek naar en selecteer [!DNL Workfront] [!UICONTROL **Projecten**].
1. (Facultatief) Onderzoek naar en selecteer gebruiker of team [!UICONTROL **Taken**].
1. Klik **toepassen**. De objecten worden in de innamekolom van het bord weergegeven als verbonden kaarten.

   ![&#x200B; Intake kolom &#x200B;](assets/intake-column-added3.png)

## Een inlaatkolom maken met behulp van geavanceerde filters

{{step1-to-boards}}

1. Selecteer een board op het dashboard.
1. Klik **vormen** op het recht van de raad om **te openen** paneel vormt.
1. Selecteer de **raad** sectie. Er worden nieuwe velden weergegeven.
1. Zet **dynamisch innamepunten aan raad** aan. De lege inlaatkolom wordt aan de linkerkant van het bord weergegeven.

1. Klik [!UICONTROL **Geavanceerde filters van het Gebruik**].

1. Klik op **[!UICONTROL Add filter sources]** en selecteer vervolgens **[!UICONTROL Tasks]** of **[!UICONTROL Issues]** .

   ![&#x200B; de kolom Geavanceerde filteropties van de Neem &#x200B;](assets/add-filter-sources-options.png)

   >[!NOTE]
   >
   >U kunt de inlaatkolom filteren om zowel taken als problemen op te nemen, maar u moet de filters voor elk objecttype afzonderlijk instellen.
   >
   >Bovendien zijn opgeslagen filters en standaardfilters van het systeem beschikbaar voor u om te selecteren.

1. Klik op **[!UICONTROL New filter]** in het filterdeelvenster.

1. Maak het filter en klik op **[!UICONTROL Save as new]** .

   ![&#x200B; Bouwer van de Filter &#x200B;](assets/intake-filter-dialog6.png)

   In het bovenstaande voorbeeld wordt een filter getoond voor taken van een specifiek project die de status [!UICONTROL New] of [!UICONTROL In Progress] hebben.

   >[!NOTE]
   >
   >Het wordt geadviseerd om &quot;me&quot;(het programma geopende gebruiker) geen vervanging op een bordeelfilter te gebruiken, omdat het niet gegarandeerd is om taken of kwesties voor de het programma geopende gebruiker altijd te tonen. Nadat de raad opstelling met de correcte taken en de kwesties is, kunt u de raad filtreren om punten voor een specifieke toegewezen te tonen. Voor meer informatie, zie [&#x200B; Filter en onderzoek in een raad &#x200B;](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   Voor meer details over de bouw van een filter, zie de sectie creeer of geef een filter in de standaardbouwer in artikel uit [&#x200B; creeer of geef filters in  [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md) uit.

1. Geef het filter een naam en klik op **[!UICONTROL Save]** . Het filter wordt weergegeven in de lijst met opgeslagen filters en wordt automatisch toegepast op de inlaatkolom.

   ![&#x200B; het ingaan van een nieuwe filternaam &#x200B;](assets/save-as-modal.png)

1. Klik op de X boven aan het filterdeelvenster om het te sluiten.

1. (Facultatief) om de filter met anderen te delen, over de bewaarde filter te bewegen, het **[!UICONTROL More]** menu ![&#x200B; Meer menupictogram &#x200B;](assets/more-menu.png) te klikken, en **[!UICONTROL Share]** te selecteren. Kies de gebruikers of de teams met in het **delen van de Filter** doos te delen. Voor meer informatie, zie [&#x200B; een filter, mening, of groepering &#x200B;](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md) delen.
1. (Optioneel) Als u zowel taken als problemen in de inlaatkolom wilt opnemen, klikt u op **[!UICONTROL Filter sources]** en selecteert u het andere object om een ander filter te maken.
1. Wanneer u klaar bent met het toevoegen van filters, bekijkt u de inlaatkolom om te controleren of de juiste taken en problemen worden weergegeven.

   ![&#x200B; Intake kolom &#x200B;](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >U kunt de filters op elk gewenst moment bijwerken door het deelvenster Configureren te openen, op **[!UICONTROL Filter sources]** te klikken en **[!UICONTROL Tasks]** of **[!UICONTROL Issues]** te selecteren.

## De inlaatkolom gebruiken

Kaarten in de inlaatkolom kunnen pas worden bewerkt als u ze naar andere boardkolommen verplaatst. U kunt op de kaart klikken om het in een read-only mening te openen, of ![&#x200B; Open taak of kwestie &#x200B;](assets/boards-launch-icon.png) te klikken om de taak of de kwestie in een nieuwe browser tabel te openen.

U kunt de volgorde van de items in de inlaatkolom handmatig wijzigen.

De pictogrammen op de bovenkant recht van de inlaatkolom tonen u hoeveel kaarten momenteel in de kolom zijn, en hoeveel filters worden toegepast.

1. (Facultatief) om naar een punt in de inlaatkolom te zoeken, klik ![&#x200B; pictogram van het Onderzoek &#x200B;](assets/search-icon.png) op de kolom.
1. (Optioneel) Als u een kaart van de inlaatkolom naar een andere kolom wilt verplaatsen, sleept u de kaart naar de gewenste positie.

   of

   Klik het **[!UICONTROL More]** menu ![&#x200B; Meer menupictogram &#x200B;](assets/more-menu.png) op de kaart, en selecteer **[!UICONTROL Move]**. Dan, op het **vakje van het Punt van de Beweging []**, kies een andere kolom en selecteer **[!UICONTROL Move]**.

1. (Facultatief) om de inputkolom te schrappen, klik het **[!UICONTROL More]** menu ![&#x200B; Meer menupictogram &#x200B;](assets/more-menu.png) en selecteer **[!UICONTROL Delete]**.
