---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Gebruikersnaam al in gebruik
description: Lees deze tips als er een fout optreedt die de gebruikersnaam al gebruikt.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Gebruikersnaam al in gebruik

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licentie</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau</strong></td> 
   <td> <p>[!UICONTROL System administrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vraag

Wanneer u een nieuwe gebruiker maakt, kunt u [!UICONTROL Whoops] Er wordt een fout weergegeven met de mededeling dat de gebruikersnaam al in gebruik is. Er zijn geen andere exemplaren van deze e-mail in het systeem. Waarom wordt dit weergegeven?

## Oplossing

Dit kan zich voordoen omdat de gebruikersnaam of het e-mailadres niet uniek is in het huidige [!DNL Adobe Workfront] -instantie. Gebruikers kunnen in afzonderlijke gevallen dezelfde gebruikersnaam of hetzelfde e-mailadres hebben. Bijvoorbeeld, zou Gebruiker A de volgende e-mailadressen kunnen hebben verbonden aan a [!DNL Workfront] account: usera@company1.com en usera@company2.com.

>[!NOTE]
>
>De primaire [!DNL Workfront] beheerder kan niet dezelfde gebruikersnaam of hetzelfde e-mailadres hebben als deze zich in verschillende Workfront-instanties in dezelfde cluster bevinden.
>
>Als de instanties zich in verschillende clusters bevinden, kan de primaire beheerder dezelfde gebruikersnaam of hetzelfde e-mailadres hebben. U kunt de cluster bekijken waarop de instantie is ingeschakeld [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Customer Info].

### Controleren of uw gebruikersnaam uniek is in uw exemplaar

Zorg ervoor dat de gebruikersnaam en het e-mailadres uniek zijn in het huidige [!DNL Workfront] instantie:

1. Als de [!DNL Workfront] beheerder, klik **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Users]**.
1. Ga in de lijst met personen naar de knop **[!UICONTROL Email]** om ervoor te zorgen dat er geen dubbele e-mails zijn.
1. Voeg een kolom voor gebruikersnaam toe aan de weergave.

   1. In de **[!UICONTROL View]** vervolgkeuzelijst, klikt u op **[!UICONTROL Customize View]**.
   1. Klik op **[!UICONTROL Add Column]**.
   1. Typ in het zoekveld *[!UICONTROL username]*.
   1. Selecteren **[!UICONTROL User]** > **[!UICONTROL Username]**.
   1. Sla de weergave op.\
      Dit resulteert in een weergave om de gebruikersnamen weer te geven op de locatie waar u naar het duplicaat kunt zoeken.

1. Ga in de lijst met personen naar de knop **[!UICONTROL Username]** om ervoor te zorgen dat er geen dubbele gebruikersnamen zijn.
