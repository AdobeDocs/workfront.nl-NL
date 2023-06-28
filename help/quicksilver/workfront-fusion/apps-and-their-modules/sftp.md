---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP-modules
description: De [!DNL Adobe Workfront Fusion SFTP] kunt u bestandswijzigingen in een geselecteerde map of submap controleren, nieuwe bestanden naar de gewenste map uploaden, bestaande bestanden die zich al in een map bevinden, wijzigen of verwijderen, of bestandsmachtigingen wijzigen.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1698'
ht-degree: 0%

---

# SFTP-modules

De [!DNL Adobe Workfront Fusion] SFMet TP-modules kunt u bestandswijzigingen in een geselecteerde map of submap controleren, nieuwe bestanden naar de gewenste map uploaden, bestaande bestanden die zich al in een map bevinden wijzigen of verwijderen of de bestandsmachtigingen wijzigen.

## Toegangsvereisten

U moet de volgende toegang hebben om de functionaliteit in dit artikel te kunnen gebruiken:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] of hoger</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licentie**</td> 
   <td>
   <p>Huidige vergunningsvereiste: Nee [!DNL Workfront Fusion] vergunningsvereiste.</p>
   <p>of</p>
   <p>Vereisten voor oudere licenties: [!UICONTROL [!DNL Workfront Fusion] voor werkautomatisering en -integratie] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Huidige productvereisten: Als u de [!UICONTROL Select] of [!UICONTROL Prime] [!DNL Adobe Workfront] Abonnement, uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken. [!DNL Workfront Fusion] is opgenomen in de [!UICONTROL Ultimate] [!DNL Workfront] plannen.</p>
   <p>of</p>
   <p>Oudere productvereisten: Uw organisatie moet [!DNL Adobe Workfront Fusion] alsmede [!DNL Adobe Workfront] om de in dit artikel beschreven functionaliteit te gebruiken.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Neem contact op met uw [!DNL Workfront] beheerder.

Voor informatie over [!DNL Adobe Workfront Fusion] licenties, zie [[!DNL Adobe Workfront Fusion] licenties](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Vereisten

Voor het gebruik van SFTP met [!DNL Workfront Fusion], is het noodzakelijk een SFTP-account te hebben (zoals [!DNL GoDaddy] webhosting).

## SFTP verbinden met [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Uw SFTP-account verbinden met [!DNL Workfront Fusion] u moet de doelGastheer en de geloofsbrieven van SFTP (gebruikersnaam en wachtwoord of gebruikersnaam en sleutel) aan de module ingaan [!UICONTROL Create a connection] .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection name]</td> 
   <td> <p> Voer de naam in voor uw SFTP-verbinding.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Voer de hostnaam in van de SFTP-server waarmee u verbinding wilt maken.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Voer de SFTP-serverpoort in. Bijvoorbeeld 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Auth type]</p> </td> 
   <td> <p>Selecteer de machtigingsmethode die u wilt gebruiken om verbinding te maken met de SFTP-server.</p> 
    <ul> 
     <li><strong>[!UICONTROL User name and password]</strong>: Voer uw referenties in.</li> 
     <li> <p><strong>[!UICONTROL User name and key]</strong>: Voer uw gebruikersnaam en persoonlijke sleutel/certificaat in</p> <p>Upload de persoonlijke sleutel om de clientverificatie te gebruiken of upload uw certificaat (P12- of PFX-bestand) als u TLS wilt gebruiken met uw zelfondertekende certificaat. Als u de client-side certificaatautorisatie gebruikt, kunt u hier uw CA-certificaat invoeren.</p> <p>[!DNL Workfront Fusion] bewaart of bewaart geen gegevens (dossiers, wachtwoorden) u hier verstrekt. Bestand en wachtwoord worden alleen gebruikt om een persoonlijke sleutel of certificaat te extraheren.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Na het invoeren van de verbindingsgegevens klikt u op **[!UICONTROL Continue]** om een verbinding tot stand te brengen.

## [!UICONTROL SFTP] modules en hun velden

Wanneer u [!UICONTROL SFTP] modules, [!DNL Workfront Fusion] geeft de onderstaande velden weer. Samen met deze [!UICONTROL SFTP] er worden mogelijk velden weergegeven, afhankelijk van factoren zoals uw toegangsniveau in de app of service. Een bolde titel in een module wijst op een vereist gebied.

Als u de kaartknoop boven een gebied of een functie ziet, kunt u het gebruiken om variabelen en functies voor dat gebied te plaatsen. Zie voor meer informatie [De informatie van de kaart van één module aan een andere binnen [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### [!UICONTROL Watch Files in a Folder]

Hiermee worden bestanden met details geretourneerd wanneer een bestand in een opgegeven map wordt gemaakt of gewijzigd.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Voer de map in die u wilt controleren of wijs deze toe. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Buffergrootte [B]</td> 
   <td> <p> Voer de buffergrootte in bytes in. De waarde definieert de grootte van overgedragen blokken van de server. Sommige servers kunnen problemen veroorzaken of bestanden beschadigen wanneer de waarde te hoog is.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
   <td> <p> Het maximum aantal bestanden instellen dat [!DNL Workfront Fusion] werkt met één cyclus</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Watch Subfolders in a Folder]

Retourneert mappen met details wanneer een map wordt gemaakt of gewijzigd in een opgegeven map.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Voer de map in die u wilt controleren of wijs deze toe. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned files]</td> 
   <td> <p> Het maximum aantal mappen instellen [!DNL Workfront Fusion] zal gedurende één cyclus terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Handelingen

#### [!UICONTROL List a folder's content]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Selecteer of u bestanden, mappen of beide wilt ophalen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Voer de map in of wijs de map toe die de bestanden of mappen bevat die u wilt weergeven. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Voer de zoekterm in of wijs deze toe. Als u bijvoorbeeld naar bestanden met de bestandsextensie .txt wilt zoeken, voert u <code>.txt</code>.U kunt ook de naam invoeren of toewijzen van het bestand waarnaar u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort By]</td> 
   <td> <p> Selecteer of u de resultaten wilt sorteren op bestandsnaam, grootte, datum van laatste toegang of datum van laatste wijziging.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort Order] </td> 
   <td> <p>Selecteer of het resultaat in oplopende of aflopende volgorde moet worden geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continue the execution of the route even if the module returns no results]</p> </td> 
   <td>Schakel deze optie in om ervoor te zorgen dat deze module het scenario niet stopt als het geen resultaten retourneert.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Stel het maximale aantal resultaten in dat [!DNL Workfront Fusion] zal gedurende één cyclus terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Files]

In deze module worden bestanden uit een opgegeven map weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buffer Size [B]]</td> 
   <td> <p> Voer de buffergrootte in bytes in. De waarde definieert de grootte van overgedragen blokken van de server. Sommige servers kunnen problemen veroorzaken of bestanden beschadigen wanneer de waarde te hoog is.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Voer de map in of wijs de map toe die de bestanden of mappen bevat die u wilt weergeven. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Voer de zoekterm in of wijs deze toe. Als u bijvoorbeeld naar bestanden met de bestandsextensie .txt wilt zoeken, voert u <code>.txt</code>.U kunt ook de naam invoeren of toewijzen van het bestand waarnaar u wilt zoeken.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort By]</td> 
   <td> <p> Selecteer of u de resultaten wilt sorteren op de bestandsnaam, grootte, datum van laatste toegang of datum van laatste wijziging.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sort Order]</td> 
   <td> <p> Selecteer of het resultaat in oplopende of aflopende volgorde moet worden geretourneerd.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Continue the execution of the route even if the module returns no results]</p> </td> 
   <td>Schakel deze optie in om ervoor te zorgen dat deze module het scenario niet stopt als het geen resultaten retourneert.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of returned results]</td> 
   <td> <p> Het maximum aantal bestanden instellen dat [!DNL Workfront Fusion] zal gedurende één cyclus terugkeren.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a File]

In deze module worden de bestandsgegevens opgehaald, inclusief de gegevens van een bestand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Buffer Size [B]]</td> 
   <td> <p> Voer de buffergrootte in bytes in. De waarde definieert de grootte van overgedragen blokken van de server. Sommige servers kunnen problemen veroorzaken of bestanden beschadigen wanneer de waarde te hoog is.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path] </td> 
   <td> <p>Voer het pad naar het bestand in. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a File]

Met deze module kunt u een bestand uploaden naar de SFTP-server.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Geef een bestaande map op als opslaglocatie voor het bestand. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source File]</td> 
   <td> <p> Wijs het bronbestand van een vorige module toe, zoals [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. U kunt ook de bestandsnaam en de bestandsgegevens invoeren of toewijzen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Stel de gewenste machtigingen in voor het bestand of de map. Gebruik chmod-parameters. Bijvoorbeeld: <code>777 </code>of <code>-rwxrwxrwx</code>.</p> <p>Voor meer informatie over chmod raadpleegt u de <a href="https://ss64.com/bash/chmod.html">chmod-documentatie</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rename a File]

Wijzigt de naam van een bestand.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Voer het pad in naar het bestand waarvan u de naam wilt wijzigen. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New file name]</td> 
   <td> <p> Voer de nieuwe naam voor het bestand in, inclusief de bestandsextensie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Voer het pad in naar het bestand dat u wilt verplaatsen. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New Folder]</td> 
   <td> <p> Voer het pad naar de nieuwe locatie van het bestand in. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Voer het pad in naar het bestand dat u wilt verwijderen. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update file permissions]

Hiermee kunt u machtigingen voor het bestand wijzigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL File Path]</td> 
   <td> <p> Voer het pad in naar het bestand dat u wilt verplaatsen. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Stel de gewenste bestandsmachtigingen in. Gebruik de parameters chmod. Bijvoorbeeld: <code>777 </code>of <code>-rwxrwxrwx</code>.</p> <p>Moet overeenkomen met patroon <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Voor meer informatie over chmod raadpleegt u de <a href="https://ss64.com/bash/chmod.html">chmod-documentatie</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Folder]

Maakt een nieuwe map op de opgegeven locatie.

>[!NOTE]
>
>Als de map al bestaat, genereert de module een fout. Om de stroom ononderbroken voort te zetten, maak een route van de foutenmanager aan de module vast om de fout te vangen en aan te wenden [!UICONTROL Resume] de richtlijn om de doorstroming voort te zetten. Voor informatie over het vastmaken van een route van de foutenmanager, zie [Foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Voor informatie over de route van de foutenmanager, zie [Richtlijnen voor foutafhandeling in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Geef een bestaande map op als opslaglocatie voor de nieuwe map. U kunt een absoluut pad opgeven, zoals <code>/home/user/file.txt</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name]</td> 
   <td> <p> Voer de mapnaam in.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Permissions]</p> </td> 
   <td> <p>Stel de gewenste mapmachtigingen in. Gebruik chmod-parameters. Bijvoorbeeld: <code>777 </code>of <code>-rwxrwxrwx</code>.</p> <p>Moet overeenkomen met patroon <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Voor meer informatie over chmod raadpleegt u de <a href="https://ss64.com/bash/chmod.html">chmod Man Page</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Folder]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td>
   <td> <p>Voor instructies over het aansluiten van uw SFTP-account op [!DNL Workfront Fusion], zie <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden met [!DNL Workfront Fusion]</a> in dit artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Geef het pad op naar de map die u wilt verwijderen. U kunt een absoluut pad opgeven, zoals <code>/home/user/</code>. U kunt ook een relatief pad opgeven dat verwijst naar een specifieke map van de aangemelde gebruiker, zoals <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
