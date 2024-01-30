---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Een scorecard maken
description: Een scorecard meet hoe goed een project zich aan de eerder vastgestelde criteria van een portefeuille richt. Een scorecard weerspiegelt vaak de missie, de waarden, en de strategische doelstellingen van een organisatie.De managers van het Portfolio bepalen gewoonlijk de scorecardvragen en de antwoorden om ervoor te zorgen zij zinvol en waardevol tijdens projectprioriteit en selectie zijn. An [!DNL Adobe Workfront] de beheerder bouwt de scorecards die op de aanbevelingen van portefeuillemanagers worden gebaseerd.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Een scorecard maken

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Een scorecard meet hoe goed een project zich aan de eerder vastgestelde criteria van een portefeuille richt. Een scorecard weerspiegelt vaak de missie, de waarden, en de strategische doelstellingen van een organisatie.

De managers van het Portfolio bepalen gewoonlijk de scorecard vragen en de antwoorden om ervoor te zorgen zij tijdens project voorrang geven en selectie zinvol en waardevol zijn. An [!DNL Adobe Workfront] de beheerder bouwt de scorecards die op de aanbevelingen van portefeuillemanagers worden gebaseerd.

De vragen en antwoorden die voor een scorecard worden gekozen moeten kwantificeerbaar zijn om een groeperingswaarde te verstrekken om verschillende projecten te vergelijken.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Huidige: [!UICONTROL Business] of hoger</p> 
   of
   <p>Nieuw: [!UICONTROL Prime] of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td> 
   <td><p>Huidige: [!UICONTROL Plan]</p>
   of
   <p>Nieuw: [!UICONTROL Standard]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Een scorecard maken

{{step-1-to-setup}}

1. Klikken **[!UICONTROL Scorecards]** en klik vervolgens op **[!UICONTROL New Scorecard]** om de scorecard bouwer te lanceren en een scorecard te creëren.

1. Geef een **[!UICONTROL Scorecard Name]** en **[!UICONTROL Description]**.

   De naamvertoningen wanneer u scorecard met het project associeert. De beschrijving toont naast de scorecardnaam in de scorecardlijst.

1. Klik op de knop **[!UICONTROL Add Question]** vervolgkeuzelijst om het dialoogvenster [!UICONTROL scorecard question] en geeft u vervolgens de volgende informatie op voor uw vraag:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Question]</td> 
      <td>Typ de vraag die u in de scorecard wilt opnemen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Points]</td> 
      <td>Typ het maximum aantal punten dat mogelijk is voor deze vraag.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Negative Points]</td> 
      <td>Selecteer deze optie om aan te geven dat [!DNL Workfront] moeten worden afgetrokken van het totaal van de mogelijke punten. Negatieve scores kunnen niet aan de maximum mogelijke punten van een scorecard worden toegevoegd.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Display Type]</td> 
      <td>Selecteren <strong>[!UICONTROL Value(0-100)]</strong> als u een numeriek veld wilt weergeven in de scorecard waar gebruikers een waarde tussen 0 en 100 kunnen opgeven.<p>Of selecteer <strong>[!UICONTROL Drop Down]</strong> of <strong>[!UICONTROL Radio Buttons]</strong> om een antwoord tot stand te brengen kunnen de gebruikers specificeren gebruikend dat besturingselement. Klikken <strong>[!UICONTROL Add Answer]</strong>Typ vervolgens de tekst <strong>[!UICONTROL Value]</strong> in procentpunten voor dit antwoord, indien het antwoord is uitgevoerd. Als u 100% kiest, wordt het aantal punten dat voor deze vraag is toegewezen, volledig bereikt. Als u wilt aangeven dat dit antwoord slechts een gedeelte van het totale aantal punten bevat dat aan deze vraag is toegewezen, selecteert u een lager percentage. Als uw vraag bijvoorbeeld op 10 punten wordt gewaardeerd en u wilt dat dit antwoord 5 van deze punten bevat, kiest u 50% voor uw waarde.</p>
      <p>Selecteren <strong>[!UICONTROL Default]</strong> als u moet aangeven dat dit het standaardantwoord is.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Klikken **[!UICONTROL Add Question]** om meer vragen en antwoorden aan uw scorecard toe te voegen, die de zelfde stappen volgen.

   >[!NOTE]
   >
   >U kunt de vragen in uw scorecard opnieuw ordenen door de vragen in de juiste volgorde te slepen en neer te zetten.

1. Klikken **[!UICONTROL Save]** wanneer u klaar bent met het invoeren van alle gegevens.

   Dit leidt tot scorecard en de projectmanagers kunnen het aan hun projectbedrijfscase nu vastmaken.

## Pas een scorecard op een project toe

Een gebruiker met [!UICONTROL manage] de toestemmingen aan een project kunnen een scorecard op een project toepassen, nadat scorecard door is gecreeerd [!DNL Workfront] beheerder.

Een scorecard wordt toegevoegd aan een project als deel van het creëren van een bedrijfsgeval voor het project. Voor meer informatie over het toevoegen van een scorecard aan een project, zie [Pas een scorecard op een project toe en produceer een Score van de Uitlijning](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Zie voor meer informatie over projectmachtigingen [Een project delen in [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
