---
title: Deel een document
content-type: reference
product-area: user-management
navigation-topic: grant-and-request-access-to-objects
description: Uw Adobe Workfront-beheerder geeft gebruikers toegang om documenten te bekijken of te bewerken wanneer zij toegangsniveaus toewijzen, zoals uitgelegd in Verleen toegang tot documenten.
author: Courtney
feature: Get Started with Workfront
exl-id: c83a3184-4af0-4897-985b-29f7ee3a0b73
source-git-commit: 7f8c9b9f63770d6364f0eb1b9c23e4648dacaf93
workflow-type: tm+mt
source-wordcount: '1387'
ht-degree: 0%

---

# Deel een document

De Workfront-beheerder bepaalt wie documenten kan bekijken of bewerken in het Toegangsniveau-gedeelte in Setup. Voor meer informatie, zie [Toegang verlenen tot documenten](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md).

Gebruikers kunnen ook documenten delen die ze hebben geüpload of waartoe ze toegang hebben, zodat anderen toestemming krijgen om ze te bekijken of te beheren.

* Machtigingen zijn van toepassing op afzonderlijke items en definiëren welke handelingen iemand kan uitvoeren.
* De persoon die een document uploadt krijgt automatisch volledige controle (beheermachtigingen).
* Om een volledige omslag te delen, zie [ een documentomslag ](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md) delen.

>[!NOTE]
>
>Als uw Workfront-exemplaar gebruikmaakt van Adobe Enterprise Storage, kunt u geen afzonderlijke documenten delen. In plaats daarvan, verleent u toegang op het projectniveau. Houd in mening dat het delen van het project toegang tot gevoelige projectinformatie zoals financiële medewerkers afhankelijk van het gekozen niveau van toestemming kan verlenen.



## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-pakket</td> 
   <td> <p>Elk </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td> <p>Standard</p> 
   <p>Werk of hoger</p>
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

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++



## Een document delen

De gebruiker die een document uploadt naar Workfront heeft standaard Beheren-rechten voor het document.

{{step1-to-documents}}

1. Op de **pagina Documenten** beweeg je de muis over het document dat je wilt delen en klik je op de **Link Documentdetails** die verschijnt. De **pagina met documentdetails** opent.

   ![Link naar documentdetails](assets/document-details-link.png)

1. Klik het **Meer** pictogram ![ Meer pictogram ](assets/more-icon.png) aan het recht van de documentnaam, dan klik **Aandeel**. Het **de dialoogvakje van de Naam van het Document 1} Aandeel [ opent.]**

   ![ Deel een document ](assets/share-a-document-350x160.png)

1. In het **document van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u het document met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt een document alleen delen met actieve gebruikers, teams, rollen of bedrijven.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van het document selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan het document worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **iedereen in het systeem kan** bekijken: Alle gebruikers in het systeem kunnen het document zonder een uitnodiging bekijken.

1. (Facultatief) om het document openbaar te maken, klik het tandwielpictogram ![ selecteren het tandwielpictogram ](assets/gear-icon.png), dan klik de doos in-lijn met **maak dit openbaar aan externe gebruikers**. De **openbare verbinding van het Exemplaar** knoop verschijnt bij de bodem van de dialoogdoos.

1. Klik op de vervolgkeuzelijst rechts van de gebruikersnaam en selecteer het machtigingsniveau voor dit document:

   * **Mening**: De gebruiker kan het document herzien en delen.
   * **Beheren**: De gebruiker heeft volledige toegang tot het document zonder beheerdersrechten, die op toegangsniveau worden verleend (inclusief alle weergave-rechten).

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor het document te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-options-icon.png)

1. (Facultatief) om geërfte toestemmingen voor de kindvoorwerpen van het document uit te zetten, klik **Draai** gealigneerd met **Geërfde toestemmingen**.

1. (Voorwaardelijk) om de openbare verbinding te kopiëren die u toestaat om het document met externe gebruikers te delen, klik **openbare verbinding van het Exemplaar**.

   >[!CAUTION]
   >
   >Wij raden aan voorzichtig te zijn bij het delen van een document met vertrouwelijke informatie met externe gebruikers. Op deze manier kunnen ze informatie weergeven zonder dat ze een Workfront-gebruiker of onderdeel van uw organisatie zijn.

1. Klik op **Opslaan**.

## Deel documenten in bulk

{{step1-to-documents}}

1. Op het **tabblad Alle Documenten** op de **pagina Documenten** houd **je Command** (Mac) of **Ctrl** (Windows) ingedrukt op je toetsenbord en klik je vervolgens op elk document dat je wilt delen.

1. Klik bovenaan de pagina op het **deel-icoon** ![Delen-icoon](assets/share-icon.png). De deelmodaliteit opent.

   ![ pictogram van het Aandeel ](assets/share-documents-in-bulk.png)

1. In het **document van de Verlening toegang tot** gebied, begin typend de naam van de gebruiker, het team, de rol, de groep, of het bedrijf u de documenten met wilt delen, dan klik de naam wanneer het in de drop-down lijst verschijnt.

   >[!TIP]
   >
   >U kunt documenten alleen delen met actieve gebruikers, teams, rollen of bedrijven.


1. (Facultatief) selecteer **wie toegang** drop-down heeft en het de toegangsniveau van de documenten selecteert:

   * **slechts kunnen de uitgenodigde mensen toegang hebben:** slechts de gebruikers die aan de documenten worden uitgenodigd kunnen tot het (Gebrek) toegang hebben.
   * **Iedereen in het systeem kan bekijken**: Alle gebruikers in het systeem kunnen de documenten zonder uitnodiging bekijken.

1. Klik op het keuzemenu rechts van de naam van de gebruiker en selecteer hun toestemmingsniveau voor de documenten:

   * **Bekijk** de documenten: De gebruiker kan de documenten bekijken en delen.
   * **leidt**: De gebruiker heeft volledige toegang tot de documenten zonder administratieve rechten, die op het toegangsniveau (omvat ook alle toestemmingen van de Mening) worden verleend.

1. (Optioneel) Klik op het pictogram Geavanceerde opties naast het machtigingsniveau dat u hebt toegekend om specifieke machtigingen voor de documenten te configureren.

   ![ gevormde geavanceerde toestemmingsopties ](assets/advanced-options-icon.png)

1. Klik **sparen**.

## Documentdeling met Adobe enterprise storage

Workfront maakt de overstap naar de Adobe enterprise storage-oplossing om betere connectiviteit te bieden met Adobe Creative Cloud-producten. Bestaande klanten zullen in fasen worden overgestapt naar het nieuwe model. Voor meer informatie over de voordelen van Adobe enterprise storage, bezoek [Adobe enterprise storage overzicht](/help/quicksilver/review-and-approve-work/esm-overview.md).

Als je Workfront-instantie Adobe enterprise storage gebruikt, kun je individuele documenten niet direct delen. In plaats daarvan moet je toegang verlenen op projectniveau.

>[!IMPORTANT]
>
>Het delen van een project kan gebruikers toegang tot gevoelige projectinformatie, zoals financiën, afhankelijk van het toestemmingsniveau ook verlenen u kiest.
>
>Controleer de machtigingsinstellingen zorgvuldig voordat u gaat delen.

## Documentmachtigingen

Machtigingen gelden specifiek voor één item in Workfront en definiëren welke handelingen u op dat item kunt uitvoeren. Voor informatie over objecten toestemmingen, zie [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

In de volgende tabel wordt aangegeven welke machtigingen u gebruikers kunt verlenen wanneer zij documenten mogen weergeven of beheren:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong> Actie </strong> </p> </th> 
   <th> <p><strong>Managen</strong> </p> </th> 
   <th> <p><strong>Uitzicht</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Creëer</td> 
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
   <td scope="row">Voeg goedkeuringspersonen toe</td> 
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
   <td scope="row">Updates/ Reacties</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Upload nieuwe versie</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Verwijder versie</td> 
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
   <td scope="row">Verwijder Bewijs**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Deel systeembreed*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Delen documenten openbaar*</td> 
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
   <td scope="row">Link (met integratie)</td> 
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

&#42; Actie wordt gedeeld door zowel Documenten- als Documentmappen.

&#42;&#42; U moet een aparte proefdruklicentie aan uw Workfront-account hebben gekoppeld om documenten te kunnen controleren. Neem contact op met uw accountmanager voor het verkrijgen van een proefdruklicentie. Voor meer informatie over het proef in Workfront, zie [ het Bewijzen ](../../review-and-approve-work/proofing/proofing.md).

## Overwegingen bij het delen van documenten

Naast de overwegingen hieronder, zie ook [ Overzicht van het delen van toestemmingen op voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Een Workfront-beheerder kan machtigingen toevoegen of verwijderen voor alle items in het systeem, zonder de eigenaar van die items te zijn.

* Een document delen is vergelijkbaar met het delen van een ander object in Workfront. Voor informatie over hoe te om documenten in Workfront te delen, zie [ een voorwerp ](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md) delen.
* Je kunt de volgende rechten aan documenten geven:

   * Uitzicht
   * Managen

* U kunt een document ook openbaar of systeembreed delen.

  >[!CAUTION]
  >
  >We raden u aan voorzichtig te zijn wanneer u een object met vertrouwelijke informatie deelt met externe gebruikers. Dit stelt hen in staat informatie te bekijken zonder Workfront-gebruiker te zijn of deel uit te maken van uw organisatie.

* Je kunt een document delen met iemand die geen Workfront-account heeft, door hun e-mailadres toe te voegen in het veld &#39;Geef document toegang toe.
* Wanneer je een document deelt, hebben gebruikers dezelfde toegang tot alle documentversies en alle documentbewijzen.\
  Voor meer informatie over proefdrukken in Workfront, zie de [sectie Proefdrukken](../../review-and-approve-work/proofing/proofing.md) .

* Je kunt rechten op documenten erven van de objecten waarmee ze gekoppeld zijn. Je Workfront-beheerder kan de overerving van rechten voor documenten in jouw toegangsniveau beperken.

  Voor meer informatie over het beperken van geërfte toestemmingen op documenten, zie [ tot douanetoegangsniveaus ](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) leiden of wijzigen.

  U kunt overgeërfde machtigingen voor documenten handmatig verwijderen. Voor meer informatie, zie [ toestemmingen uit voorwerpen ](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md) verwijderen

* Een bijgevoegd document neemt alleen machtigingen over van het object waaraan het is gekoppeld. Als u een map voor het object maakt en het document naar de map verplaatst, neemt deze de machtigingen van de map over. Maar als u een map maakt op een bovenliggend of bovenliggend object en het document naar die map verplaatst, worden de machtigingen van die map niet overgenomen.