---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Een aangepaste status als standaardstatus voor een groep gebruiken
description: Als groepsbeheerder, kunt u een douanestatus als standaardstatus voor een groep of subgroep vormen die u beheert.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: fb555df123701c62e9a0f2d451ad6dcd16586595
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 0%

---

# Een aangepaste status als standaardstatus voor een groep gebruiken

Als groepsbeheerder, kunt u een douanestatus als standaardstatus voor een groep of subgroep vormen die u beheert. Dit is handig wanneer het systeem automatisch een Workfront-status moet toewijzen aan een project, taak of uitgave. In een project, taak of uitgave wordt altijd de aangepaste status weergegeven die u als standaardstatus instelt in plaats van de Workfront-status die deze status heeft.

De status u vormt kan om het even welke douanestatus zijn die voor de groep wordt gecreeerd, van een groep boven de groep wordt geërft, of van het systeemniveau wordt geërft.

Als er groepen zijn boven de groep die u beheert, kunnen hun beheerders dit ook voor uw groep doen. Hetzelfde geldt voor Workfront-beheerders (voor elke groep).

>[!INFO]
>
>**Voorbeeld:** u kon een douanestatus tot stand brengen genoemd Voltooid en het plaatsen als standaardstatus die met de voltooide status van Workfront wordt gelijkgesteld.
>
>Voor taken die zijn ingesteld op wijzigen in de status Voltooid wanneer ze 100% bereiken, wordt de status weergegeven als Voltooid in plaats van Voltooid.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-pakket</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Adobe Workfront-licentie</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td>U moet een groepsbeheerder van de groep of een systeembeheerder zijn.</td>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Uitgiftestatus

Als de aangepaste status de status Uitgave is, moeten alle vier de uitgiftetypen hiervoor zijn ingeschakeld (Foutenrapport, Wijzigingsvolgorde, Uitgave en Verzoek). In de onderstaande status van de uitgave kan de status Opnieuw geopend bijvoorbeeld niet als standaardstatus worden gebruikt omdat het type Uitgave volgorde wijzigen niet is geselecteerd:

![&#x200B; Alle toegelaten uitgiftetypen &#x200B;](assets/all-4-issue-types-enabled.png)

## Een aangepaste status instellen als standaardstatus voor een groep

{{step-1-to-setup}}

1. In het linkerpaneel, klik **Groepen** ![&#x200B; Groepen &#x200B;](assets/groups-icon.png), dan klik de naam van de groep waar u statussen creëren of wilt aanpassen.
1. In het linkerpaneel, klik **Statussen** ![&#x200B; het montagespictogram van het Gear &#x200B;](assets/gear-icon-settings.png).
1. Open het **Project**, **Taken**, of **Kwesties** lusje, afhankelijk van het type van status u als standaardstatus wilt plaatsen.
1. Klik **Vastgestelde StandaardStatussen** dichtbij de hoger-juiste hoek.
1. Selecteer in het vervolgkeuzemenu dat wordt weergegeven, naast de status waar u de standaardstatus wilt instellen, de standaardstatus die u wilt instellen.
1. Klik **sparen**.

   De status is nu beschikbaar als standaardstatus voor gebruik met projecten die aan de groep zijn gekoppeld.

1. Koppel de aangepaste status aan het project waar u deze wilt gebruiken.

   U associeert de status met het project door de groep te associëren waar de status met het project verblijft. De gebruikers kunnen de douanestatus slechts gebruiken als de groep waar de status verblijft met het project wordt geassocieerd.

   >[!NOTE]
   >
   >Als u het project aan een verschillende groep toewijst, zal de projectstatus opnieuw laden en kon veranderen.

   1. Ga naar het project waar u de douanestatus wilt gebruiken.
   1. Klik het Meer menu ![&#x200B; Meer pictogram &#x200B;](assets/more-icon.png), dan klik **uitgeven**.
   1. In **geef de doos van het Project** uit die, op het **3&rbrace; gebied van de Groep &lbrace;onder** de vereniging van het Project **toont, de groep selecteren die de douanestatus met wordt geassocieerd.**

   1. Klik **sparen Veranderingen**.

## Groepen nemen standaardstatusconfiguraties over

Nadat een beheerder van Workfront een douanestatus als standaardstatus vormt, erven de nieuwe groepen die worden gecreeerd die configuratie.

Op dezelfde manier nadat een groepsbeheerder een douanestatus als standaardstatus plaatst, erven de nieuwe die subgroepen direct onder de groep worden gecreeerd die configuratie.

Voor meer informatie, zie [&#x200B; Hoe de groepen statussen &#x200B;](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md) erven.

## Wanneer een standaardstatus verborgen is

Als u een standaardstatus verbergt (door de statusoptie Verbergen hiervoor in te schakelen), probeert het systeem een andere status van het equivalente type als de standaardstatus in te stellen.

Als er geen beschikbare status van het gelijkwaardige type is, toont het statustype als **Verborgen** en is niet beschikbaar voor het werkpunten.

![&#x200B; Geen beschikbare status &#x200B;](assets/when-hide-default-status-no-equivalent.png)
