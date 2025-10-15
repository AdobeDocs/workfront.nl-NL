---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: single-sign-on-in-workfront
title: Gebruikers bijwerken voor eenmalige aanmelding
description: U kunt gebruikers bijwerken voor eenmalige aanmelding in Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0f9c543a-2ae2-4c2c-9c4d-647079263a7e
source-git-commit: 75fea812b4574191522af4721a013b57aa5d609f
workflow-type: tm+mt
source-wordcount: '793'
ht-degree: 0%

---

# Gebruikers bijwerken voor eenmalige aanmelding

<!-- Audited: 1/2024 -->

{{important-admin-console-onboard}}

Wanneer SSO (Single Sign-On) is ingeschakeld in uw Adobe Workfront-instantie, kunnen uw gebruikers zich aanmelden bij Workfront met hun SSO-referenties.

Als u een bestaand systeem hebt dat al is gevuld met gebruikers die zijn gekoppeld aan SSO-referenties, kunt u de gebruikers-id&#39;s importeren in Workfront door een CSV-bestand (comma-separated values, door komma&#39;s gescheiden waarden) te importeren in Workfront.

Voor meer informatie over het integreren van Workfront met een SSO systeem, zie [&#x200B; Overzicht van enige sign-on in Adobe Workfront &#x200B;](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).


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
   <td> <p>U moet een Workfront-beheerder zijn.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SSO-gebruikersnamen

Afhankelijk van welke oplossing SSO u gebruikt, kan de gebruikersbenaming in uw milieu SSO om het even welke volgend worden genoemd:

* SSO-gebruikersnaam
* Federatie-id
* Federation-gebruikersnaam

Ongeacht wat de gebruikersbenaming in uw milieu SSO wordt geroepen, wordt de waarde van het gebied opgeslagen op het gebied van de Gebruikersnaam SSO, op het voorwerp van de Gebruiker.

Uw gebruikers kunnen zich alleen aanmelden bij Workfront als hun SSO-gebruikersgegevens zijn bijgewerkt met hun profiel en hun SSO-gebruikersnaam en Workfront-gebruikersnaam worden opgenomen.

Als Workfront-beheerder kunt u het veld SSO-gebruikersnaam voor uw Workfront-gebruikers bulksgewijs bijwerken door een lijst met gebruikersnamen te importeren in Workfront. Deze lijst moet:

* Bevat de Workfront-gebruikersnaam (GUID) en de bijbehorende SSO-gebruikersnaam voor elke gebruiker
* Opslaan als CSV- of TSV-bestand.

Dit proces werkt bestaande SSO-gebruikersnamen in Workfront bij of voegt een nieuwe SSO-gebruikersnaam toe als deze ontbreekt voor gebruikers.

## Het importbestand voorbereiden {#prepare-the-import-file}

U kunt uw importbestand voorbereiden door een rapport van alle gebruikers in Workfront op te stellen waarin de velden voor SSO-gebruikersnaam moeten worden bijgewerkt.

1. Bouw een gebruikersrapport in Workfront.

   Voor instructies bij de bouw van gebruikersrapporten in Workfront, zie [&#x200B; een douanerapport &#x200B;](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Selecteer de volgende gebieden in uw rapport:

   | Veld | Toelichting |
   |---|---|
   | Naam | De volledige naam van de Workfront-gebruiker. |
   | ID | De id is de alfanumerieke GUID van Workfront. |
   | SSO-gebruikersnaam | Door het veld SSO-gebruikersnaam toe te voegen, weet u zeker dat u geen gebruikersnamen overschrijft met het importeren. Dit veld moet leeg zijn voor alle gebruikers als uw gebruikers nog niet zijn bijgewerkt voor SSO. |

   ![&#x200B; Gebruikers met gebruikersbenaming SSO maar geen toegang &#x200B;](assets/users-with-sso-username-and-no-sso-access-only-field.png)

1. Sla het rapport op.
1. Klik **Uitvoer** bij de bovenkant van het rapport en voer het rapport naar Excel uit.
1. Open het geëxporteerde Excel-bestand en voeg uw SSO-gebruikersnamen voor elke gebruiker toe in het rapport in de kolom Gebruikersnaam van SSO.

   >[!IMPORTANT]
   >
   >SSO-gebruikersnamen zijn hoofdlettergevoelig.

1. Schrap alle kolommen in het dossier van Excel, behalve **identiteitskaart** en de **Sso- Gebruikersnaam** kolommen.

1. Schrap de kolomkopballen en zorg ervoor er geen lege rijen bij de bovenkant van het rapport zijn.

   Het dossier u voor het bijwerken van uw gebruikers van Workfront met de gebruikersnamen SSO **gebruikt moet** enkel 2 kolommen, in deze orde bevatten:

   * In de eerste kolom moet de Workfront-gebruikersnaam worden weergegeven (de gebruiker GUID in Workfront).
   * De tweede kolom moet de Sso- Gebruikersnaam bevatten, aangezien het in uw SSO systeem toont.
   * De kolommen mogen geen kopteksten hebben en er mogen geen lege rijen boven aan de lijst met namen staan.

     ![&#x200B; de gebruikers CSV van de Update &#x200B;](assets/update-users-for-sso-csv-file-for-import.png)

1. Sla het rapport op als een CSV- of TSV-bestand op uw computer.

## Uw gebruikers bijwerken voor SSO {#update-your-users-for-sso}

Het proces om gebruikers voor SSO bij te werken of voegt het gebied van de Gebruikersnaam SSO aan uw gebruikers van Workfront toe als men niet aanwezig is, of werkt de waarde op dat gebied bij als er een waarde reeds verbonden aan de gebruikers is.

{{step-1-to-setup}}

1. Klik **Systeem**, dan uitgezochte **Gebruikers van de Update voor SSO**.

1. Klik **kiezen Dossier** om voor het dossier te doorbladeren u voorbereidde.

   Voor meer informatie over hoe te om dit dossier voor te bereiden, zie [&#x200B; het de invoerdossier &#x200B;](#prepare-the-import-file) voorbereiden.

1. Selecteer het dossier van waar het op uw computer wordt bewaard, dan klik **Open**.

   Hiermee worden de SSO-gegevens ingevoegd in Workfront, zodat alle gebruikers zich met hun SSO-gegevens kunnen aanmelden bij Workfront.

   **slechts staat `<SSO Configuration>` Authentificatie** het plaatsen toe wordt toegelaten voor alle gebruikers inbegrepen in CSV. Dit zorgt ervoor dat de gebruikers zich door SSO moeten aanmelden.

## Verifieer SSO tegen de gebruikersnamen van Workfront van uw gebruikers

Voor instructies bij de bouw van een gebruikersrapport dat Sso- Gebruikersnaam informatie bevat, zie [&#x200B; het de invoerdossier &#x200B;](#prepare-the-import-file) voorbereiden.

1. Voer een gebruikersrapport met SSO-gebruikersnaam in.

   Bericht dat de kolom van de Gebruikersnaam SSO voor elke gebruiker wordt bevolkt.

1. Zorg ervoor dat de waarden voor de kolom Gebruikersnaam SSO overeenkomen met de gebruikersnaam van SSO op uw SSO-server.
1. Als de kolom Gebruikersnaam SSO leeg is, werkt u de SSO-gebruikersnamen van uw gebruikers bij.

   ![&#x200B; Gebruikers met gebied SSO &#x200B;](assets/users-with-sso-field-updated.png)

   Voor instructies bij het bijwerken van uw gebruikers voor SSO, zie [&#x200B; Update uw gebruikers voor SSO &#x200B;](#update-your-users-for-sso).
