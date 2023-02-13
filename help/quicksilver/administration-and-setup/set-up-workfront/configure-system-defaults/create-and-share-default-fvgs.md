---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Standaardfilters, weergaven en groepen maken, bewerken en delen
description: U kunt standaardfilters, -weergaven en -groepen maken en deze vervolgens beschikbaar maken voor gebruikers in uw organisatie.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '767'
ht-degree: 0%

---

# Standaardfilters, weergaven en groepen maken, bewerken en delen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

U kunt standaardfilters, -weergaven en -groepen maken en deze vervolgens beschikbaar maken voor gebruikers in uw organisatie.

Wanneer u standaardfilters, -weergaven en -groepen maakt, zoals in dit artikel wordt beschreven, kunnen gebruikers met wie u ze deelt, deze benutten bij het weergeven van hun lijsten. Gebruikers kunnen hun eigen filters, weergaven en groepen maken op basis van de filters, groepen en groepen die u maakt, maar ze kunnen de filters, weergaven en groepen die u maakt, niet rechtstreeks wijzigen.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standaardfilters, -weergaven of -groepen maken

{{step-1-to-setup}}

1. Voer een van de volgende handelingen uit, afhankelijk van het feit of u een filter, weergave of groep maakt of bewerkt:

   * Klik op **[!UICONTROL Interface]** > **[!UICONTROL Filters]**.

   * Klik op **[!UICONTROL Interface]>** **[!UICONTROL Views]**.

   * Klik op **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**.

1. Als u een filter, weergave of groep maakt, klikt u op **[!UICONTROL Add Filter]**, **[!UICONTROL Add View]**, of **[!UICONTROL Add Grouping]** Selecteer vervolgens het objecttype waaraan u het nieuwe filter, de nieuwe weergave of de nieuwe groep wilt koppelen.

   of

   Als u een bestaand filter, een bestaande weergave of een bestaande groep bewerkt, selecteert u deze en klikt u op de knop **[!UICONTROL Edit]** pictogram ![Pictogram Bewerken](assets/edit-icon.png).

1. Configureer het filter, de weergave of de groep.

   Zie een van de volgende artikelen voor informatie over beschikbare opties:

   * [Overzicht van filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Overzicht van weergaven in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Overzicht van groepen in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klikken **[!UICONTROL Save]** in de linkerbenedenhoek.

U kunt het filter, de mening, of de groepering ter beschikking stellen van gebruikers in uw systeem. Zie de sectie voor meer informatie over het delen van filters, weergaven of groepen met andere gebruikers [Filters, weergaven of groepen beschikbaar maken voor gebruikers](#make-filters-views-or-groupings-available-to-users) in dit artikel.


## Filters, weergaven of groepen tonen of verbergen die beschikbaar zijn via de sjabloon Indeling

U kunt filters, weergaven of groepen weergeven of verbergen in de sjabloon Indeling. Zichtbare filters zijn beschikbaar voor alle gebruikers in het hele systeem. Met een lay-outsjabloon kunt u zichtbare filters voor bepaalde gebruikers of groepen verbergen.

>[!NOTE]
>
>Als een gebruiker actief een filter, mening, of groepering en dan een beheerder het onbruikbaar maakt, heeft de gebruiker nog toegang tot tot zij een nieuwe filter, mening, of groepering kiezen. Nadat ze een nieuw filter, een nieuwe weergave of een nieuwe groep hebben gekozen, kunnen ze niet meer terugkeren naar het verborgen filter, de verborgen weergave of de verborgen groep.

Filters, weergaven of groepen die beschikbaar zijn in de Lay-outsjabloon weergeven of verbergen:

1. Klikken **[!UICONTROL Interface]** en klikt u op een van de volgende opties: **[!UICONTROL Filters]**, **[!UICONTROL Views]**, of **[!UICONTROL Groupings]**.

1. (Voorwaardelijk) Selecteer het filter, de weergave of de groep die u beschikbaar wilt maken voor gebruikers, en klik vervolgens op **[!UICONTROL Enable system-wide]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Als u het filter, de weergave of de groep beschikbaar wilt houden voor de meeste gebruikers, maar deze voor anderen wilt verbergen, kunt u het Lay-outsjabloon gebruiken. Zie voor meer informatie [Filters, weergaven en groepen aanpassen met een lay-outsjabloon](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Voorwaardelijk) Selecteer het filter, de mening, of de groep die u wilt maken verbergen voor gebruikers, dan klik **[!UICONTROL Disable system-wide]**. Als deze optie is uitgeschakeld, worden het filter, de weergave of de groep verborgen achter de lay-outsjabloon en gebruikers in het hele systeem.


## Filters, weergaven of groepen beschikbaar maken voor alle gebruikers {#make-filters-views-or-groupings-available-to-users}

In deze stappen wordt uitgelegd hoe u filters, weergaven en groepen beschikbaar kunt maken in het dialoogvenster [!UICONTROL Share] in het dialoogvenster [!UICONTROL Interface] gebied in [!UICONTROL Setup]. Deze instelling fungeert als een aan/uit-schakelaar voor het gehele systeem, inclusief de Lay-outsjabloon.

{{step-1-to-setup}}

1. Klikken **[!UICONTROL Interface]** en klikt u op een van de volgende opties: **[!UICONTROL Filters]**, **[!UICONTROL Views]**, of **[!UICONTROL Groupings]**.

1. Selecteer het filter, de weergave of de groep die u beschikbaar wilt maken voor gebruikers en klik op de knop **[!UICONTROL Share]** pictogram ![Pictogram Delen](assets/share-icon.png) om de [!UICONTROL Filter Access], [!UICONTROL View Access], of [!UICONTROL Grouping Access] formulier.
1. (Voorwaardelijk) Als u het filter, de weergave of de groep beschikbaar wilt maken voor alle gebruikers in het systeem, klikt u op de knop **[!UICONTROL Gear]** vervolgkeuzemenu ![](assets/gear-menu-for-sharing-items.png)en klik vervolgens op **[!UICONTROL Make this visible system-wide]**. Alle gebruikers in het systeem kunnen het filter, de mening, of de groepering nu zien.

   of

   Typ de naam van specifieke gebruikers, teams, rollen, groepen of bedrijven om het filter, de weergave of de groep met te delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   Zie voor meer informatie over delen [Overzicht van het delen van machtigingen voor objecten](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klik op **[!UICONTROL Save]**.

   Gebruikers die u hebt opgegeven, kunnen nu het standaardfilter, de standaardweergave of de standaardgroep zien wanneer ze het objecttype bekijken waaraan u het hebt gekoppeld.

## Filters, weergaven en groepen verwijderen

{{step-1-to-setup}}

1. Voer een van de volgende handelingen uit, afhankelijk van het feit of u een filter, weergave of groep verwijdert:

   * Klik op **[!UICONTROL Interface]** > **[!UICONTROL Filters]**

   * Klik op **[!UICONTROL Interface]** > **[!UICONTROL Views]**

   * Klik op **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**

1. Selecteer een of meer items in de lijst en klik op de knop **[!UICONTROL Delete]** pictogram ![Pictogram Verwijderen](assets/delete.png).
1. Zie een van de volgende artikelen voor gedetailleerde informatie over het configureren van een filter, weergave of groepering.

   * [Overzicht van filters in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Overzicht van weergaven in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Overzicht van groepen in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
