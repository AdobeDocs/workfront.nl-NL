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
source-wordcount: '472'
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
   <td> <p>Toegang tot projecten en financiële gegevens bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Machtigingen voor het project beheren met beheerdersmachtigingen</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Overwegingen bij PIM in Workfront

* Uw beheerder van Workfront of een groepsbeheerder plaatst - omhoog het gebrek voor of de Methode van de Index van Prestaties (PIM) op uur-gebaseerd of op kosten-gebaseerd zou moeten zijn. De berekeningen voor de prestatiemetriek veranderen volgens hoe dit gebrek wordt geplaatst. Voor meer informatie over hoe te om het gebrek voor te veranderen hoe te om PIM te berekenen, zie [Projectvoorkeuren voor het hele systeem configureren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Projectmanagers kunnen ook de instelling voor de PIM wijzigen, op projectniveau, voor afzonderlijke projecten in het subtabblad Financiën van het project. U moet beheerdersmachtigingen voor het project hebben om het subtabblad Financiën van het project te kunnen bewerken.

## Plaats de Methode van de Index van Prestaties (PIM) voor een project

1. Ga naar een project waarvan u de eigenaar bent.

   >[!IMPORTANT]
   >
   >U hebt beheermachtigingen voor het project nodig om de volgende stappen uit te voeren. We raden ook aan dat alleen de eigenaar van het project wijzigingen aanbrengt in het gebied Financiën van het project.

1. Klikken **Projectdetails** in het linkerpaneel, dan ga naar **Financiën** gebied.
1. Dubbelklik op de waarde in het dialoogvenster **Prestatiesindexmethode** te bewerken.
1. Selecteer een van de volgende opties in het dialoogvenster **Prestatiesindexmethode** veld:

   | Op uurbasis | Workfront gebruikt de geplande uren voor de berekening van de CPI en de EAC van het project en de EAC van het project wordt weergegeven als een aantal, in uren. |
   |---|---|
   | Op basis van kosten | Workfront gebruikt de geplande loonkosten voor de berekening van de CPI en de EAC van het project, en de EAC wordt weergegeven als een valutawaarde. Wanneer u deze optie selecteert, moet u ervoor zorgen dat uw taaktoewijzingen (taakrollen of gebruikers) aan kostentarieven zijn gekoppeld. |

   {style=&quot;table-layout:auto&quot;}

1. Klikken **Opslaan** **Wijzigingen**.
