---
title: Een document delen
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder verleent gebruikers toegang tot weergave- of bewerkingsdocumenten wanneer zij toegangsniveaus toewijzen, zoals wordt uitgelegd in Toegang verlenen tot documenten.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 48c0f5c617f41a4ce51ea45c17817aa869ba5adb
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 0%

---

# Een document delen

De beheerder van Workfront controleert wie documenten in het gebied van Niveaus van de Toegang in Opstelling kunnen bekijken of uitgeven. Voor meer informatie, zie [&#x200B; toegang van de Verlening tot documenten &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Gebruikers kunnen ook documenten delen die ze hebben geüpload of waartoe ze toegang hebben, zodat anderen toestemming krijgen om ze te bekijken of te beheren.

* Machtigingen zijn van toepassing op afzonderlijke items en definiëren welke handelingen iemand kan uitvoeren.
* De persoon die een document uploadt krijgt automatisch volledige controle (beheermachtigingen).
* Om een volledige omslag te delen, zie [&#x200B; een documentomslag &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) delen.

>[!NOTE]
>
>Als uw Workfront-exemplaar gebruikmaakt van Adobe Enterprise Storage, kunt u geen afzonderlijke documenten delen. In plaats daarvan, hebt u grote toegang op het projectniveau. Houd in mening dat het delen van het project toegang tot gevoelige projectinformatie zoals financiële medewerkers kan verlenen afhankelijk van het gekozen niveau van toestemming.



## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

U moet het volgende hebben om objecten te delen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Nieuw: Standaard</p> 
   of
   <p>Huidig: Werk of hoger</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang tot of hoger weergeven voor de objecten die u wilt delen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen of hoger weergeven voor de objecten die u wilt delen</p></td> 
  </tr> 
 </tbody> 
</table>

Voor meer informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Een document delen

De gebruiker die een document naar Workfront uploadt, beschikt standaard over de machtiging Beheren.

{{step1-to-documents}}

1. Op de **pagina van Documenten**, houd over het document over u wilt delen en klik de **verbinding van de Details van het Document** die verschijnt. De **detailleert van het Document** pagina opent.

   ![&#x200B; verbinding van de Details van het Document &#x200B;](assets/document-details-link.png)

1. Klik het **Meer** pictogram ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png) aan het recht van de documentnaam, dan klik **Aandeel**. Het **de dialoogvakje van de Naam van het Document 1&rbrace; Aandeel [ opent.]**

   ![&#x200B; Deel een document &#x200B;](assets/share-a-document-350x160.png)

1. In het **document van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u het document met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt een document alleen delen met actieve gebruikers, teams, rollen of bedrijven.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van het document selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan het document worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen het document zonder een uitnodiging bekijken.

1. (Facultatief) om het document openbaar te maken, klik het tandwielpictogram ![&#x200B; selecteren het tandwielpictogram &#x200B;](assets/gear-icon.png), dan klik de doos in-lijn met **maak dit openbaar aan externe gebruikers**. De **openbare verbinding van het Exemplaar** knoop verschijnt bij de bodem van de dialoogdoos.

1. Klik op de vervolgkeuzelijst rechts van de gebruikersnaam en selecteer het machtigingsniveau voor dit document:

   * **Mening**: De gebruiker kan het document herzien en delen.
   * **leidt**: De gebruiker heeft volledige toegang tot het document zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor het document te configureren.

   ![&#x200B; gevormde geavanceerde toestemmingsopties &#x200B;](assets/advanced-options-icon.png)

1. (Facultatief) om geërfte toestemmingen voor de kindvoorwerpen van het document uit te zetten, klik **Draai** gealigneerd met **Geërfde toestemmingen**.

1. (Voorwaardelijk) om de openbare verbinding te kopiëren die u toestaat om het document met externe gebruikers te delen, klik **openbare verbinding van het Exemplaar**.

   >[!CAUTION]
   >
   >We raden u aan voorzichtig te zijn wanneer u een document met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

1. Klik **sparen**.

## Documenten bulksgewijs delen

{{step1-to-documents}}

1. In **Alle Documenten** lusje op de **pagina van Documenten**, onderdruk **Bevel** (Mac) of **CTRL** (Vensters) op uw toetsenbord, dan klik op elk document u wilt delen.

1. Bij de bovenkant van de pagina, klik het **pictogram van het Aandeel** van het Aandeel ![. &#x200B;](assets/share-icon.png) Het deelmodaal wordt geopend.

   ![&#x200B; pictogram van het Aandeel &#x200B;](assets/share-documents-in-bulk.png)

1. In het **document van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de documenten met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt documenten alleen delen met actieve gebruikers, teams, rollen of bedrijven.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van de documenten selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de documenten worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen de documenten zonder een uitnodiging bekijken.

1. Klik op de vervolgkeuzelijst rechts van de naam van de gebruiker en selecteer het desbetreffende machtigingsniveau voor de documenten:

   * **Mening**: De gebruiker kan de documenten herzien en delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de documenten zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor de documenten te configureren.

   ![&#x200B; gevormde geavanceerde toestemmingsopties &#x200B;](assets/advanced-options-icon.png)

1. Klik **sparen**.

## Document delen met Adobe Enterprise Storage

Workfront gaat over naar de Adobe Enterprise Storage-oplossing om Adobe Creative Cloud-producten beter te kunnen aansluiten. Bestaande klanten worden in fasen naar het nieuwe model verplaatst. Voor meer informatie over de voordelen van de ondernemingsopslag van Adobe, bezoek [&#x200B; overzicht van de ondernemingsopslag van Adobe &#x200B;](/help/quicksilver/review-and-approve-work/esm-overview.md).

Als uw Workfront-exemplaar gebruikmaakt van Adobe Enterprise Storage, kunt u afzonderlijke documenten niet rechtstreeks delen. In plaats daarvan, moet u toegang op het projectniveau verlenen.

>[!IMPORTANT]
>
>Het delen van een project kan gebruikers toegang tot gevoelige projectinformatie, zoals financiën, afhankelijk van het toestemmingsniveau ook verlenen u kiest.
>
>Controleer de machtigingsinstellingen zorgvuldig voordat u gaat delen.

## Documentmachtigingen

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren. Voor informatie over objecten toestemmingen, zie [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

In de volgende tabel wordt aangegeven welke machtigingen u gebruikers kunt verlenen wanneer zij documenten mogen weergeven of beheren:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Actie </strong> </p> </th> 
   <th> <p><strong> leiden </strong> </p> </th> 
   <th> <p><strong> Mening </strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Maken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Documentdetails bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verwijderen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Downloaden</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Afhandeling</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">fiatteurs toevoegen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Document goedkeuren</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aangepast formulier bijvoegen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aangepaste velden bewerken</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Naar (object)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Naar (integratie)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Updates/opmerkingen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Nieuwe versie uploaden</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Versie verwijderen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Document(en) weergeven</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Voorvertoning</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proef**</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Proef genereren**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Proef verwijderen**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Delen op systeemniveau*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Documenten openbaar delen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen met een extern e-mailadres</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Toevoegen/verwijderen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Naam wijzigen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Koppeling (met integratie)</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Ontkoppelen (met integratie)</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Actie wordt gedeeld door zowel Documenten als Documentmappen.

&#42;&#42; U moet een aparte proefdruklicentie aan uw Workfront-account hebben gekoppeld om documenten te kunnen controleren. Neem contact op met uw accountmanager voor het verkrijgen van een proefdruklicentie. Voor meer informatie over het proef in Workfront, zie [&#x200B; het Bewijzen &#x200B;](../../review-and-approve-work/proofing/proofing.md).

## Overwegingen bij het delen van documenten

Naast de overwegingen hieronder, zie ook [&#x200B; Overzicht van het delen van toestemmingen op voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

* Het delen van een document is vergelijkbaar met het delen van andere objecten in Workfront. Voor informatie over hoe te om documenten in Workfront te delen, zie [&#x200B; een voorwerp &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.
* U kunt documenten de volgende machtigingen geven:

   * Weergave
   * Beheren

* U kunt een document ook openbaar of systeembreed delen.

  >[!CAUTION]
  >
  >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

* U kunt een document delen met iemand die geen Workfront-account heeft, door het e-mailadres ervan toe te voegen in het veld Toegang tot document geven.
* Als u een document deelt, hebben gebruikers dezelfde toegang tot alle documentversies en alle documentproefdrukken.\
  Voor meer informatie over het proef in Workfront, zie [&#x200B; het Bewijzen &#x200B;](../../review-and-approve-work/proofing/proofing.md) sectie.

* U kunt machtigingen voor documenten overnemen van de objecten waaraan ze zijn gekoppeld. Uw Workfront-beheerder kan de overerving van machtigingen voor documenten op uw toegangsniveau beperken.

  Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [&#x200B; tot douanetoegangsniveaus &#x200B;](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

  U kunt overgeërfde machtigingen voor documenten handmatig verwijderen. Voor meer informatie, zie [&#x200B; toestemmingen uit voorwerpen &#x200B;](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md) verwijderen

* Een bijgevoegd document neemt alleen machtigingen over van het object waaraan het is gekoppeld. Als u een map voor het object maakt en het document naar de map verplaatst, neemt deze de machtigingen van de map over. Maar als u een map maakt op een bovenliggend of bovenliggend object en het document naar die map verplaatst, worden de machtigingen van die map niet overgenomen.