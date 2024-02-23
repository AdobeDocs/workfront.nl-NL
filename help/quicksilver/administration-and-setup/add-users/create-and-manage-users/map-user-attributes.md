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
source-git-commit: 5b1efd8000417b9368fe3eb9037ac55464579bb4
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Gebruikerskenmerken toewijzen

<!--Audited 2/2024-->

Met SSO (Single Sign-On) kunt u kenmerken van de Active Directory van uw identiteitsprovider doorgeven aan uw Adobe Workfront-gebruikers.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td><p>Nieuw: Standaard</p><p>of</p><p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> </td> 
  </tr> 
 </tbody> 
</table>

Zie voor meer informatie over de informatie in deze tabel [Toegangsvereisten in Workfront-documentatie](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Tips voor het toewijzen van kenmerken

Houd rekening met het volgende wanneer u kenmerken toewijst:

* Test altijd in een voorvertoningssandbox of een CR-sandbox (Customer Refresh).
* Test met zowel beheerder als niet-beheerder rekeningen om te bevestigen dat u attributen correct in kaart brengt.
* Kenmerken die worden toegewezen, worden telkens toegepast wanneer een gebruiker zich via Single Sign On aanmeldt.

  Voorbeeld: als u &quot;achternaam&quot; toewijst en de naam in Workfront bijwerkt zonder de waarde in hun identiteitsprovider bij te werken, wordt de achternaam overschreven zodat deze overeenkomt met de waarde van wat zich in de identiteitsprovider bevindt de volgende keer dat de gebruiker zich aanmeldt.

## Gebruikerskenmerken toewijzen aan uw organisatie

De procedure voor het toewijzen van kenmerken hangt af van het feit of uw organisatie op de Adobe verenigde ervaring is.

Om te bepalen of uw organisatie op de Adobe verenigde ervaring is, onderzoek URL die u gebruikt om tot Workfront toegang te hebben.

| URL | Ervaring met Adobe |
|---|---|
| (Bedrijfsnaam).my.workfront.com | Klassieke ervaring |
| experience.adobe.com | Uniforme Adobe |

* [Gebruikerskenmerken toewijzen in de klassieke ervaring](#map-user-attributes-in-the-classic-experience)
* [Gebruikerskenmerken toewijzen in de verenigde Adobe](#map-user-attributes-in-the-adobe-unified-experience)

### Gebruikerskenmerken toewijzen in de klassieke ervaring

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Eenmalige aanmelding (SSO)**.

1. In de **Type** vervolgkeuzelijst, klikken **SAML 2.0**.

1. Klikken **Gebruikerskenmerken toewijzen**.

   ![](assets/map-user-attributes.png)

1. Wijs in de rij met opties die wordt weergegeven de kenmerken toe die u voor uw Workfront-gebruikers nodig hebt.

   U kunt kenmerken toewijzen, zoals Adres, Manager, Taakrol, Thuisgroep, enzovoort.

   Kenmerktoewijzingen werken met een verhouding van 1:1. U kunt bijvoorbeeld niet elke groep instellen waartoe een gebruiker behoort; u kunt slechts één groep per gebruiker instellen.

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

1. (Optioneel) Klik op **Regels** om een regel aan het attribuut toe te voegen.

   1. Kies in de vervolgkeuzelijst de kenmerkoptie die u wilt gebruiken.
   1. Typ in de twee velden rechts de waarde van het directorykenmerk en de waarde die u wilt vervangen.

      ![](assets/rule-fields.png)

   U kunt op **Regel toevoegen** om meer regels aan de attributen toe te voegen.

1. (Optioneel) Als u meer gebruikerskenmerken wilt toewijzen, klikt u op **Toewijzing toevoegen** en herhaal stap 6-7.
1. Klikken **Opslaan**.

### Gebruikerskenmerken toewijzen in de verenigde Adobe

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-left.png) in de linkerbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Eenmalige aanmelding (SSO)**.

1. Selecteer de **Adobe** tab.

1. (Optioneel en voorwaardelijk) Als uw organisatie kenmerktoewijzingen had geconfigureerd in de klassieke ervaring en u die kenmerktoewijzing wilt kopiëren naar de Adobe verenigde ervaring, klikt u op **Toewijzingen migreren**. U kunt deze toewijzingen vervolgens verwijderen, verwijderen of bewerken.

   >[!NOTE]
   >
   >Wij adviseren migrerende afbeeldingen de eerste keer u afbeeldingen in de Adobe verenigde ervaring vormt. Het heeft geen enkel nadeel om ze later opnieuw te migreren, maar het is niet nodig ze meer dan één keer te migreren.

1. Als u een nieuwe kenmerktoewijzing wilt maken, klikt u **Toewijzing toevoegen**.

1. Klik op de pijl naast de Workfront-veldnaam en selecteer de optie [!DNL Workfront] veld waarnaar u wilt toewijzen.

1. (Optioneel) Als u voor een bepaald veld meerdere regels wilt maken, klikt u op de pijl naast **Altijd** en selecteert u de operator die u voor de regel wilt gebruiken.

1. (Voorwaardelijk) Als u naast Altijd een operator hebt geselecteerd, selecteert u het veld Workfront en de waarde waarop de operator van toepassing is.

   >[!NOTE]
   >
   >De exploitanten `Is Truthy` en `Is Falsy` vereisen geen waarden.

1. Selecteer of u de waarde van een attribuut in uw identiteitsmanager op het gebied van Workfront wilt toepassen, of als u een specifieke constante waarde wilt toepassen.

1. Voer de naam in van het veld voor identiteitsbeheer dat u wilt toepassen of voer de tekst in van de constante waarde die u wilt toepassen.

1. (Optioneel) Als u meer regels voor hetzelfde Workfront-veld wilt toevoegen, klikt u op **Nieuwe regel toevoegen** en volg stap 4-9.

   >[!IMPORTANT]
   >
   > * Alle regels onder een regel Altijd wordt genegeerd. Als u een regel Altijd hebt, moet u deze naar de onderkant van de lijst met regels verplaatsen. U kunt regels in de lijst verplaatsen door op het menu met drie punten rechts van de regel te klikken en de regel omhoog of omlaag te verplaatsen.
   > * Als u een regel in het midden van de lijst wilt maken, klikt u op het menu met drie punten naast de regel die u boven of onder de nieuwe regel wilt plaatsen en selecteert u **Regel toevoegen boven** of **Regel toevoegen onder**.

1. Als u een regel wilt verwijderen, klikt u op het menu met drie punten naast de regel die u wilt verwijderen en selecteert u **Verwijderen**.
1. Als u een toewijzing wilt verwijderen, klikt u op de knop **Verwijderen** pictogram dat op de kaart voor die afbeelding staat.

1. Ga naar de bovenkant van de pagina en klik op Opslaan **Opslaan**.


