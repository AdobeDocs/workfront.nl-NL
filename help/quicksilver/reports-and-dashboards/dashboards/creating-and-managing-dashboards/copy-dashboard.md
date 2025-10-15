---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Een dashboard kopiëren
description: U kunt een dashboard en al zijn inhoud (rapporten, kalenders, en externe pagina's) kopiëren. Wanneer u de inhoud van een dashboard kopieert, kunt u ervoor kiezen deze op het oorspronkelijke dashboard te houden, of nieuwe items te maken die kopieën zijn van de items op het oorspronkelijke dashboard. U kunt er ook voor kiezen om items niet over te brengen of te kopiëren naar het nieuwe dashboard.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 0%

---

# Een dashboard kopiëren

<!-- Audited: 1/2025 -->

U kunt een dashboard en al zijn inhoud (rapporten, kalenders, en externe pagina&#39;s) kopiëren. Wanneer u de inhoud van een dashboard kopieert, kunt u ervoor kiezen deze op het oorspronkelijke dashboard te houden, of nieuwe items te maken die kopieën zijn van de items op het oorspronkelijke dashboard. U kunt er ook voor kiezen om items niet over te brengen of te kopiëren naar het nieuwe dashboard.

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
      <p>Standard</p>
      <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot rapporten, dashboards en kalenders bewerken</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot een dashboard weergeven</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vereisten

U moet een dashboard maken voordat u het kunt kopiëren.

Voor informatie bij het creëren van dashboards, zie [ een dashboard ](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) creëren.

## Een dashboard kopiëren

1. Klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon.png) in de hoger-juiste hoek van Adobe Workfront, of (als beschikbaar), klik het **[!UICONTROL Main Menu]** pictogram ![ Belangrijkste Menu ](/help/_includes/assets/main-menu-icon-left-nav.png) in de upper-left hoek, dan klik **[!UICONTROL Dashboards]**.

1. Selecteer het dashboard dat u wilt kopiëren, dan klik **** het pictogram van het Exemplaar ![.](assets/copy-icon.png)\
   of\
   Open het dashboard dat u wilt kopiëren, dan klik **Acties van het Dashboard** > **Exemplaar**.\
   Het dialoogvenster Kopiëren van dashboard wordt weergegeven. Alle items op het oorspronkelijke dashboard worden weergegeven.

1. Op het **gebied van de Naam van het Dashboard**, specificeer een nieuwe naam voor het dashboard.
1. Om alle punten op het bestaande dashboard te selecteren en hen te kopiëren aan het gekopieerde dashboard, verlaten **Uitgezochte allen** geselecteerd. Standaard worden de rapporten, kalenders of lijsten op het bestaande dashboard naar het nieuwe dashboard gekopieerd.\
   of\
   Als u alleen bepaalde items van het oorspronkelijke dashboard naar het nieuwe dashboard wilt overbrengen, deselecteert u de items die u niet op het nieuwe dashboard wilt weergeven. Voor elk geselecteerd item kiest u een van de volgende opties:

   * **maak een Exemplaar:** het punt wordt gekopieerd van het originele dashboard en een nieuwe versie van dat punt wordt getoond op het nieuwe dashboard. Wijzigingen die worden aangebracht in het item op het nieuwe dashboard, worden niet doorgevoerd in het item op het oorspronkelijke dashboard. Op dezelfde manier worden wijzigingen die zijn aangebracht in het item op het oorspronkelijke dashboard, niet doorgevoerd in het item op het nieuwe dashboard.\
     Gebruik deze optie als u het oorspronkelijke rapport op het oorspronkelijke dashboard wilt wijzigen.\
     Bijvoorbeeld, kopieert u een dashboard genoemd &quot;Team B&quot;en hernoemt het aan &quot;Team A.&quot; Op het dashboard &#39;Team B&#39; staat een rapport met de naam &#39;Team B Report&#39;. Omdat dit rapport gegevens specifiek voor Team B bevat, selecteert u de optie om een exemplaar van dit rapport te maken zodat kunt u het voor Team A aanpassen en het later anders noemen aan &quot;Team A Rapport&quot;.\
     Met deze optie, verwijdert u de het delen toestemmingen van het originele rapport uit het gekopieerde rapport. De looppas dit rapport met de Rechten van de Toegang van informatie blijft intact op het gekopieerde rapport.

   * **Origineel van het Gebruik:** toont het originele punt op het nieuwe dashboard. Wijzigingen die worden aangebracht in het item op het nieuwe dashboard, worden ook doorgevoerd in het item op het oorspronkelijke dashboard. Op dezelfde manier worden wijzigingen die zijn aangebracht in het item op het oorspronkelijke dashboard weerspiegeld in het item op het nieuwe dashboard.\
     Met deze optie, houdt u de het delen toestemmingen van het originele rapport. Dit rapport uitvoeren met de toegangsrechten van informatie blijft ook intact.

1. (Optioneel) Wijzig de naam van geselecteerde items.
1. Klik **Dashboard van het Exemplaar**.
1. (Optioneel) Als u een van de gekopieerde rapporten, kalenders of externe pagina&#39;s op het gekopieerde dashboard wilt bewerken, voert u een van de volgende handelingen uit:

   * Om om het even welke informatie voor om het even welke gekopieerde rapporten uit te geven, klik de rapportnaam op het dashboard, en dan **de Acties van het Rapport** > **uitgeven**.

     U kunt bijvoorbeeld de weergave, Filter, Groepering, Vragen of Diagram of een gekopieerd rapport bewerken.

   * Om toestemmingen op de gekopieerde rapporten opnieuw op te nemen, klik de rapportnaam in het nieuwe dashboard, en klik dan de Acties van het Rapport **>** delend **en werk de toestemmingen op het rapport bij.**

     Wanneer u een rapport kopieert terwijl het kopiëren van een dashboard, worden de toestemmingen op dat rapport verwijderd.

   * Om dit rapport met de Rechten van de Toegang van informatie te wijzigen, klik de naam van het rapport over het nieuwe dashboard, dan **de Acties van het Rapport** > **geeft** > **Opties van het Rapport** uit.\
     Na het kopiëren van een rapport, wordt de Looppas dit rapport met de Rechten van de Toegang van toestemmingen gehandhaafd slechts in de volgende omstandigheden:

     (Als geen van deze voorwaarden waar zijn, dan stel dit rapport met de Rechten van de Toegang van toestemmingen in werking wordt verwijderd, en de nieuwe Looppas dit rapport met de Rechten van de Toegang van wordt veranderd in de gebruiker die het gekopieerde rapport creeerde.)

     Als de gebruiker die het dashboard en zijn rapporten kopieert de toegangsrechten van de Beheerder heeft.

      * Als de gebruiker die het dashboard en zijn rapporten kopieert de toegangsrechten van de Beheerder heeft.
      * Als de gebruiker die het dashboard en zijn rapporten kopieert momenteel als Looppas dit rapport met de Rechten van de Toegang van voor de rapporten wordt geplaatst die worden gekopieerd.
      * Als de gebruiker die het rapport kopieert beheertoestemmingen op het rapport heeft.
