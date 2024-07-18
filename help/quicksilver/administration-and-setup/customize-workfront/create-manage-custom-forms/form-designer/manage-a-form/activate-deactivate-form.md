---
title: Een aangepast formulier deactiveren of opnieuw activeren
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: U kunt een aangepast formulier opnieuw activeren of deactiveren. We raden u aan aangepaste formulieren te deactiveren in plaats van formulieren te verwijderen die u niet meer gebruikt om historische gegevens te behouden.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Een aangepast formulier deactiveren of opnieuw activeren

U kunt een aangepast formulier opnieuw activeren of deactiveren. We raden u aan aangepaste formulieren te deactiveren in plaats van formulieren te verwijderen die u niet meer gebruikt om historische gegevens te behouden.

>[!NOTE]
>
>Als een douaneformulier wordt gedeactiveerd maar nog deel van een rijonderwerp of de definitie van de verzoekrij uitmaakt, zal het aan nieuwe verzoeken worden vastgemaakt. Als u niet wilt dat het formulier op de aanvragen staat, moet u het handmatig uit de aanvraagwachtrij verwijderen.

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Administratieve toegang tot aangepaste formulieren</p></td> 
  </tr>  
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Een aangepast formulier deactiveren

U kunt aangepaste formulieren die u niet meer gebruikt, deactiveren zonder de bijbehorende historische gegevens te verliezen. Gebruikers kunnen geen inactief aangepast formulier aan objecten toevoegen, maar ze kunnen wel gegevens weergeven en toevoegen aan de velden van objecten waaraan het al was gekoppeld.

Velden op een inactief aangepast formulier zijn ook nog steeds beschikbaar voor inlinebewerking in een weergave. Als een gebruiker tijdens een inlinebewerking een veld uit een inactief aangepast formulier toevoegt, wordt het formulier automatisch aan het object gekoppeld, ook al wordt het aangepaste formulier gedeactiveerd.

Een aangepast formulier deactiveren:

{{step-1-to-setup}}

1. In het linkerpaneel, kies **Aangepaste Forms**.
1. In het **Forms** gebied, selecteer de douanevorm u wilt deactiveren.
1. In is Actieve kolom, kies **Vals** en klik uit de kolom. Het formulier is niet meer actief.

## Een aangepast formulier opnieuw activeren

Als u een aangepast formulier opnieuw activeert, blijven de instellingen die het eerder had, behouden en kunnen gebruikers ermee werken alsof het nooit is gedeactiveerd.

{{step-1-to-setup}}

1. In het linkerpaneel, kies **Aangepaste Forms**.
1. In het **Forms** gebied, selecteer de douanevorm u wilt reactiveren.
1. In is Actieve kolom, kies **Waar** en klik uit de kolom. Het formulier is nu actief.
