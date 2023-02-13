---
product-area: resource-management
navigation-topic: resource-scheduling
title: Automatisch niet-toegewezen taken en problemen toewijzen in de planningsgebieden
description: Wanneer u de planningsprogramma's gebruikt, kunt u Adobe Workfront toestaan om de huidige werktoewijzingen voor alle beschikbare gebruikers te analyseren en intelligente, logische toewijzingen voor te stellen voor alle taken of problemen die nog niet zijn toegewezen. U kunt voorgestelde toewijzingen wijzigen voordat u ze voltooit.
author: Alina
feature: Resource Management
exl-id: 087fe3ef-9b85-491b-9fdc-436a01822ede
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 0%

---

# Automatisch niet-toegewezen taken en problemen toewijzen in de planningsgebieden

>[!IMPORTANT]
>  
><span class="preview">De planningsfunctionaliteit die in dit artikel wordt beschreven, is vanaf de release 23.1 in januari 2023 vervangen en uit Adobe Workfront verwijderd.   </span>
>  
> <span class="preview"> Dit artikel wordt ook verwijderd kort na de release van 23.1, begin 2023. Op dit moment raden we u aan eventuele bladwijzers dienovereenkomstig bij te werken. </span>
> 
><span class="preview"> U kunt de werklastbalans nu gebruiken om werk voor uw bronnen te plannen. </span>
>  
> <span class="preview">Voor informatie over het plannen van middelen die de Balancer van de Werkbelasting gebruiken, zie de sectie [De werklastbalans](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!-- 

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 
-->

Wanneer u de planningsprogramma&#39;s gebruikt, kunt u Adobe Workfront toestaan om de huidige werktoewijzingen voor alle beschikbare gebruikers te analyseren en intelligente, logische toewijzingen voor te stellen voor alle taken of problemen die nog niet zijn toegewezen. U kunt voorgestelde toewijzingen wijzigen voordat u ze voltooit.

Workfront bekijkt de taken en kwesties beschikbaar in het Niet toegewezen gebied binnen de momenteel geselecteerde datumwaaier en stelt taken voor elk punt in één keer voor. U kunt een filter maken om het aantal items te beperken dat beschikbaar is in het gebied Niet toegewezen.

Uw systeembeheerder bepaalt hoe Workfront middelbeschikbaarheid op het systeemniveau berekent (het overwegen van uren evenals beschikbaarheid FTE). Afhankelijk van dit systeem-brede plaatsen, wordt de middelbeschikbaarheid berekend of gebruikend het standaardprogramma of het programma van de gebruiker. Zie voor meer informatie [Vorm hoe Workfront middeluur en FTE beschikbaarheid voor het Plannende gebied berekent](../../resource-mgmt/resource-scheduling/calculate-hours-fte-scheduling-area.md).

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
   <td> <p>Werk of hoger</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Toegangsniveau*</td> 
   <td> <p>De mening of hogere toegang tot Projecten, Taken, en Kwesties</p> <p><strong>OPMERKING</strong>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Contribute-machtigingen of hoger voor de projecten, taken en uitgaven waarvoor u toewijzingen bijwerkt</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Vereisten {#prerequisites}

Workfront gebruikt een eigen algoritme om toewijzingsvoorstellen te bepalen. Om de beste resultaten te bereiken, moet u ervoor zorgen dat de volgende informatie in Workfront correct is:

* Taak- en informatieverstrekking, waaronder:

   * Roltoewijzingen\
      Er wordt geen voorstel gedaan voor taken en kwesties die niet aan een rol worden toegewezen.
   * Geplande uren\
      Als een taak of kwestie momenteel geen geplande uren heeft, neemt Workfront 4 geplande uren per werkdag over wanneer automatisch het toewijzen van werk. Deze uren worden niet automatisch toegewezen aan het werkitem; zij worden alleen gebruikt om een realistischere taakverdeling te waarborgen .
   * Geplande begindatums en geplande einddatums

* Gebruikersgegevens, waaronder:

   * Primaire en secundaire roltoewijzingen op het gebruikersprofiel
   * Projectteamgegevens

## Rollimieten configureren

Rollimieten bepalen het aantal gebruikers met een specifieke rol dat automatisch werk kan worden toegewezen. Rollimieten werken per project om ervoor te zorgen dat op rollen gebaseerde taken niet worden verspreid onder een groot aantal gebruikers.

De volgende scenario&#39;s schetsen hoe rolgrenzen op projecten van toepassing zijn:

* **Scenario 1**: Als er geen gebruikers aan het projectteam worden toegewezen, gebruikt het systeem de rolgrens om taken toe te wijzen.\
   Bijvoorbeeld, hebt u een project zonder gebruikers die aan het projectteam worden toegewezen. Dit project heeft 10 projectbeheertaken die moeten worden toegewezen, en u hebt een rolgrens van 1 voor de rol van de Manager van het Project geplaatst. Het systeem wijst alle 10 taken aan 1 projectmanager toe omdat de rolgrens aan 1 wordt geplaatst.

* **Scenario 2**: Als de rolgrens groter is dan het aantal gebruikers die aan het projectteam worden toegewezen, worden de extra gebruikers toegewezen taken.\
   Bijvoorbeeld, hebt u een project met één schrijver die aan het projectteam wordt toegewezen. Dit project heeft 12 schrijvertaken die moeten worden toegewezen, en u hebt een rolgrens van 2 die voor de rol van de Schrijver wordt geplaatst. Het systeem wijst alle 12 taken tussen de schrijver van het projectteam en een extra schrijver toe omdat de rolgrens aan 2 wordt geplaatst.

* **Scenario 3**: Als de rolgrens minder dan het aantal gebruikers is die aan het projectteam wordt toegewezen, wordt de rolgrens met voeten getreden.\
   Bijvoorbeeld, hebt u een project met 4 die ontwerpers aan het projectteam worden toegewezen. Dit project heeft 8 ontwerpertaken die moeten worden toegewezen, en u hebt een rolgrens van 2 voor de rol van de Ontwerper geplaatst. Het systeem wijst alle 8 taken tussen elk van de 4 ontwerpers van het projectteam toe alhoewel de rolgrens aan 2 wordt geplaatst.

Limieten instellen voor taakrolltoewijzingen:

1. Ga naar de het plannen chronologie voor veelvoudige projecten of voor een individueel project:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.

1. Klik op de knop **Instellingen** pictogram.\
   ![Automode_settings.png](assets/automode-settings.png)

1. In de Geautomatiseerde sectie van de Planning van het Middel, klik in **Limiet** kolom inline met het item in het dialoogvenster **Rol** en voert u een positief getal in.\
   Workfront slaat uw wijzigingen automatisch op.

   >[!NOTE]
   >
   >Alle huidige leden van het projectteam zijn automatisch geschikt voor al geadviseerd werk ongeacht de ingestelde rolgrens.

   ![set_Role_Limits.png](assets/set-role-limits-350x341.png)

1. (Optioneel) Klik op de knop **Weergeven** boven aan de kolom Limiet en selecteer de gewenste weergaveopties.
1. Om terug naar het middel het plannen gebied te gaan, klik **Terugkeren naar planning**.

## Taken en problemen automatisch toewijzen

U kunt taken en kwesties aan gebruikers op de het plannen chronologie toewijzen of u op het Plannende lusje (wanneer het plannen van middelen voor veelvoudige projecten) of het Stafsende lusje (wanneer het plannen van middelen voor een individueel project) bent.

Workfront toestaan om automatisch toewijzingen voor taken en problemen in het niet-toegewezen gebied voor te stellen:

1. Ga naar de het plannen chronologie voor veelvoudige projecten of voor een individueel project:

   * **Voor meerdere projecten**: Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Workfront klikt u op **Bronnen > Werklastverdeling** selecteert u vervolgens **Planning** in het drop-down menu linksboven.
   * **Voor een afzonderlijk project**: Ga naar een project, klik **Werklastverdeling** in het linkerdeelvenster en selecteer vervolgens **Planning** in het keuzemenu linksboven.

1. (Optioneel) Maak een filter om aan te passen welke inhoud wordt weergegeven in het gedeelte Niet toegewezen op de tijdlijn van de planning.\
   Zie voor meer informatie over het maken van een filter [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md#creating-and-modifying-filters-on-the-scheduling-tab-for-projects) in [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md) [Gegevens filteren in het planningsgebied](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md)

   >[!TIP]
   >
   >Om ervoor te zorgen dat Workfront werk toewijst aan de meest in aanmerking komende gebruikers:
   >
   >* Filter slechts informatie die beïnvloedt welke taken in Unassigned gebied (zoals Portfolio, Programma&#39;s, en Projecten) worden getoond.
   >* We raden u aan geen informatie te filteren die invloed heeft op welke gebruikers beschikbaar zijn om toe te wijzen op de tijdlijn die gepland is. Hierdoor kan Workfront niet alle mogelijke toewijzingen bekijken, wat tot minder bevredigende toewijzingen kan leiden.


1. (Optioneel) Wijzig het datumbereik dat wordt weergegeven op de tijdlijn van de planning, zoals beschreven in [Het datumbereik van de planningsgebieden aanpassen](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#adjusting-the-date-range-for-which-data-is-displayed) in [Aan de slag met Resource Scheduling](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md). Workfront maakt toewijzingen alleen voor taken en problemen binnen het zichtbare datumbereik op de tijdlijn van de planning.

1. Klik op de knop **Automatisch** in de rechterbovenhoek van de tijdlijn van de planning.\
   ![plannen_auto.png](assets/scheduling-auto-350x221.png)\
   Workfront stelt taken voor elke taak of elk onderwerp in het **Niet toegewezen** gebied.

   >[!TIP]
   >
   >Taken en kwesties moeten reeds aan een rol worden toegewezen om een opdracht te kunnen voorstellen. Om de beste resultaten te bereiken, moeten de taken en kwesties de in [Vereisten](#prerequisites).

   De voorgestelde toewijzingen worden als volgt gedifferentieerd met een gestippelde omtrek rond elke taak of uitgave:\
   **Voorgestelde taaktoewijzing:**

   **Bestaande taaktoewijzing:**

1. (Optioneel) U kunt voorgestelde of bestaande toewijzingen wijzigen voordat u de taken voltooit:

   >[!NOTE]
   >
   >Als u een bestaande toewijzing wijzigt, verandert deze in een voorgestelde status.

   * Een item toewijzen aan een andere gebruiker:

      * Sleep de taak of de kwestie van de voorgestelde gebruiker aan de rij van een verschillende gebruiker u wilt toewijzen.

         <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE: lists in this article need to be reformatted and maybe split - too many levels in)      
        </MadCap:conditionalText>      
        -->

         Een maximum van 10 taken per dag wordt getoond voor een bepaalde gebruiker. U kunt de lijst uitvouwen om alle taken weer te geven die momenteel aan die gebruiker zijn toegewezen. (Na het uitvoeren van taken op de planningstijdlijn, zouden meer dan 10 taken tijdelijk kunnen worden getoond.)\
         Terwijl u een item sleept, wordt de volgende informatie weergegeven voordat u de taak of uitgave loslaat en de toewijzing voltooit:

         * Er wordt een neerzetindicator weergegeven in de rij van de gebruiker. Hierdoor kunt u zien waar een item wordt toegewezen voordat u de toewijzing maakt.
         * Als gebruikerstoewijzingen zijn ingeschakeld op de tijdlijn van de planning, worden de rode overtoewijzingsindicatoren weergegeven als het voltooien van de toewijzing ertoe zal leiden dat de gebruiker wordt oververdeeld.\
            Zie voor meer informatie over overtoewijzingsindicatoren [Toewijzingsindicatoren](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md#understanding-allocation-indicators).

         * Gebruikers die niet in aanmerking komen om de toewijzing te ontvangen, worden grijs weergegeven.
      * Vouw de taak of uitgave die u wilt toewijzen uit, klik op de vervolgkeuzepijl in het dialoogvenster **Toewijzingen** typt u eerst de naam van de gebruiker die u wilt toewijzen en vervolgens klikt u op de naam van de gebruiker in de vervolgkeuzelijst.\
         ![programma_taak_uitgevouwen.png](assets/schedule-task-expanded-350x170.png)
   * Als u een toewijzing wilt uitstellen, sleept u een taak of uitgave die u nog niet kunt toewijzen aan de **Niet toegewezen** gebied.



1. Klik op de knop **Toewijzingen maken** boven aan de tijdlijn van de planning om eventuele voorgestelde toewijzingen te voltooien.\
   of\
   Klikken **Annuleren** alle voorgestelde opdrachten terug te brengen naar hun vroegere functie.
