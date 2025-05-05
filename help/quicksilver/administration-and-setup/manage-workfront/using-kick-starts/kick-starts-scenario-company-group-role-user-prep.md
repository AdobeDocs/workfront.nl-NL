---
user-type: administrator
product-area: system-administration;user-management
keywords: kickstart,trap-start,kickstart,trap-start
navigation-topic: use-kick-starts
title: 'Kick-start Scenario: Bedrijf, Groep, Rol, en de Kick-Begint Voorbereiding van de Gebruiker'
description: Wanneer u begint met het implementeren van Adobe Workfront, in plaats van handmatig gegevens in te voeren, kunt u uw lijst met klanten, interne afdelingen, taakrollen en gebruikersgegevens importeren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b83e2e35-dd9d-4d98-b8d4-2f8718b3c6c1
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1147'
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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong> Bedrijven </strong> </th> 
   <th><strong> Groepen </strong> </th> 
   <th><strong> Rollen </strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td valign="top"> <p>Acme, Co</p> <p>Workfront, Inc.</p> <p><em> Uw Bedrijf </em> </p> <p>XYZ, Inc.</p> </td> 
   <td valign="top"> <p valign="top" rowspan="7">Financiën</p> <p valign="top" rowspan="7">IT </p> <p valign="top" rowspan="7">Marketing </p> <p valign="top" rowspan="7">Verkoop</p> </td> 
   <td valign="top"> <p valign="top">Zakelijke analist</p> <p valign="top">Controller, creatief</p> <p valign="top">Designer</p> <p valign="top">Resource Manager</p> <p valign="top">Scrumstramien</p> <p valign="top">Technisch schrijver</p> <p valign="top">Webontwikkelaar</p> </td> 
  </tr> 
 </tbody> 
</table>

Rolnamen moeten uniek zijn. Bestaande taakrollen kunnen niet worden geïmporteerd.

In de volgende tabellen worden de te importeren gebruikers en diverse gebruikerskenmerken voor elke tabel weergegeven:

### Gebruiker 1

| **Voornaam** | Chris |
|---|---|
| **Achternaam** | Manning |
| **Gebruikersnaam/E-mail** | mailto:cmanning@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Teamlid |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | Zakelijke analist |

{style="table-layout:auto"}

### Gebruiker 2

| **Voornaam** | Jennifer |
|---|---|
| **Achternaam** | Campbell |
| **Gebruikersnaam/E-mail** | jcampbell@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Projectmanager |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | Projectmanager |

{style="table-layout:auto"}

### Gebruiker 3

| **Voornaam** | Jill |
|---|---|
| **Achternaam** | Sullivan |
| **Gebruikersnaam/E-mail** | jsullivan@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Helpdesk |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Verkoop |
| **Rol van de Baan** | Verkoopvertegenwoordiger |

{style="table-layout:auto"}

### Gebruiker 4

| **Voornaam** | Marc |
|---|---|
| **Achternaam** | Lewis |
| **Gebruikersnaam/E-mail** | mlewis@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Portfolio Manager |
| **Bedrijf** | &lt;*Uw Bedrijf>* |
| **Groep van het Huis** | Financiën |
| **Rol van de Baan** | Controller |

{style="table-layout:auto"}

### Gebruiker 5

| **Voornaam** | Pam |
|---|---|
| **Achternaam** | Reynolds |
| **Gebruikersnaam/E-mail** | preynolds@foo.com |
| **Wachtwoord** | updateMe |
| **Toegang** | Projectmanager |
| **Bedrijf** | *Uw Bedrijf>* |
| **Groep van het Huis** | Marketing |
| **Rol van de Baan** | IT |

{style="table-layout:auto"}

### Gebruiker 6

| **Voornaam** | Ray |
|---|---|
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

## Informatie over invoerbedrijf

1. Open het {**dossier 0} Workfront.xlsx u enkel downloadde.**

   >[!TIP]
   >
   >Als u met zeer brede gegevensbladen werkt, kunt u het gereedschap Venster vastzetten (of equivalent) van de werkbladeditor gebruiken om het werkblad gemakkelijker te maken.

1. Ga naar het blad &#39;CMPY Company&#39;.

   Het zou leeg moeten zijn tenzij de bedrijven reeds in het systeem zijn. ![ blad van het Bedrijf ](assets/cmpysheet-350x16.png)

   ![ identiteitskaart van het Bedrijf ](assets/companyid--1--350x78.png)

1. Specificeer WAAR in de **isNew** kolom.
1. Herhaal deze handeling voor elk bedrijf dat wordt toegevoegd. (In dit voorbeeld voert u deze handeling uit voor de rijen 3-6, omdat er vier bedrijven worden toegevoegd.)

   ![ Bedrijf is nieuw ](assets/cmpyisnew-350x86.png)

1. Geef een unieke id op.

   Dit moet voor elke rij voor de kolom van identiteitskaart worden gedaan. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Bedrijf is nieuw ](assets/cmpyisnew-350x86.png)

1. Stel een naam in.

   Specificeer de namen van elke klant in de **setName** kolom.

   ![ identiteitskaart van het Bedrijf ](assets/companyid-350x78.png)

1. Ga naar het groepsblad van de GROEP.

   Tenzij u al groepen hebt gemaakt in Workfront, wordt op dit blad alleen de standaardgroep weergegeven die is ingericht voor elke account van Workfront.

   ![&#128279;](assets/groupsheet-350x15.png) ![ Lege groepsblad van 0&rbrace; Groep ](assets/emptygroupsheet-350x85.png)

1. Plaats **isNew** column.Volgens het scenario, zullen 4 groepen worden ingevoerd, zo specificeer WAAR in rijen 4 door 7 voor de &quot;isNew&quot;kolom.
1. Geef een unieke id op.

   Dit moet voor elke rij voor de kolom van identiteitskaart worden gedaan. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Groep IDs ](assets/groupids-350x85.png)

1. Stel een naam in.

   Specificeer de namen van elke afdeling in de **setName** kolom.

   ![ de namen van de Groep ](assets/groupnames-350x85.png)

   Rolgegevens opgeven. Ga naar het Rolblad van de ROL.

1. Tenzij u al rollen in uw account hebt gemaakt of verwijderd, moet dit blad 8 rollen weergeven die zijn ingericht voor elke account van Workfront.

   ![ de namen van de Groep ](assets/groupnames-350x85.png)

1. True instellen, instructie.

   Zeven de Rollen van de Baan invoeren, input WAAR in rijen 12 door 18 voor de &quot;isNew&quot;kolom.

   ![ Rol is nieuw ](assets/roleisnew-350x104.png)

1. Geef een unieke id op.

   Dit moet voor elke rij voor de kolom van identiteitskaart worden gedaan. Gehele getallen die bij 1 beginnen, werken goed bij het maken van nieuwe records.

   ![ Gebruikersblad ](assets/usersheet-350x16.png)

   ![ Rol is nieuw ](assets/roleisnew--1--350x104.png)

1. Geef een naam voor elke rol op door deze in de kolom setName te typen.

   ![ Rol is nieuw ](assets/roleisnew-350x104.png)

1. Geef zo nodig aanvullende gegevens op.

   Neem indien nodig factureringssnelheden, kostentarieven en beschrijvingen op voor de rollen die u maakt.

1. Ga naar het Gebruikersblad van de GEBRUIKER om de Informatie van de Gebruiker in te voeren.

   Tenzij u al gebruikers in uw account hebt gemaakt, wordt op dit blad alleen de Admin-gebruiker weergegeven die voor elke account van Workfront is ingericht.

   ![&#128279;](assets/rolenames-350x104.png) ![ Lege gebruikersblad van de Rol 0&rbrace; ](assets/emptyusersheet-350x52.png)

1. Stel de waarde True in door TRUE op te geven in de rijen 4 tot en met 9 voor de kolom &#39;isNew&#39;, aangezien er 6 gebruikers worden geïmporteerd.

   ![ Gebruiker is nieuw ](assets/userisnew-350x52.png)

1. Stel een unieke id in door in elke rij een unieke id voor de kolom Id op te geven. Gewoonlijk werken gehele getallen vanaf 1 goed voor nieuwe records.

   ![ Gebruiker is nieuw ](assets/userisnew-350x52.png)

1. Voer de namen van elke gebruiker in de kolommen &#39;setFirstName&#39; en &#39;setLastName&#39; in.

   ![ Gebruikersnamen ](assets/usernames-350x52.png)

1. Stel detailwaarden in door waarden op te geven in de kolommen &#39;setEmail&#39;, &#39;setPassword&#39; en &#39;setGebruikersnaam&#39;.

   ![ geloofsbrieven van de Gebruiker ](assets/usercredentials-350x52.png)

1. Geef waarden op voor Toegangsniveau.

   Bijvoorbeeld, Chris Manning, die een Lid van het Team is, kijkt omhoog identiteitskaart op het blad van het Niveau van de Toegang van ACSLVL voor het de toegangsniveau van het Lid van het Team. Kopieer identiteitskaart in uw klembord, en op het blad van de Gebruiker kleeft het in de **setAccessLevelID** kolom op de rij van Chris.

   Herhaal deze stap voor elke gebruiker en toegangsniveau.

   ![ identiteitskaart van het de toegangsniveau van het Exemplaar ](assets/copyalid-350x171.png) ![ identiteitskaart van het de toegangsniveau van het Deeg ](assets/pastealid-350x59.png)

1. Geef de gegevens van de thuisgroep op.

   Volgens het scenario behoort Chris Manning tot de marketinggroep. Op het blad van de Groep van de GROEP, bepaal de plaats van identiteitskaart voor de groep van de Marketing, kopieer het in het klembord, en op het blad van de Gebruiker kleeft het in **setHomeGroupID** kolom op Chris&#39; rij. &#x200B;Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ de groepsidentiteitskaart van het Exemplaar ](assets/copygroupid-1-350x133.png) ![ groepsidentiteitskaart van het Deeg ](assets/pastegroupid-350x59.png)

1. Geef bedrijfsgegevens op.

   Alle gebruikers in dit scenario behoren tot hetzelfde bedrijf. Voor het blad van het Bedrijf CMPY, bepaal de plaats van identiteitskaart voor *Your Ewn Bedrijf *company, kopieer identiteitskaart in het klembord, en op het lusje van de Gebruiker van de GEBRUIKER, kleef deze waarde in elke rij van de kolom &quot;setCompanyID&quot;&#x200B;

   Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ identiteitskaart van het Bedrijf ](assets/companyid--1--350x78.png)

   ![ bedrijf identiteitskaart van het Deeg ](assets/pastecompanyid-350x84.png)

1. Geef taakroldetails op.

   Volgens het scenario, zal Chris Manning de rol van BedrijfsAnalyst hebben. Voor het blad van de Rol van de ROL van de ROL, bepaal de plaats identiteitskaart voor de rol BedrijfsAnalyst, kopieer het in het klembord, en op het blad van de Gebruiker kleef het in de kolom &quot;setRoleID&quot;op Chris&#39; rij. &#x200B;Herhaal deze stap voor elke gebruiker en groepstoewijzing.

   ![ identiteitskaart van de rol van het Exemplaar ](assets/copyroleid-350x149.png)

   ![ identiteitskaart van de rol van het Deeg ](assets/pasteroleid-350x95.png)

1. Vul desgewenst andere gebruikersgegevens in en sla het bestand op.
1. Het Excel-bestand importeren.

   Volg de richtingen die in [ worden verstrekt de gegevens van de Invoer in Adobe Workfront gebruikend een Kick-Begin malplaatje ](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
