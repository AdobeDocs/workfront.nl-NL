---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Gebruikerskenmerken toewijzen
description: Met SSO (Single Sign-On) kunt u kenmerken van de Active Directory van uw identiteitsprovider doorgeven aan uw Adobe Workfront-gebruikers.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: d8ccdeac9a658ca7a2862781e98c2c3c6fa0e8a0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Gebruikerskenmerken toewijzen

<!--Audited 2/2024-->

Met SSO (Single Sign-On) kunt u kenmerken van de Active Directory van uw identiteitsprovider doorgeven aan uw Adobe Workfront-gebruikers.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Standard</p><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td><p>U moet een Workfront-beheerder zijn</p></td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tips voor het toewijzen van kenmerken

Houd rekening met het volgende wanneer u kenmerken toewijst:

* Test altijd in een voorvertoningssandbox of een CR-sandbox (Customer Refresh).
* Test met zowel beheerder als niet-beheerder rekeningen om te bevestigen dat u attributen correct in kaart brengt.
* Kenmerken die worden toegewezen, worden telkens toegepast wanneer een gebruiker zich via Single Sign On aanmeldt.

  Voorbeeld: als u &quot;achternaam&quot; toewijst en de naam in Workfront bijwerkt zonder de waarde in hun identiteitsprovider bij te werken, wordt de achternaam overschreven zodat deze overeenkomt met de waarde van wat zich in de identiteitsprovider bevindt de volgende keer dat de gebruiker zich aanmeldt.

## Gebruikerskenmerken toewijzen aan uw organisatie

1. Klik het **pictogram 1} van het Belangrijkste Menu** Belangrijkste menupictogram ![ in de upper-left hoek van Adobe Workfront, dan klik ](assets/main-menu-left.png) de montages van de Opstelling **** Gear pictogram ![.](assets/gear-icon-settings.png)

1. Klik **Systeem** > **Enige Sign-On (SSO)**.

1. Selecteer het **Adobe** lusje.

1. (Facultatief en voorwaardelijk) als uw organisatie kenmerkafbeelding had die in de klassieke ervaring wordt gevormd en u die attributenafbeelding aan de verenigde ervaring van Adobe wilt kopiëren, klik **Migrate Toewijzingen**. U kunt deze toewijzingen vervolgens verwijderen, verwijderen of bewerken.

   >[!NOTE]
   >
   >We raden u aan toewijzingen te migreren wanneer u toewijzingen voor het eerst configureert in de verenigde Adobe-ervaring. Het heeft geen enkel nadeel om ze later opnieuw te migreren, maar het is niet nodig ze meer dan één keer te migreren.

1. Om een nieuwe attributenafbeelding tot stand te brengen, klik **Toewijzing** toevoegen.

1. Klik op de pijl naast de Workfront-veldnaam en selecteer het [!DNL Workfront] -veld waarnaar u wilt toewijzen.

1. (Facultatief) als u meer dan één regel voor een bepaald gebied wilt tot stand brengen, klik de pijl naast **altijd** en selecteer de exploitant die u de regel wilt gebruiken.

1. (Voorwaardelijk) Als u naast Altijd een operator hebt geselecteerd, selecteert u het veld Workfront en de waarde waarop de operator van toepassing is.

   >[!NOTE]
   >
   >De operatoren `Is Truthy` en `Is Falsy` vereisen geen waarden.

1. Selecteer of u de waarde van een attribuut in uw identiteitsmanager op het gebied van Workfront wilt toepassen, of als u een specifieke constante waarde wilt toepassen.

1. Voer de naam in van het veld voor identiteitsbeheer dat u wilt toepassen of voer de tekst in van de constante waarde die u wilt toepassen.

1. (Facultatief) om meer regels voor het zelfde gebied van Workfront toe te voegen, klik **voeg Nieuwe Regel** toe, en volg stappen 4-9.

   >[!IMPORTANT]
   >
   > * Alle regels onder een regel Altijd wordt genegeerd. Als u een regel Altijd hebt, moet u deze naar de onderkant van de lijst met regels verplaatsen. U kunt regels in de lijst verplaatsen door op het menu met drie punten rechts van de regel te klikken en de regel omhoog of omlaag te verplaatsen.
   > * Om een regel in het midden van de lijst tot stand te brengen, klik het drie-punt menu naast de regel die u boven of onder de nieuwe regel wilt zijn, en selecteer **toevoegen Lijn boven** of **voeg Lijn onder** toe.

1. Om een regel te schrappen, het drie-punt menu naast de regel te klikken wilt u schrappen, en **Schrapping** selecteren.
1. Om een afbeelding te schrappen, klik het **Schrapping** pictogram dat op de kaart voor die afbeelding is.

1. Om te bewaren, scrol aan de bovenkant van de pagina en klik **sparen**.


