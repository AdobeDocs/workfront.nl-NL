---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: 'Kick-start Scenario: Bedrijf, Groep, Rol, en de Kick-Begint Voorbereiding van de Gebruiker'
description: Wanneer u begint met het implementeren van Adobe Workfront, in plaats van handmatig gegevens in te voeren, kunt u uw lijst met klanten, interne afdelingen, taakrollen en gebruikersgegevens importeren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 59431354076a0909fb1878d68cf266f08d2114b3
workflow-type: tm+mt
source-wordcount: '1213'
ht-degree: 0%

---

# Kick-Starts scenario: bedrijf, groep, rol, en gebruiker Kick-Start voorbereiding

Wanneer u begint met het implementeren van Adobe Workfront, in plaats van handmatig gegevens in te voeren, kunt u uw lijst met klanten, interne afdelingen, taakrollen en gebruikersgegevens importeren.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

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
   <td>
   <p> Nieuw: Standaard</p>
   of
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wat u kunt importeren

In de volgende tabel worden de bedrijven, groepen en rollen weergegeven die moeten worden geïmporteerd:

| Bedrijven | Groepen | Rollen |
|---|---|---|
| Acme, Co <p>Workfront, Inc. <p>_Uw Bedrijf_ <p>XYZ, Inc. | Financiën <p>IT <p>Marketing <p>Verkoop | Zakelijke analist <p>Controller Creative <p>Designer <p>Resource Manager <p>Scrumstramien <p>Technisch schrijver <p>Webontwikkelaar |

{style="table-layout:auto"}

Rolnamen moeten uniek zijn. Bestaande taakrollen kunnen niet worden geïmporteerd.

In de volgende tabellen worden de te importeren gebruikers en diverse gebruikerskenmerken voor elke tabel weergegeven:

### Gebruiker 1

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Chris |
| **Achternaam** | Manning |
| **Gebruikersnaam/E-mail** | mailto:cmanning@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Teamlid |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | Zakelijke analist |

{style="table-layout:auto"}

### Gebruiker 2

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Jennifer |
| **Achternaam** | Campbell |
| **Gebruikersnaam/E-mail** | jcampbell@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Projectmanager |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | Projectmanager |

{style="table-layout:auto"}

### Gebruiker 3

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Jill |
| **Achternaam** | Sullivan |
| **Gebruikersnaam/E-mail** | jsullivan@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Helpdesk |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Verkoop |
| **Rol van de Baan** | Verkoopvertegenwoordiger |

{style="table-layout:auto"}

### Gebruiker 4

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Marc |
| **Achternaam** | Lewis |
| **Gebruikersnaam/E-mail** | mlewis@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Portfolio Manager |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Financiën |
| **Rol van de Baan** | Controller |

{style="table-layout:auto"}

### Gebruiker 5

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Pam |
| **Achternaam** | Reynolds |
| **Gebruikersnaam/E-mail** | preynolds@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Projectmanager |
| **Bedrijf** | *Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | IT |

{style="table-layout:auto"}

### Gebruiker 6

| Kenmerk | Waarde |
|---|---|
| **Voornaam** | Ray |
| **Achternaam** | Andrews |
| **Gebruikersnaam/E-mail** | randrews@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Beheerder |
| **Bedrijf** | *Uw Bedrijf>* |
| **Groep van het Huis** | Resource Manager |
| **Rol van de Baan** | none |

{style="table-layout:auto"}

## Een Kick-Start-sjabloon downloaden

{{step-1-to-setup}}

1. Klik **Systeem** > **Kick-Begint** > **de Gegevens van de Invoer.**

1. Klik **Meer Opties** om de volledige lijst van de invoeropties te zien.
1. Selecteer het Niveau van de Toegang, Bedrijf, Groep, de Rol van de Baan, en de voorwerpen van de Gebruiker die u wilt invoeren.
1. Klik **Download**.

## Informatie over invoerbedrijf

1. Open het {**dossier 0} Workfront.xlsx u enkel downloadde.**

   >[!TIP]
   >
   >Als u met zeer brede gegevensbladen werkt, kunt u het gereedschap Venster vastzetten (of equivalent) van de werkbladeditor gebruiken om het werkblad gemakkelijker te maken.

1. Ga naar het **blad van het Bedrijf 0&rbrace; CMPY.**

   Het zou leeg moeten zijn tenzij de bedrijven reeds in het systeem zijn.

   ![ blad van het Bedrijf ](assets/cmpysheet-350x16.png) ![ identiteitskaart van het Bedrijf ](assets/companyid--1--350x78.png)

1. Ga **WAAR** in **isNew** kolom in.

   Herhaal deze handeling voor elk bedrijf dat wordt toegevoegd. (In dit voorbeeld voert u deze handeling uit voor de rijen 3-6, omdat er vier bedrijven worden toegevoegd.)

   ![ Bedrijf is nieuw ](assets/cmpyisnew-350x86.png)

1. Ga een unieke **identiteitskaart** in.

   U moet een id invoeren voor elke rij. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Bedrijf is nieuw ](assets/cmpyisnew-350x86.png)

1. Ga de namen van elke klant in de **setName** kolom in.

   ![ identiteitskaart van het Bedrijf ](assets/companyid-350x78.png)

1. Ga naar het **blad van de Groep van de GROEP**.

   Tenzij u al groepen hebt gemaakt in Workfront, wordt op dit blad alleen de standaardgroep weergegeven die is ingericht voor elke account van Workfront.

   ![&#128279;](assets/groupsheet-350x15.png) ![ Lege groepsblad van 0&rbrace; Groep ](assets/emptygroupsheet-350x85.png)

1. Ga **WAAR** in **isNew** kolom in.

   Volgens het scenario, zullen 4 groepen worden ingevoerd, zodat ga **WAAR** in **isNew** kolom voor rijen 4 door 7 in.

1. Ga een unieke **identiteitskaart** in.

   U moet een id invoeren voor elke rij. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Groep IDs ](assets/groupids-350x85.png)

1. Ga de namen van elke afdeling in de **setName** kolom in.

   ![ de namen van de Groep ](assets/groupnames-350x85.png)

1. Ga naar het **blad van de Rol 0&rbrace; ROL.**

   Tenzij u al rollen in uw account hebt gemaakt of verwijderd, moet dit blad 8 rollen weergeven die zijn ingericht voor elke account van Workfront.

   ![ de namen van de Groep ](assets/groupnames-350x85.png)

1. Ga **WAAR** in **isNew** kolom in.

   Volgens het scenario, 7 Rollen van de Baan zullen worden ingevoerd, zodat ga **WAAR** in **isNew** kolom voor rijen 12 door 18 in.

   ![ Rol is nieuw ](assets/roleisnew-350x104.png)

1. Ga een unieke **identiteitskaart** in.

   U moet een id invoeren voor elke rij. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Rol is nieuw ](assets/roleisnew--1--350x104.png)

1. Ga een naam voor elke rol in de **setName** kolom in.

   ![ Rol is nieuw ](assets/roleisnew-350x104.png)

1. Geef zo nodig aanvullende gegevens op.

   Neem indien nodig factureringssnelheden, kostentarieven en beschrijvingen op voor de rollen die u maakt.

1. Ga naar het **blad van de Gebruiker 0&rbrace; GEBRUIKER.**

   Tenzij u al gebruikers in uw account hebt gemaakt, wordt op dit blad alleen de Admin-gebruiker weergegeven die voor elke account van Workfront is ingericht.

   ![ Gebruikersblad ](assets/usersheet-350x16.png) ![ Lege gebruikersblad ](assets/emptyusersheet-350x52.png)

1. Ga **WAAR** in **isNew** kolom in.

   Volgens het scenario, zullen 6 gebruikers worden ingevoerd, zodat ga **WAAR** in **isNew** kolom voor rijen 4 door 9 in.

   ![ Gebruiker is nieuw ](assets/userisnew-350x52.png)

1. Ga een unieke **identiteitskaart** in.

   U moet een id invoeren voor elke rij. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Gebruiker is nieuw ](assets/userisnew-350x52.png)

1. Ga de namen van elke gebruiker in **setFirstName** en **setLastName** kolommen in.

   ![ Gebruikersnamen ](assets/usernames-350x52.png)

1. Plaats detailwaarden door waarden in te gaan in **setEmail**, **setPassword**, en **setGebruikersnaam** kolommen.

   ![ geloofsbrieven van de Gebruiker ](assets/usercredentials-350x52.png)

1. Geef waarden op voor Toegangsniveau.

   Chris Manning is bijvoorbeeld een teamlid. Zoek omhoog identiteitskaart op het **blad van het Niveau van de Toegang 0&rbrace; ACSLVL voor het de toegangsniveau van het Lid van het Team.** Kopieer identiteitskaart, en op het **blad van de Gebruiker van de 0&rbrace; GEBRUIKER kleeft het in de** setAccessLevelID **kolom op de rij van die gebruiker.**

   Herhaal deze stap voor elke gebruiker en toegangsniveau.

   ![ identiteitskaart van het de toegangsniveau van het Exemplaar ](assets/copyalid-350x171.png) ![ identiteitskaart van het de toegangsniveau van het Deeg ](assets/pastealid-350x59.png)

1. Voer de gegevens van de thuisgroep van de gebruiker in.

   Volgens het scenario behoort Chris Manning tot de marketinggroep. Op het **blad van de Groep van 0&rbrace; GROEP, bepaal de plaats van identiteitskaart voor de Marketing groep, kopieer het, en op het** 3&rbrace; blad van de Gebruiker van de GEBRUIKER het in de **setHomeGroupID** kolom op de rij van de gebruiker. &#x200B;**&#x200B;** Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ de groepsidentiteitskaart van het Exemplaar ](assets/copygroupid-1-350x133.png) ![ groepsidentiteitskaart van het Deeg ](assets/pastegroupid-350x59.png)

1. Voer de bedrijfsgegevens van de gebruiker in.

   Alle gebruikers in dit scenario behoren tot hetzelfde bedrijf. Op het **blad van het Bedrijf van de STEEKPROEF**, bepaal de plaats van identiteitskaart voor het **Uw Eigen bedrijf** bedrijf, kopieer identiteitskaart, en op het **lusje van de Gebruiker van de GEBRUIKER**, kleef deze waarde in elke rij van de **setCompanyID** kolom. &#x200B;

   Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ identiteitskaart van het Bedrijf ](assets/companyid--1--350x78.png) ![ bedrijf identiteitskaart van het Deeg ](assets/pastecompanyid-350x84.png)

1. Voer de taakdetails van de gebruiker in.

   Volgens het scenario, zal Chris Manning de rol van BedrijfsAnalyst hebben. Op het **blad van de Rol van 0&rbrace; ROL, bepaal de plaats van identiteitskaart voor de rol Bedrijfs van de Analysator, kopieer het, en op het** blad van de Gebruiker **kleeft het in de** setRoleID **kolom op de rij van de gebruiker. &#x200B;** Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ rolidentiteitskaart van het Exemplaar ](assets/copyroleid-350x149.png) ![ rolidentiteitskaart van het Deeg ](assets/pasteroleid-350x95.png)

1. Vul desgewenst andere gebruikersgegevens in en sla het bestand op.
1. Het Excel-bestand importeren.

   Volg de richtingen die in [ worden verstrekt de gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

>[!NOTE]
>
>Gebruikers die naar Workfront zijn geïmporteerd, worden in de status Deactiveerd en In afwachting van goedkeuring gemaakt.
> 
>Als uw organisatie naar de Adobe Admin Console is gemigreerd en een gebruiker binnen een paar minuten niet de status gedeactiveerd en In afwachting van goedkeuring verlaat, kunt u de batch gebruikers rechtstreeks aan de Adobe Admin Console toevoegen.
>
>Voor instructies, zie [ veelvoudige gebruikers beheren | Bulk CSV upload ](https://helpx.adobe.com/nl/enterprise/using/bulk-upload-users.html) in de documentatie van Adobe.
