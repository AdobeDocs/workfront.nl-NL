---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Gebruikersnaam al in gebruik
description: Lees deze tips als er een fout optreedt die de gebruikersnaam al gebruikt.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 722295463c1338a70ff42c26acf69b09cf33f725
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Gebruikersnaam is al in gebruik

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td><p>Systeembeheerder</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Vraag

Bij het maken van een nieuwe gebruiker wordt een [!UICONTROL Whoops] -fout weergegeven met de mededeling dat de gebruikersnaam al in gebruik is. Er zijn geen andere exemplaren van deze e-mail in het systeem. Waarom wordt dit weergegeven?

## Oplossing

Dit kan voorkomen omdat de gebruikersnaam of het e-mailadres niet uniek is in de huidige [!DNL Adobe Workfront] -instantie. Gebruikers kunnen in afzonderlijke gevallen dezelfde gebruikersnaam of hetzelfde e-mailadres hebben. Bijvoorbeeld, gebruiker A zou de volgende e-mailadressen kunnen hebben verbonden aan een [!DNL Workfront] rekening: usera@company1.com en usera@company2.com.

>[!NOTE]
>
>De primaire [!DNL Workfront] -beheerder kan niet dezelfde gebruikersnaam of hetzelfde e-mailadres hebben als deze zich in verschillende Workfront-instanties in dezelfde cluster bevindt.
>
>Als de instanties zich in verschillende clusters bevinden, kan de primaire beheerder dezelfde gebruikersnaam of hetzelfde e-mailadres hebben. U kunt de cluster waarop de instantie is ingeschakeld, weergeven onder [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Customer Info] .

### Controleren of uw gebruikersnaam uniek is in uw exemplaar

Zorg ervoor dat de gebruikersnaam en het e-mailadres uniek zijn in de huidige [!DNL Workfront] -instantie:

{{step-1-to-users}}

1. Kijk in de lijst met personen in de kolom **[!UICONTROL Email]** om ervoor te zorgen dat er geen dubbele e-mails voorkomen.
1. Voeg een kolom voor gebruikersnaam toe aan de weergave.

   1. Klik in de vervolgkeuzelijst **[!UICONTROL View]** op **[!UICONTROL Customize View]** .
   1. Klik op **[!UICONTROL Add Column]**.
   1. Typ *[!UICONTROL username]* in het zoekveld.
   1. Selecteer **[!UICONTROL User]** > **[!UICONTROL Username]** .
   1. Sla de weergave op.\
      Dit resulteert in een weergave om de gebruikersnamen weer te geven op de locatie waar u naar het duplicaat kunt zoeken.

1. Kijk in de lijst met personen in de kolom **[!UICONTROL Username]** om er zeker van te zijn dat er geen dubbele gebruikersnamen voorkomen.
