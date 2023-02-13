---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: De projectsjablonen van een groep maken en wijzigen
description: Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met projectmalplaatjes bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# De projectsjablonen van een groep maken en wijzigen

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met projectmalplaatjes bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

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
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Toegang tot of hoger weergeven voor de sjablonen die u wilt weergeven en waarmee u wilt werken</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de Workfront-beheerder als u wilt weten welk abonnement- of licentietype u hebt.

## De mening, het werk met, en creeert malplaatjes voor uw groep van het gebied van Groepen

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).

1. Klik in het linkerdeelvenster op **Groepen** ![](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u sjablonen wilt maken of wijzigen.
1. Klik in het linkerdeelvenster op **Sjablonen** om een lijst te maken van de malplaatjes die met de groep en met om het even welke subgroups worden geassocieerd het zou kunnen hebben.

   U moet toegang tot een sjabloon weergeven als u de sjabloon in deze lijst wilt zien. Voor informatie over deze toegang, zie [Toegang tot sjablonen verlenen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een sjabloon toevoegen</td> 
      <td> <p>Klikken <strong>Nieuwe sjabloon</strong>en configureer de toepassing vervolgens met de beschikbare opties. Voor informatie over deze opties raadpleegt u <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Een projectsjabloon maken</a>.</p> <p>De sjabloon wordt automatisch gekoppeld aan de groep.</p> <p>Voor informatie over hoe groepsvoorkeuren van toepassing zijn op nieuwe sjablonen raadpleegt u <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Hoe voorkeuren van toepassing zijn op sjablonen en sjabloontaken</a> in dit artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen bewerken</td> 
      <td> <p>Selecteer ten minste één sjabloon en klik op het pictogram Bewerken <img src="assets/edit-icon.png">en gebruik vervolgens een van de beschikbare opties om de toepassing te configureren. Voor informatie over deze opties raadpleegt u <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projectsjablonen bewerken</a>.</p> <p>Het pictogram Bewerken is alleen beschikbaar als u toegang hebt tot alle sjablonen die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Toegang tot sjablonen verlenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen verwijderen</td> 
      <td> <p>Selecteer ten minste één sjabloon en klik op het pictogram Verwijderen <img src="assets/delete.png">.</p> <p>Dit pictogram is alleen beschikbaar als u toegang tot alle sjablonen hebt die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Toegang tot sjablonen verlenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen delen</td> 
      <td> <p>Selecteer ten minste één sjabloon en klik op het pictogram Delen <img src="assets/share-icon.png">Klik vervolgens op een van de volgende opties in het vervolgkeuzemenu:</p> 
       <ul> 
        <li> <p><strong>Sjabloon</strong>: In de <strong>Sjabloontoegang</strong> In dit vak voegt u namen toe om aan te geven wie toegang tot de sjabloon wilt hebben.</p> <p>Zie de sectie voor meer informatie <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Een sjabloon delen</a> in het artikel <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Projectsjablonen delen</a>.</p> </li> 
        <li><strong>Project</strong>: In de <strong>Projecttoegang</strong> doos die toont, voeg namen toe om te specificeren wie u toegang tot de projecten wilt hebben die van het malplaatje worden gecreeerd</li> 
       </ul> <p>Het pictogram Delen is alleen beschikbaar als u toegang hebt tot alle sjablonen die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Toegang tot sjablonen verlenen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De lijst met sjablonen exporteren</td> 
      <td>Klikken <strong>Exporteren</strong> <img src="assets/export.png">Selecteer vervolgens de bestandsindeling die u voor de geëxporteerde lijst wilt gebruiken.</td> 
     </tr> 
    </tbody> 
   </table>

## Hoe voorkeuren van toepassing zijn op sjablonen en sjabloontaken {#how-preferences-apply-to-templates-and-template-tasks}

Wanneer u een projectmalplaatje creeert, worden de montages die in de lijsten hieronder worden vermeld gevormd automatisch door een correlerend project of taakvoorkeur.

>[!NOTE]
>
>Of een groep-vlakke of systeem-vlakke project of taakvoorkeur beïnvloedt een projectmalplaatje, afhankelijk van of u het malplaatje met een groep associeerde toen u het creeerde.
>
>Als u deze aan een groep hebt gekoppeld, wordt de voorkeur op groepsniveau van kracht. Dit gebeurt in de volgende scenario&#39;s:
>
>* U maakt de sjabloon vanuit het gebied Groepen, zoals in dit artikel wordt uitgelegd
>* U geeft een groep op wanneer u de sjabloon maakt met een Kickstart-bestand
>* U geeft een groep op wanneer u de sjabloon maakt met de API
>
>Als u het nieuwe malplaatje niet met een groep associeerde, wordt de systeem-vlakke voorkeur van kracht. Dit gebeurt in de onderstaande scenario&#39;s. (Als u later een groep toewijst aan de sjabloon of sjabloontaak, hebben de voorkeuren van de groep geen invloed op de groep.)
>
>* U maakt de sjabloon vanuit het gebied Sjablonen
>* U geeft geen groep op wanneer u de sjabloon maakt met een Kickstart-bestand
>* U geeft geen groep op wanneer u de sjabloon maakt met de API
>


* [Instellingen voor projectsjablonen geconfigureerd door project- en taakvoorkeuren](#project-template-settings-configured-by-project-and-task-preferences)
* [Taakinstellingen voor sjablonen configureren op basis van taakvoorkeuren](#template-task-settings-configured-by-task-preferences)

### Instellingen voor projectsjablonen geconfigureerd door project- en taakvoorkeuren {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prestatiesindexmethode</p> </td> 
   <td> <p>Gevormd door groep-vlakke projectvoorkeur "de Methode van de Index van Prestaties"als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type voorwaarde</p> </td> 
   <td> <p>Gevormd door groep-vlakke projectvoorkeur "plaatst automatisch de Voorwaarde van het project die op de Status van de Voortgang wordt gebaseerd"als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Schema vanuit</p> </td> 
   <td> <p>Gevormd door groep-vlakke projectvoorkeur "Programma van"als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Gebruikerstijd uitgeschakeld</p> </td> 
   <td> <p>Gevormd door groep-vlakke projectvoorkeur "de tijd van de Gebruiker van"als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type bijwerken</p> </td> 
   <td> <p>Gevormd door groep-vlakke projectvoorkeur "de chronologie van het Project zal automatisch opnieuw worden berekend"als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Instellingen voor toegang</p> </td> 
   <td> <p>Gevormd door groep-vlakke taakvoorkeur in de "Toegang"sectie als u het nieuwe malplaatje met een groep associeert, of de zelfde systeem-vlakke projectvoorkeur als u niet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie over de projectvoorkeur die in deze lijst wordt vermeld, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Voor informatie over de taak en uitgiftevoorkeur raadpleegt u [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Als u de groep wijzigt die aan een bestaand projectmalplaatje wordt geassocieerd, blijven de montages van het malplaatje het zelfde.
>* Als u een bestaande sjabloontaak naar een andere sjabloon verplaatst, blijven de volgende instellingen ongewijzigd in de sjabloontaak, ongeacht de groep die aan de nieuwe sjabloon is gekoppeld:>
   >   * Duur
   >   * Type inkomsten
   >   * Kostensoort
>
>  Nochtans, wordt de malplaatjetaak beïnvloed door het plaatsen &quot;wanneer iemand aan een taak&quot;op het nieuwe malplaatje wordt toegewezen. Zie de sectie voor meer informatie [Toegang](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) in het artikel [Projectsjablonen bewerken](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Wanneer een beheerder een project als malplaatje bewaart, worden alle montages voor het malplaatje geërft van het project, met inbegrip van de groep.
>
>  Wanneer een beheerder een taak of een kwestie in een project gebruikend een malplaatje omzet, worden alle montages voor het malplaatje bepaald door wat reeds op het malplaatje wordt bewaard.

### Taakinstellingen voor sjablonen configureren op basis van taakvoorkeuren {#template-task-settings-configured-by-task-preferences}

Wanneer u een malplaatjetaak creeert, worden sommige van zijn montages gevormd automatisch door een correlerende taakvoorkeur. Deze instellingen worden in de onderstaande tabel weergegeven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Duur </p> </td> 
   <td> <p>Gevormd door de groep-vlakke taakvoorkeur "het Type van Duur"als u het malplaatje met een groep, of de zelfde systeem-vlakke taak associeert en voorkeur uitgeeft als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type inkomsten</p> </td> 
   <td> <p>Gevormd door de groep-vlakke taakvoorkeur "Inkomsten Type"als u het malplaatje met een groep associeert, of de zelfde systeem-vlakke taak en geeft voorkeur uit als u niet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Kostensoort </p> </td> 
   <td> <p> Gevormd door de groep-vlakke taakvoorkeur "Kostentype"als u het malplaatje met een groep associeert, of de zelfde systeem-vlakke taak en uitgiftevoorkeur als u niet.</p> </td> 
  </tr> 
 </tbody> 
</table>

Voor informatie over de taakvoorkeuren in deze tabel raadpleegt u [Taak- en probleemvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
