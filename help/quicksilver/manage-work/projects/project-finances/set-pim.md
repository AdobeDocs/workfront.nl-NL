---
product-area: projects
navigation-topic: financials
title: De PIM-methode (Performance Index) instellen
description: De Methode van de Index van Prestaties (PIM) voor het project controleert de methode Adobe Workfront gebruikt om de metriek van projectprestaties zoals de Index van de Prestaties van de Kosten (CPI), de Index van de Prestaties van het Programma van het Programma (CSI), en Schatting bij Voltooiing (EAC) te berekenen.
author: Alina
feature: Work Management
exl-id: de628881-c016-4521-bc33-3bcfba19a88f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# De PIM-methode (Performance Index) instellen

De Methode van de Index van Prestaties (PIM) voor het project controleert de methode Adobe Workfront gebruikt om de metriek van projectprestaties zoals de Index van de Prestaties van de Kosten (CPI), de Index van de Prestaties van het Programma van het Programma (CSI), en Schatting bij Voltooiing (EAC) te berekenen.

Workfront berekent deze waarden met behulp van het volgende:

* Uren
* Kosten

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor het project beheren met beheerdersmachtigingen</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Overwegingen bij PIM in Workfront

* Uw beheerder van Workfront of een groepsbeheerder plaatst - omhoog het gebrek voor of de Methode van de Index van Prestaties (PIM) op uur-gebaseerd of op kosten-gebaseerd zou moeten zijn. De berekeningen voor de prestatiemetriek veranderen volgens hoe dit gebrek wordt geplaatst. Voor meer informatie over hoe te om het gebrek voor te veranderen hoe te om PIM te berekenen, zie [ systeem-brede projectvoorkeur ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) vormen.
* Projectmanagers kunnen ook de instelling voor de PIM wijzigen, op projectniveau, voor afzonderlijke projecten in het subtabblad Financiën van het project. U moet beheerdersmachtigingen voor het project hebben om het subtabblad Financiën van het project te kunnen bewerken.

## De PIM-methode (Performance Index) voor een project instellen

1. Ga naar een project waarvan u de eigenaar bent.

   >[!IMPORTANT]
   >
   >U hebt beheermachtigingen voor het project nodig om de volgende stappen uit te voeren. We raden ook aan dat alleen de eigenaar van het project wijzigingen aanbrengt in het gebied Financiën van het project.

1. Klik **Details van het Project** in het linkerpaneel, dan ga naar het **Financiën** gebied.
1. Dubbelklik de waarde op het **gebied van de Methode van de Index van Prestaties** om het uit te geven.
1. Selecteer van de volgende opties op het **gebied van de Methode van de Index van Prestaties 0}:**

   | Op uurbasis | Workfront gebruikt de geplande uren voor de berekening van de CPI en de EAC van het project en de EAC van het project wordt weergegeven als een aantal, in uren. |
   |---|---|
   | Op basis van kosten | Workfront gebruikt de geplande loonkosten voor de berekening van de CPI en de EAC van het project, en de EAC wordt weergegeven als een valutawaarde. Wanneer u deze optie selecteert, moet u ervoor zorgen dat uw taaktoewijzingen (taakrollen of gebruikers) aan kostentarieven zijn gekoppeld. |

   {style="table-layout:auto"}

1. Klik **sparen** **Veranderingen**.
