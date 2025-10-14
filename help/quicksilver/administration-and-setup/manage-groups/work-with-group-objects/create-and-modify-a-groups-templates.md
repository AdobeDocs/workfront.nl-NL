---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Creeer en wijzig de Malplaatjes van het Project van een Groep
description: Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met projectmalplaatjes bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '1264'
ht-degree: 0%

---

# De projectsjablonen van een groep maken en wijzigen

Wanneer u een groep bekijkt die u in het gebied van Groepen beheert, kunt u met projectmalplaatjes bekijken en werken verbonden aan de groep en om het even welk van zijn subgroups.

Als er om het even welke groepen boven uw groep zijn, kunnen hun beheerders deze dingen voor uw groep ook doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

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
   <td><p>Nieuw: Standaard</p>
       <p>of</p>
       <p>Huidig: Plan</p></td>
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr>
  <tr> 
   <td role="rowheader">Objectmachtigingen</td>
   <td>Toegang tot of hoger weergeven voor de sjablonen die u wilt weergeven en waarmee u wilt werken</td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sjablonen voor uw groep weergeven, bewerken en maken vanuit het gebied Groepen

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![&#x200B; Groepen &#x200B;](assets/groups-icon.png).

1. Klik op de naam van de groep waarvoor u sjablonen wilt maken of wijzigen.
1. In het linkerpaneel, klik **Malplaatjes** om van de malplaatjes een lijst te maken die met de groep en met om het even welke subgroups worden geassocieerd het zou kunnen hebben.

   U moet toegang tot een sjabloon weergeven als u de sjabloon in deze lijst wilt zien. Voor informatie over deze toegang, zie [&#x200B; toegang van de Verlening tot malplaatjes &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Voer een van de volgende handelingen uit:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Een sjabloon toevoegen</td> 
      <td> <p>Klik <strong> Nieuw Malplaatje </strong>, dan vorm het gebruikend de beschikbare opties. Voor informatie over deze opties, zie <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref"> een projectmalplaatje </a> creëren.</p> <p>De sjabloon wordt automatisch gekoppeld aan de groep.</p> <p>Voor informatie over hoe de groepsvoorkeur op nieuwe malplaatjes van toepassing is, zie <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref"> hoe voorkeur op malplaatjes en malplaatjetaken </a> in dit artikel van toepassing is.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen bewerken</td> 
      <td> <p>Selecteer ten minste één sjabloon, klik op het pictogram Bewerken <img src="assets/edit-icon.png"> en gebruik vervolgens een van de beschikbare opties om de sjabloon te configureren. Voor informatie over deze opties, zie <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref"> projectmalplaatjes </a> uitgeven.</p> <p>Het pictogram Bewerken is alleen beschikbaar als u toegang hebt tot alle sjablonen die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref"> toegang van de Verlening tot malplaatjes </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen verwijderen</td> 
      <td> <p>Selecteer ten minste één sjabloon en klik op het pictogram Verwijderen <img src="assets/delete.png"> .</p> <p>Dit pictogram is alleen beschikbaar als u toegang tot alle sjablonen hebt die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref"> toegang van de Verlening tot malplaatjes </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Een of meer sjablonen delen</td> 
      <td> <p>Selecteer ten minste één sjabloon, klik op het pictogram Delen <img src="assets/share-icon.png"> en klik vervolgens op een van de volgende opties in het vervolgkeuzemenu:</p> 
       <ul> 
        <li> <p><strong> Malplaatje </strong>: In het <strong> vakje van de Toegang van het Malplaatje </strong> dat toont, voeg namen toe om te specificeren wie u toegang tot het malplaatje zelf wilt hebben.</p> <p>Voor meer informatie, zie de sectie <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref"> een malplaatje </a> in het artikel <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref"> het projectmalplaatjes van het Aandeel </a>.</p> </li> 
        <li><strong> Project </strong>: In het <strong> vakje van de Toegang van het Project </strong> dat toont, voeg namen toe om te specificeren wie u toegang tot de projecten wilt hebben die van het malplaatje worden gecreeerd</li> 
       </ul> <p>Het pictogram Delen is alleen beschikbaar als u toegang hebt tot alle sjablonen die u selecteert. Voor informatie over deze toegang, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref"> toegang van de Verlening tot malplaatjes </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">De lijst met sjablonen exporteren</td> 
      <td>Klik <strong> Uitvoer </strong> <img src="assets/export.png">, dan selecteer het dossierformaat u voor de uitgevoerde lijst wilt.</td> 
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

* [&#x200B; het malplaatjemontages van het Project die door project en taakvoorkeur worden gevormd &#x200B;](#project-template-settings-configured-by-project-and-task-preferences)
* [Taakinstellingen voor sjablonen geconfigureerd door taakvoorkeuren](#template-task-settings-configured-by-task-preferences)

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

Voor informatie over de projectvoorkeur die in deze lijst wordt vermeld, zie [&#x200B; systeem-brede projectvoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.

Voor informatie over de taak en de uitgiftevoorkeur, zie [&#x200B; systeembrede taak en uitgiftevoorkeur &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) vormen.

>[!NOTE]
>
>* Als u de groep wijzigt die aan een bestaand projectmalplaatje wordt geassocieerd, blijven de montages van het malplaatje het zelfde.
>* Als u een bestaande sjabloontaak naar een andere sjabloon verplaatst, blijven de volgende instellingen ongewijzigd in de sjabloontaak, ongeacht de groep die aan de nieuwe sjabloon is gekoppeld:>
>   * Duur
>   * Type inkomsten
>   * Kostensoort
>
>  Nochtans, wordt de malplaatjetaak beïnvloed door het plaatsen &quot;wanneer iemand aan een taak&quot;op het nieuwe malplaatje wordt toegewezen. Voor meer informatie, zie de sectie [&#x200B; Toegang &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) in het artikel [&#x200B; projectmalplaatjes &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) uitgeven.
>
>* Wanneer een beheerder een project als malplaatje bewaart, worden alle montages voor het malplaatje geërft van het project, met inbegrip van de groep.
>
>  Wanneer een beheerder een taak of een kwestie in een project gebruikend een malplaatje omzet, worden alle montages voor het malplaatje bepaald door wat reeds op het malplaatje wordt bewaard.
>

### Taakinstellingen voor sjablonen geconfigureerd door taakvoorkeuren {#template-task-settings-configured-by-task-preferences}

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

Voor informatie over de taakvoorkeur die in deze lijst wordt vermeld, zie [&#x200B; de taak van het hele systeem vormen en voorkeur uitgeven &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
