---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Creeer, geef, en deel Systeem-brede Filters uit, Meningen, en Groepen
description: U kunt standaardfilters, -weergaven en -groepen maken en deze vervolgens beschikbaar maken voor gebruikers in uw organisatie.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Systeembrede filters, weergaven en groepen maken, bewerken en delen

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

U kunt filters, weergaven en groeperingen maken en deze beschikbaar stellen voor gebruikers in uw hele organisatie.

Wanneer u systeembrede filters, weergaven en groeperingen maakt, zoals beschreven in dit artikel, kunnen gebruikers met wie u ze deelt, deze benutten bij het bekijken van hun lijsten. Gebruikers kunnen hun eigen filters, weergaven en groepen maken op basis van de filters, groepen en groepen die u maakt, maar ze kunnen deze niet rechtstreeks wijzigen.

Houd er rekening mee dat de filters, weergaven en groepen die u voor het hele systeem maakt, verschillen van de standaardfilters, -weergaven en -groepen die Adobe Workfront automatisch voor u maakt in het systeem. Deze standaardfilters, -weergaven en -groeperingen kunnen niet worden bewerkt of verwijderd.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filters, weergaven of groepen maken

{{step-1-to-setup}}


1. Klik op **[!UICONTROL Interface]** en vervolgens op een van de volgende opties: **[!UICONTROL Filters]** , **[!UICONTROL Views]** of **[!UICONTROL Groupings]** .

1. Als u een filter, weergave of groep maakt, klikt u op **[!UICONTROL Add Filter]** , **[!UICONTROL Add View]** of **[!UICONTROL Add Grouping]** en selecteert u het objecttype waaraan u het nieuwe filter, de nieuwe weergave of de nieuwe groep wilt koppelen.

   of

   Als u een bestaand filter, mening, of groepering uitgeeft, selecteer het, dan klik het **[!UICONTROL Edit]** pictogram ![&#x200B; uitgeven pictogram &#x200B;](assets/edit-icon.png).

1. Configureer het filter, de weergave of de groep.

   Zie een van de volgende artikelen voor informatie over beschikbare opties:

   * [&#x200B; Overzicht van Filters &#x200B;](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [&#x200B; Overzicht van weergaven in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Overzicht van groepen in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klik op **[!UICONTROL Save]** in de linkerbenedenhoek.

U kunt het filter, de mening, of de groepering ter beschikking stellen van gebruikers in uw systeem. Voor meer informatie over het delen van filters, meningen of groeperingen met andere gebruikers, zie de sectie [&#x200B; filters, meningen, of groeperingen van de Maken beschikbaar aan gebruikers &#x200B;](#make-filters-views-or-groupings-available-to-users) in dit artikel.


## Filters, weergaven of groepen beschikbaar maken voor alle gebruikers {#make-filters-views-or-groupings-available-to-users}

U kunt ervoor kiezen om filters, weergaven of groepen in het systeem weer te geven of te verbergen. Zichtbare filters zijn beschikbaar voor alle gebruikers in het hele systeem. Deze instelling fungeert als een aan/uit-schakelaar voor het gehele systeem, inclusief de Lay-outsjabloon.

Als u filters, weergaven of groepen van specifieke gebruikers wilt verbergen, raden we u aan een lay-outsjabloon te gebruiken in plaats van deze voor het hele systeem uit te schakelen.

>[!NOTE]
>
>* Als een gebruiker actief een filter, mening, of groepering en dan een beheerder het onbruikbaar maakt, heeft de gebruiker nog toegang tot tot zij een nieuwe filter, mening, of groepering kiezen. Nadat ze een nieuwe hebben gekozen, kunnen ze niet meer terugkeren naar de verborgen versie.
>* Als alle filters, weergaven en groepen zijn beperkt via het Lay-outsjabloon of zijn uitgeschakeld op het hele systeem, ziet de gebruiker de standaardopties, omdat het systeem iets moet weergeven.

Filters, weergaven of groepen weergeven of verbergen:

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Interface]** en vervolgens op een van de volgende opties: **[!UICONTROL Filters]** , **[!UICONTROL Views]** of **[!UICONTROL Groupings]** .

1. (Voorwaardelijk) Selecteer het filter, de weergave of de groep die u beschikbaar wilt maken voor gebruikers en klik op **[!UICONTROL Enable system-wide]** .

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Als u het filter, de weergave of de groep beschikbaar wilt houden voor de meeste gebruikers maar deze wilt verbergen voor andere gebruikers, kunt u de Indelingssjabloon gebruiken. Voor meer informatie, zie [&#x200B; Filters, Mening, en Groepen aanpassen gebruikend een lay-outmalplaatje &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Voorwaardelijk) Selecteer het filter, de mening, of de groep die u voor gebruikers wilt verbergen, dan klik **[!UICONTROL Disable system-wide]**. Het filter, de weergave of de groepering is nu verborgen in zowel de lay-outsjabloon als in gebruikers op het systeem.


## Aangepaste filters, weergaven of groepen delen met specifieke gebruikers

In deze stappen wordt uitgelegd hoe u aangepaste filters, weergaven en groepen kunt delen met specifieke gebruikers via het dialoogvenster Delen in het [!UICONTROL Interface] -gebied in [!UICONTROL Setup] . U kunt toegang verlenen aan of beheren tot filters, weergaven en groepen die u of anderen maken. U kunt systeemstandaardinstellingen niet delen met gebruikers.


{{step-1-to-setup}}

1. Klik op **[!UICONTROL Interface]** en vervolgens op een van de volgende opties: **[!UICONTROL Filters]** , **[!UICONTROL Views]** of **[!UICONTROL Groupings]** .

1. Selecteer de filter, de mening, of het groeperen die u wilt delen, dan het **[!UICONTROL Share]** pictogram ![&#x200B; pictogram van het Aandeel &#x200B;](assets/share-icon.png) klikken.
1. Typ de naam van specifieke gebruikers, teams, rollen, groepen of bedrijven om het filter, de weergave of de groep met te delen. Klik vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   Voor meer informatie over het delen, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Kies **Mening** of **leiden** naast de naam van de gebruiker, het team, de rol, de groep, of het bedrijf. Als u machtigingen wilt verfijnen, klikt u op het schuifregelaarpictogram en past u de machtigingen aan.

   ![&#x200B; verfijnen toestemmingen &#x200B;](assets/fine-tune-permissions.png)

1. Klik op **[!UICONTROL Save]**. Gebruikers die u hebt opgegeven, kunnen nu interactie aangaan met het filter, de weergave of de groep wanneer zij het objecttype bekijken waaraan u het hebt gekoppeld.


## Filters, weergaven en groepen verwijderen

{{step-1-to-setup}}

1. Klik op **[!UICONTROL Interface]** en vervolgens op een van de volgende opties: **[!UICONTROL Filters]** , **[!UICONTROL Views]** of **[!UICONTROL Groupings]** .

1. Selecteer één of meerdere punten in de lijst, dan klik het **[!UICONTROL Delete]** pictogram ![&#x200B; pictogram van de Schrapping &#x200B;](assets/delete.png).

1. In de **Schrapping** dialoogdoos die verschijnt, klik **ja, schrap het**.
