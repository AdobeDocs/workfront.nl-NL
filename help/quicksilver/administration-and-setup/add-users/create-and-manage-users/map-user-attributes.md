---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Kenmerken van gebruikers toewijzen en nieuwe gebruikers automatisch instellen
description: Met SSO (Single Sign-On) kunt u kenmerken van de Active Directory van uw identiteitsprovider doorgeven aan uw Adobe Workfront-gebruikers. U kunt ook nieuwe gebruikers aan Workfront toevoegen met de optie voor automatische voorzieningen (ook wel Just In Time Provisioning of JIT genoemd).
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Kenmerken van gebruikers toewijzen en nieuwe gebruikers automatisch instellen

Met SSO (Single Sign-On) kunt u kenmerken van de Active Directory van uw identiteitsprovider doorgeven aan uw Adobe Workfront-gebruikers. U kunt ook nieuwe gebruikers aan Workfront toevoegen met de optie voor automatische voorzieningen (ook wel Just In Time Provisioning of JIT genoemd).

>[!NOTE]
>
>Dit is niet beschikbaar als uw organisatie is aangemeld bij de Adobe Admin Console. Zie uw netwerk of beheerder van IT als u meer informatie nodig hebt.


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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tips voor het toewijzen van kenmerken

Houd rekening met het volgende wanneer u kenmerken toewijst:

* Test altijd in een voorvertoningssandbox of een CR-sandbox (Customer Refresh).
* Test met zowel beheerder als niet-beheerder rekeningen om te bevestigen dat u attributen correct in kaart brengt.
* Kenmerken worden toegewezen wanneer een gebruiker zich via SSO aanmeldt bij Workfront, en niet alleen tijdens de automatische provisioning.

## Kenmerken van gebruikers toewijzen en nieuwe gebruikers automatisch instellen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klikken **Systeem** > **Single Sign-On (SSO)**.

1. In de **Type** vervolgkeuzelijst, klikken **SAML 2.0**.

1. Klikken **Gebruikerskenmerken toewijzen**.

   ![](assets/map-user-attributes.png)

1. (Optioneel) Als u wilt dat Workfront automatisch nieuwe gebruikers maakt vanuit uw Active Directory, klikt u op **Gebruiker automatisch voorzien van voorzieningen**.

   Voor deze functie is kenmerktoewijzing vereist.

1. Wijs in de rij met opties die wordt weergegeven de kenmerken toe die u voor uw Workfront-gebruikers nodig hebt.

   U kunt kenmerken toewijzen, zoals Adres, Manager, Taakrol, Thuisgroep, enzovoort.

   Kenmerktoewijzingen werken met een verhouding 1:1. U kunt bijvoorbeeld niet elke groep instellen waartoe een gebruiker behoort; u kunt slechts één per gebruiker instellen.

   >[!IMPORTANT]
   >
   >De volgende kenmerken zijn vereist voor elke gebruiker:
   >      
   >* Voornaam
   >* Achternaam
   >* E-mailadres

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
      <td>Typ het kenmerk Sso dat u wilt gebruiken./td&gt; 
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

1. (Optioneel) Klik op **Toewijzing toevoegen** en herhaal stap 6-7.
1. Klikken **Opslaan**.
