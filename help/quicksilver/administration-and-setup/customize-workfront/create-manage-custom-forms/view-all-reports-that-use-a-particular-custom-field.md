---
title: Alle rapporten weergeven die een bepaald aangepast veld of een bepaalde widget gebruiken
description: U kunt een aangepaste weergave toevoegen in het gebied Aangepaste Forms, waarin wordt aangegeven welke rapporten een bepaald aangepast veld of een bepaalde widget gebruiken. Dit is handig wanneer u het veld of de widget moet bewerken of verwijderen, omdat deze mogelijk al in een of meer rapporten is geïmplementeerd. Het is belangrijk om te beoordelen of die rapporten aanpassingen zullen nodig hebben om behoorlijk te blijven werken.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Alle rapporten weergeven die een bepaald aangepast veld of een bepaalde widget gebruiken

U kunt een aangepaste weergave toevoegen in het gebied Aangepaste Forms, waarin wordt aangegeven welke rapporten een bepaald aangepast veld of een bepaalde widget gebruiken. Dit is handig wanneer u het veld of de widget moet bewerken of verwijderen, omdat deze mogelijk al in een of meer rapporten is geïmplementeerd. Het is belangrijk om te beoordelen of die rapporten aanpassingen zullen nodig hebben om behoorlijk te blijven werken.

Voor informatie over aangepaste velden en widgets in aangepaste formulieren raadpleegt u [Een aangepast veld toevoegen aan een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) en [Een middelenwidget toevoegen of bewerken in een aangepast formulier](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-abonnement*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p> <p>Ga voor informatie over hoe Workfront-beheerders deze toegang verlenen naar <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gebruikers administratieve toegang verlenen tot bepaalde gebieden</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, type licentie of configuraties op toegangsniveau u hebt.

## Een lijst weergeven van de rapporten die een bepaald aangepast veld of een bepaalde aangepaste widget gebruiken

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Aangepaste Forms**.
1. Open de **Velden** om een rapport weer te geven met alle aangepaste velden en widgets in uw Workfront-exemplaar.

   ![](assets/fields-tab.png)

1. Klik op de knop **Weergave** vervolgkeuzemenu in de koptekst boven aan de lijst, en controleer vervolgens op aangepaste weergaven in de lijst die de **Rapporten** kolom (dit is geen standaardkolom op dit tabblad).

   In de kolom Rapporten kunt u zien welke rapporten elk aangepast veld en elke aangepaste widget gebruiken die aan een aangepast formulier in uw systeem is toegevoegd. Het is mogelijk dat iemand al een weergave heeft gemaakt die de **Rapporten** kolom.

1. Als er geen weergave wordt weergegeven die het **Rapporten** een nieuwe weergave maken die deze bevat:

   1. Klik op de knop **Weergave** vervolgkeuzemenu en vervolgens op **Nieuwe weergave**.

   1. Op de **Nieuwe weergave** pagina die in het vak bij de linkerbovenhoek wordt weergegeven, vervangen **Nieuwe parameterweergave** met een beschrijvende naam voor de weergave, zoals *Velden en widgets*.

   1. Klikken **Kolom toevoegen** in de rechterbenedenhoek.
   1. In de **Tonen in deze kolom** tekstvak dat in de linkerbovenhoek wordt weergegeven, beginnen met typen *verslag* selecteert u vervolgens **Rapporten** in de lijst onder het vak.

   1. (Voorwaardelijk) Als u het dialoogvenster **Rapporten** de kolom u enkel aan een verschillende horizontale positie toevoegde, sleept zijn kopbal in **Kolomvoorvertoning** onder aan de pagina.

   1. Klikken **Gereed** en klik vervolgens op **Weergave opslaan**.

1. Klik op de knop **Weergave** en selecteert u de naam van de aangepaste weergave die u zojuist hebt gemaakt.
1. In de **Naam** de kolom, vindt het douanegebied of widget u van plan bent uit te geven of te schrappen, dan bekijken **Rapporten** kolom op die rij om te zien welke rapporten het gebruiken, als om het even welk.

   Workfront zoekt naar de aangepaste velden en widgets in alle rapportfilters, weergaven en groepen om de informatie voor deze kolom te zoeken.

   Als u een plusteken ziet, kunt u op die tekstregel klikken om een vak weer te geven met alle extra rapporten die het veld of de widget gebruiken.

   >[!NOTE]
   >
   >De eerste laadtijd voor dit gereedschap kan van 10 seconden tot 2,5 minuten duren, afhankelijk van de hoeveelheid gegevens in uw systeem.

   >[!TIP]
   >
   >Als u geen tijd hebt om de rapporten te onderzoeken die het douanegebied of widget gebruiken, kunt u de Uitvoer klikken om een dossier tot stand te brengen dat hen een lijst maakt. U zou dit dossier met iedereen kunnen delen die een rapport bezit dat het gebied of widget gebruikt en de verandering bespreken die moet gebeuren, de invloed het op het rapport zou kunnen hebben, en wat moet worden gedaan om ervoor te zorgen dat het rapport correct blijft werken.
   >
   >Deze mening is ook beschikbaar in een rapport van de Parameter:
   >      
   > 1. Klik in het hoofdmenu op **Rapporten**.
   > 1. Klik in de linkerbovenhoek op **Nieuw rapport** en klik vervolgens op **Parameter** in de lijst die wordt weergegeven.
   > 1. Klikken **Kolom toevoegen** in de rechterbenedenhoek.
   > 1. In de **Tonen in deze kolom** tekstvak dat in de linkerbovenhoek wordt weergegeven, beginnen met typen *verslag* selecteert u vervolgens **Rapporten** in de lijst onder het vak.
   > 1. (Voorwaardelijk) Als u het dialoogvenster **Rapporten** de kolom u enkel aan een verschillende horizontale positie toevoegde, sleept zijn kopbal in **Kolomvoorvertoning** onder aan de pagina.
   > 1. Klikken **Gereed** en klik vervolgens op **Opslaan en sluiten**.
   > 1. Typ een beschrijvende naam voor het rapport, zoals *Velden en widgets*.

