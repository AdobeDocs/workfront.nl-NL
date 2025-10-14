---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: De knop Aan de werkbalk vervangen door een knop Start
description: De standaardconfiguratie van Adobe Workfront omvat het Werk aan het knoop voor taken en kwesties die voor punten tonen die u aan bent toegewezen.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '701'
ht-degree: 0%

---

# De knop [!UICONTROL Work On It] vervangen door een knop [!UICONTROL Start]

De standaardconfiguratie van [!DNL Adobe Workfront] bevat een [!UICONTROL Work On It] -knop voor taken en problemen die worden weergegeven voor items waaraan u bent toegewezen. Wanneer u op [!UICONTROL Work On It] klikt voor items die aan u zijn toegewezen, geeft u aan andere gebruikers door dat u het werk hebt ontvangen en bevestigt u dat u eraan zult werken. De knop [!DNL Work On It] werkt de taak of de uitgiftestatus echter niet bij om aan te geven dat het werk daadwerkelijk is gestart.

U kunt de knop [!DNL Work On It] vervangen door een [!UICONTROL Start] -knop voor een team waartoe u behoort. In dit geval klikt u op de knop [!UICONTROL Start] in plaats van op [!UICONTROL Work On It] , die automatisch de status en de [!UICONTROL Actual Start Date] van het werkitem bijwerkt en aangeeft dat u met werken bent begonnen. Voor informatie over het plaatsen waarvan team uw veranderingen in de [!UICONTROL Work On It] knoop zou kunnen beïnvloeden, zie de sectie [&#x200B; de [!UICONTROL Start] knoop &#x200B;](#configure-the-uicontrol-start-button) in dit artikel vormen.

>[!IMPORTANT]
>
>Wanneer u op de knop [!UICONTROL Start] klikt, veranderen de status van het item en [!UICONTROL Actual Start Date] . Als iemand anders aan een taak of kwestie (die de status in [!UICONTROL In Progress] en bevolkt [!UICONTROL Actual Start Date]) is begonnen te werken, de knoop voor het punt toont als [!UICONTROL Work On It] zelfs wanneer een team u tot hebt behoort de knoop vervangen met een [!UICONTROL Start] knoop heeft.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-plan</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## De knop [!UICONTROL Start] configureren

Als u een [!UICONTROL Plan] -licentie hebt, kunt u de [!UICONTROL Start] -knop voor een team configureren in het [!UICONTROL Edit] -teamvenster. Hieronder wordt beschreven hoe de knop werkt nadat deze is ingeschakeld voor een team:

* **het team wordt toegewezen aan een het werkpunt**: Als een team aan het het werkpunt wordt toegewezen, zien de leden op dat team de [!UICONTROL Start] knoop en de statussen die voor dat team worden gevormd.
* **de gebruiker behoort tot een Team van het Huis**: Als geen team aan het het werkpunt wordt toegewezen maar de gebruiker wordt toegewezen aan een Team van het Huis in hun profiel, dan ziet de gebruiker de [!UICONTROL Start] knoop en de statussen die voor dat team worden gevormd. Dit is het scenario dat we aanbevelen als u wilt dat gebruikers de knop [!UICONTROL Start] vaak gebruiken.
* **de gebruiker wordt toegewezen aan een het werkpunt**: Als er geen team is dat aan het het werkpunt wordt toegewezen en geen Team van het Huis dat aan de gebruiker wordt toegewezen maar de gebruiker wordt toegewezen aan het het werkpunt, dan ziet de gebruiker de [!UICONTROL Start] knoop en de gecombineerde die statussen voor dat alle teams worden gevormd zij worden toegewezen aan.
* **de gebruiker wordt niet toegewezen aan om het even welke teams:** als er geen team aan het het werkpunt en geen team voor de gebruiker, met inbegrip van het Team van het Huis wordt toegewezen, en het punt wordt toegewezen aan de gebruiker, dan lijkt de gebruiker de [!UICONTROL Work On It] knoop.

>[!NOTE]
>
>Deze functie is momenteel niet beschikbaar in
>
>* De mobiele app [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] e-mailmeldingen
>

De knop Start configureren:

{{step1-to-team}}

1. Selecteer een team in de vervolgkeuzelijst **[!UICONTROL Teams]** .\
   of\
   Klik op **[!UICONTROL Create new team]**.

1. Klik op het pictogram **[!UICONTROL More]** ![](assets/more-icon.png) en klik vervolgens op **[!UICONTROL Edit]** .

1. Zoek de knopsectie **[!UICONTROL Work On It]** onder aan de pagina van [!UICONTROL Edit Teams] .
1. Schakel het selectievakje **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]** in.
1. Selecteer een of meer statussen voor elk type werkitem. Als u meerdere statussen selecteert, wordt een vervolgkeuzemenu weergegeven wanneer u op [!UICONTROL Start] klikt waar u de gewenste status kunt kiezen.
1. Klik op **[!UICONTROL Save changes]**. Gebruikers zien nu een knop [!UICONTROL Start Task] of [!UICONTROL Start Issue] in plaats van de knop [!UICONTROL Work On It] wanneer hun een tijdelijk item wordt toegewezen.

   >[!NOTE]
   >
   >Wij adviseren plaatsend het team als Team van het Huis van de gebruiker zodat verschijnt de beginknoop op elk van hun toegewezen het werkpunten. Zie [&#x200B; gebruikers met een Team van het Huis &#x200B;](#associate-users-with-a-home-team) hieronder associëren.

## Gebruikers koppelen aan een Home Team

Om gebruikers met een Team van het Huis te associëren:

{{step-1-to-users}}

1. Selecteer de gebruiker of de gebruikers u met een Team van het Huis wilt associëren.
1. Klik op het menu **[!UICONTROL More]** en selecteer vervolgens **[!UICONTROL Edit]** .\
   ![](assets/user-settings-nwe-350x291.png)

1. Selecteer in de sectie **[!UICONTROL Organization]** het veld **[!UICONTROL Home Team]** . Begin de naam van het team te typen waarvan montages u met de gebruikers wilt associëren. Klik op de naam van het team wanneer deze wordt weergegeven in de lijst.

1. Klik op **[!UICONTROL Save Changes]**.\
   De gebruikers u selecteerde worden nu geassocieerd met een Team van het Huis.

   Alle teaminstellingen, inclusief de statussen die zijn gekoppeld aan de knop [!UICONTROL Done] , zijn nu zichtbaar voor deze gebruikers.

