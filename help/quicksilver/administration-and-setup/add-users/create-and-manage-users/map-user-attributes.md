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
source-git-commit: 9e7d20fe165e08997c14e207406fb8bed7597a56
workflow-type: tm+mt
source-wordcount: '956'
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

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tips voor het toewijzen van kenmerken

Houd rekening met het volgende wanneer u kenmerken toewijst:

* Test altijd in een voorvertoningssandbox of een CR-sandbox (Customer Refresh).
* Test met zowel beheerder als niet-beheerder rekeningen om te bevestigen dat u attributen correct in kaart brengt.
* Kenmerken die worden toegewezen, worden telkens toegepast wanneer een gebruiker zich via Single Sign On aanmeldt.

  Voorbeeld: als u &quot;achternaam&quot; toewijst en de naam in Workfront bijwerkt zonder de waarde in hun identiteitsprovider bij te werken, wordt de achternaam overschreven zodat deze overeenkomt met de waarde van wat zich in de identiteitsprovider bevindt de volgende keer dat de gebruiker zich aanmeldt.

## Gebruikerskenmerken toewijzen aan uw organisatie

De procedure voor het toewijzen van kenmerken hangt af van het feit of uw organisatie zich op de verenigde ervaring van Adobe bevindt.

Om te bepalen of uw organisatie zich op de verenigde ervaring van Adobe bevindt, onderzoek URL die u gebruikt om tot Workfront toegang te hebben.

| URL | Adobe-ervaring |
|---|---|
| (Bedrijfsnaam).my.workfront.com | Klassieke ervaring |
| experience.adobe.com | Adobe Unified Experience |

* [Gebruikerskenmerken toewijzen in de klassieke ervaring](#map-user-attributes-in-the-classic-experience)
* [Gebruikerskenmerken toewijzen in Adobe Unified Experience](#map-user-attributes-in-the-adobe-unified-experience)

### Gebruikerskenmerken toewijzen in de klassieke ervaring

1. Klik het **pictogram 1&rbrace; van het Belangrijkste Menu** Belangrijkste menupictogram ![&#x200B; in de hoger-juiste hoek van Adobe Workfront, dan klik &#x200B;](assets/main-menu-icon.png) de montages van de Opstelling **&#x200B;**&#x200B;Gear pictogram ![.](assets/gear-icon-settings.png)

1. Klik **Systeem** > **Enige Sign-On (SSO)**.

1. In het **Type** drop-down, klik **SAML 2.0**.

1. Klik **de Attributen van de Gebruiker van de Kaart**.

   ![&#x200B; de gebruikersattributen van de Kaart &#x200B;](assets/map-user-attributes.png)

1. Wijs in de rij met opties die wordt weergegeven de kenmerken toe die u voor uw Workfront-gebruikers nodig hebt.

   U kunt kenmerken toewijzen, zoals Adres, Manager, Taakrol, Thuisgroep, enzovoort.

   Kenmerktoewijzingen werken op een :1 verhouding. U kunt bijvoorbeeld niet elke groep instellen waartoe een gebruiker behoort; u kunt slechts één groep per gebruiker instellen.

   >[!IMPORTANT]
   >
   >We raden u niet aan om toegangsniveaus toe te wijzen in de toewijzingen van kenmerken. Als u dit doet, moet u voorzichtig zijn wanneer u de standaardwaarde instelt om ervoor te zorgen dat u Admin Access niet per ongeluk verwijdert.

   In de volgende tabel worden de velden uitgelegd die u kunt gebruiken om kenmerken toe te wijzen:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront-gebruikerskenmerk</td> 
      <td>Kies de naam van het kenmerk dat u wilt toewijzen</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Directory-kenmerk</td> 
      <td>Typ het kenmerk Sso dat u wilt gebruiken.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standaardwaarde</td> 
      <td> <p>Nadat u een Workfront-gebruikerskenmerk hebt gekozen en de waarde tijdens de verbinding NULL is, vult dit veld in met de bijbehorende standaardwaarde in het systeem. Typ hier alleen een waarde als u regels voor kenmerktoewijzing wilt toepassen (zie stap 7). De standaardwaarde fungeert als een uitzondering op deze regels.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Facultatief) klik **Regels** om een regel aan de attributen toe te voegen.

   1. Kies in de vervolgkeuzelijst de kenmerkoptie die u wilt gebruiken.
   1. Typ in de twee velden rechts de waarde van het directorykenmerk en de waarde die u wilt vervangen.

      ![&#x200B; de gebieden van de Regel &#x200B;](assets/rule-fields.png)

   U kunt **klikken voegt Regel** toe om meer regels aan de attributen toe te voegen.

1. (Facultatief) om meer gebruikersattributen in kaart te brengen, klik **Toewijzing** toevoegen en stappen 6-7 herhalen.
1. Klik **sparen**.

### Gebruikerskenmerken toewijzen in Adobe Unified Experience

1. Klik het **pictogram 1&rbrace; van het Belangrijkste Menu** Belangrijkste menupictogram ![&#x200B; in de upper-left hoek van Adobe Workfront, dan klik &#x200B;](assets/main-menu-left.png) de montages van de Opstelling **&#x200B;**&#x200B;Gear pictogram ![.](assets/gear-icon-settings.png)

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


