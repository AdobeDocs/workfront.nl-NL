---
user-type: administrator
product-area: system-administration;user-management
keywords: beheren,subgroep,bewerken
navigation-topic: create-and-manage-subgroups
title: Een subgroep beheren
description: Als groepsbeheerder van een subgroep kunt u de subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren en verwijderen. U kunt een subgroep ook tot een bovenste groep maken door deze uit de bovenliggende groep te verwijderen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 1%

---

# Een subgroep beheren

Als groepsbeheerder van een subgroep kunt u de subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren en verwijderen.

U kunt een subgroep ook tot een bovenste groep maken door deze uit de bovenliggende groep te verwijderen.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

Zie voor meer informatie over subgroepen [Overzicht subgroepen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Toegangsvereisten

U moet het volgende hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-abonnement*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> <p>U moet een groepsbeheerder van de groep of een beheerder van Workfront zijn. Zie voor meer informatie <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Groepbeheerders</a> en <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Volledige administratieve toegang verlenen aan een gebruiker</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## Een subgroep maken, verplaatsen, weergeven, bewerken, kopiëren, hernoemen, exporteren of verwijderen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

   In de lijst die wordt weergegeven, ziet u de groepen die u beheert, samen met eventuele subgroepen die u beheert. Adobe Workfront-beheerders kunnen alle groepen zien.

1. Klik op de naam van de groep die de subgroep bevat waarmee u wilt werken.

   of

   Als u een of meer subgroepen verplaatst, klikt u op de naam van de doelgroep (u geeft op welke subgroepen u in een latere stap wilt verplaatsen).

1. Klik in het linkermenu op **Subgroepen**.

1. Voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een nieuwe subgroep maken</td> 
      <td> <p>Als u de nieuwe subgroep één niveau lager wilt maken dan de groep die u bekijkt, klikt u op <strong>Subgroep toevoegen</strong>.</p> <p>Als u de nieuwe subgroep onder een andere subgroep in de lijst wilt maken, selecteert u de subgroep en klikt u op <strong>s toevoegen</strong><strong>subgroep</strong>.</p> <p>Zie de tabel in voor informatie over de opties die u kunt gebruiken om de subgroep te configureren <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Een subgroep maken</a>.</p> <p>Een groepshiërarchie kan niet meer dan 15 niveaus zijn, maar één niveau kan een onbeperkt aantal parallelle groepen hebben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een subgroep verplaatsen </td> 
      <td> <p>U kunt bestaande subgroepen verplaatsen onder een andere groep die u beheert.</p> <p>Een groepshiërarchie kan niet meer dan 15 niveaus zijn, maar één niveau kan een onbeperkt aantal parallelle groepen hebben.</p> 
       <ol> 
        <li value="1"> <p>(Optioneel) Selecteer een subgroep om deze tot de doelgroep te maken.</p> <p>Als u deze stap overslaat, is de groep die u in stap 3 hebt geselecteerd de doelgroep.</p> </li> 
        <li value="2">Klikken <strong>Subgroep toevoegen</strong> &gt; <strong>Bestaande groep</strong>.</li> 
        <li value="3"> <p>In de <strong>Bestaande groep</strong> in het vak dat wordt weergegeven, typt u de naam van een subgroep die u wilt verplaatsen.</p> <p>De resultaten die worden weergegeven, bevatten geen groepen boven de doelgroep.</p> <p>U kunt ervoor zorgen dat u de juiste groep selecteert door de muisaanwijzer boven de groep te plaatsen en op het informatiepictogram te klikken <img src="assets/info-icon.png"> die ernaast wordt weergegeven. Hier wordt knopinfo weergegeven met informatie over de groep, zoals de hiërarchie van de bovenliggende groepen en de bijbehorende beheerders.</p> </li> 
        <li value="4"> <p>Klik op de naam van de subgroep die u wilt verplaatsen wanneer deze in de lijst wordt weergegeven.</p> </li> 
        <li value="5"> <p>Herhaal Stappen c-d voor andere subgroepen u naar de bestemmingsgroep wilt bewegen</p> </li> 
        <li value="6">Klikken <strong>Opslaan</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een subgroep bewerken</td> 
      <td> <p>Selecteer de subgroep die u wilt bewerken en klik op het pictogram Bewerken <img src="assets/edit-icon.png">.</p> <p>Zie de tabel in voor informatie over de opties die u kunt gebruiken om de subgroep te configureren <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Een groep maken</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer subgroepen exporteren</td> 
      <td> 
       <ol> 
        <li value="1">Selecteer de subgroep of subgroepen die u wilt exporteren.</li> 
        <li value="2">Klik op het pictogram Exporteren <img src="assets/export.png">Selecteer vervolgens de gewenste bestandsindeling.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een subgroep kopiëren om een nieuwe groep op hoofdniveau te maken</td> 
      <td> <p>(Alleen beschikbaar voor Workfront-beheerders.) Wanneer u een subgroep kopieert, wordt deze een bovenliggende groep. Alle groepsleden en subgroepen worden ermee gekopieerd. De groepsleden behouden hun toewijzingen in de oorspronkelijke groep.</p> <p>Zie voor meer informatie over het kopiëren van een subgroep <a href="#about-copying-a-subgroup" class="MCXref xref">Subgroepen kopiëren</a> in dit artikel.</p> 
       <ol> 
        <li value="1">Selecteer een subgroep en klik op het pictogram Kopiëren <img src="assets/copy-icon.png"> om een nieuwe groep op hoofdniveau te maken op basis van de geselecteerde groep.</li> 
        <li value="2"> <p>Configureer de instellingen van de nieuwe groep.</p> <p>Zie de tabel in de sectie voor hulp bij deze instellingen <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Een groep op hoofdniveau maken door een bestaande groep of subgroep te kopiëren</a> in het artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Een groep op hoofdniveau maken door een bestaande groep of subgroep te kopiëren</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een subgroep verwijderen</td> 
      <td> <p><b>BELANGRIJK</b>: Wanneer u een groep of subgroep verwijdert, moet u de gebruikers, de werkitems en alle subgroepen die momenteel aan de groep of subgroep zijn toegewezen, behouden. Om ervoor te zorgen dat deze behouden blijven, moet u de objecten van de groep opnieuw toewijzen aan een andere groep in de onderstaande stap.</p> 
       <ol> 
        <li value="1">Selecteer de subgroep en klik op het pictogram Verwijderen <img src="assets/delete.png">.</li> 
        <li value="2">In de <strong>Groep verwijderen</strong> weergegeven, begint u met typen en selecteert u vervolgens de naam van de groep waarnaar u de leden, werkitems en subgroepen van de groep die u verwijdert, wilt verplaatsen.</li> 
        <li value="3">Klikken <strong>Deze verwijderen</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Wanneer u een groep beheert die subgroepen bevat, is het nuttig om gegevens over de gehele groep en alle subgroepen te kunnen identificeren en filteren. U kunt dit doen door het Bovenste gebied van identiteitskaart van de Ouder in een rapport of een lijst te gebruiken.
>
>Bijvoorbeeld, veronderstel dat u een grote afdeling van de Marketing beheert en u een lijst van alle projecten wilt die de volledige afdeling aan werkt.
>
>In Workfront, wordt deze afdeling van de Marketing vertegenwoordigd door een groep genoemd Marketing, met 3 subgroepen genoemd de Marketing van het Gebied, de Marketing van het Product, en Digitale Marketing. Om van de projecten een lijst te maken die tot de volledige afdeling van de Marketing (alle 4 groepen) behoren, kon u een Filter voor het gebied van Projecten met de volgende Regel van de Filter tot stand brengen:
>
>
```
>Group: Top Parent ID > Equal > Marketing
>```
>
>U kunt het Hoogste gebied van de Naam van de Ouder ook gebruiken om gegevens te identificeren verbonden aan een top-level groep, maar slechts in Weergaven, niet in Filters of Groepen.

## Een subgroep verwijderen uit de bovenliggende groep en deze maken tot een groep op hoofdniveau

U kunt van een subgroep een groep op hoofdniveau maken door deze uit de bovenliggende groep te verwijderen.

>[!TIP]
>
>Wanneer u een groep deactiveert die onderliggende subgroepen heeft, worden deze subgroepen ook inactief. Als u wilt dat een van deze besturingselementen actief is, kunt u deze instructies gebruiken om het onderdeel uit de bovenliggende groep te verwijderen en vervolgens opnieuw te activeren.
>
>Zie de secties voor instructies voor het deactiveren en opnieuw activeren van groepen [De details van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) en [De details van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) in het artikel [De details van een groep weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Selecteer de bovenliggende groep van de groep die u als bovenste groep wilt instellen en klik op het pictogram Bewerken ![](assets/edit-icon.png).
1. In de **Groep bewerken** vak dat wordt weergegeven onder **Groepsleden en groepbeheerders** begint u de naam te typen van de subgroep die u wilt instellen als groep op hoofdniveau. Klik vervolgens op de X rechts van de naam ervan wanneer deze wordt weergegeven.
1. Klikken **Opslaan**.

## De subgroepsleden van een groep weergeven en beheren

Wanneer u de hoofdpagina bekijkt van een groep die u beheert, kunt u alle gebruikers in de subgroepen van de groep weergeven en beheren. Zie voor instructies [Subgroepleden weergeven en beheren](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Subgroepen kopiëren {#about-copying-a-subgroup}

Houd rekening met het volgende wanneer u een subgroep kopieert.

* Als een subgroep die u kopieert, zijn eigen subgroepen heeft, worden deze opgenomen in de kopie en krijgen hun namen de volgende notatie:

   ```
   Original subgroup name (Copy)
   ```

* Om het even welke subgroep die tot een openbare groep behoort is ook openbaar, zodat kan om het even welke gebruiker met uitgeven-gebruiker toegang, in of uit de groep, gebruikers aan subgroup toevoegen.
