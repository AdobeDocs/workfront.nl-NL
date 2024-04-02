---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Overzicht van firewalls
description: Omdat Adobe Workfront communiceert met het netwerk van uw organisatie, moet de firewall van uw organisatie worden gevormd om die mededeling toe te staan. De firewalls zijn hoogst efficiënte veiligheidsmaatregelen die door het netwerk van een organisatie van Internet te scheiden functioneren. Zij zorgen ervoor dat slechts het geselecteerde gegevens en netwerkverkeer zich in of uit het netwerk van de organisatie kan bewegen. De firewall staat of blokkeert gegevens toe die op de plaats worden gebaseerd die de gegevens verzendt of ontvangt. Als Adobe Workfront-beheerder moet u ervoor zorgen dat gegevens die naar of van Workfront worden verzonden, door de firewall van uw organisatie kunnen worden doorgegeven.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: 405460158b9a540e427b9f9e5de101823838b17b
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Overzicht van firewalls

Omdat Adobe Workfront communiceert met het netwerk van uw organisatie, moet de firewall van uw organisatie worden gevormd om die mededeling toe te staan. De firewalls zijn hoogst efficiënte veiligheidsmaatregelen die door het netwerk van een organisatie van Internet te scheiden functioneren. Zij zorgen ervoor dat slechts het geselecteerde gegevens en netwerkverkeer zich in of uit het netwerk van de organisatie kan bewegen. De firewall staat of blokkeert gegevens toe die op de plaats worden gebaseerd die de gegevens verzendt of ontvangt. Als Adobe Workfront-beheerder moet u ervoor zorgen dat gegevens die naar of van Workfront worden verzonden, door de firewall van uw organisatie kunnen worden doorgegeven.

Dit wordt verwezenlijkt door een lijst van gewenste personen, die hoofdzakelijk een &quot;lijst&quot;van plaatsen is die &quot;toegestaan&quot;zijn om gegevens door de firewall te verzenden of te ontvangen. De plaatsen kunnen op één van twee manieren worden geïdentificeerd:

* **IP-adres**: een reeks getallen zoals 52.31.132.175
* **Domein**: deel van een URL, zoals &quot;this domain&quot; in www.thisdomain.com

Workfront gebruikt specifieke IP-adressen en -domeinen voor webcommunicatie. Deze moeten aan de lijst van gewenste personen van uw organisatie worden toegevoegd alvorens u Workfront in uw organisatie kunt gebruiken.

Over het algemeen, wordt een lijst van gewenste personen gevormd door een netwerkbeheerder. Werk met de netwerkbeheerder van uw organisatie om ervoor te zorgen dat uw firewall deze IP adressen toestaat. Als u niet weet wie uw netwerkbeheerder is, kan de afdeling van IT van uw organisatie u in de juiste richting wijzen.

>[!IMPORTANT]
>
>Als beheerder van Workfront, moet u ervoor zorgen dat deze IP adressen en domeinen aan de lijst van gewenste personen van uw organisatie worden toegevoegd. Dit geldt ook als u ze niet zelf toevoegt. Workfront kan de lijst van gewenste personen van uw organisatie niet configureren.

## Informatie verzamelen voor het configureren van uw firewall

Om uw firewall voor Workfront te vormen, moet uw netwerkbeheerder weten welke IP adressen en domeinen moeten toevoegen. Een deel van deze informatie is alleen beschikbaar voor een Workfront-beheerder. Als beheerder van Workfront, moet u van deze informatie de plaats bepalen en het verstrekken aan uw netwerkbeheerder.

>[!NOTE]
>
>De beste praktijken voor veiligheid moeten slechts de IP adressen en domeinen toevoegen die met functionaliteit verbinden uw organisatie actief gebruikt. Door deze informatie te verstrekken, kunt u ervoor zorgen dat deze beste praktijken wordt gevolgd.

Geef uw netwerkbeheerder de volgende informatie:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Specifieke IP-adressen en -domeinen die zijn toegestaan</td> 
   <td> <p>Het artikel <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">De lijst van gewenste personen van uw firewall configureren</a> bevat de lijst van IP adressen en domeinen die uw organisatie aan zijn lijst van gewenste personen moet toevoegen. </p> <p>Uw netwerkbeheerder heeft mogelijk geen toegang tot het artikel "lijst van gewenste personen van uw firewall configureren". In dat geval moet u het aan hen verstrekken. We raden u niet aan een papieren kopie af te drukken. Met een digitale kopie kan uw netwerkbeheerder de adressen kopiëren en plakken. Dit is sneller en nauwkeuriger dan het typen van een gedrukte kopie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uw cluster</td> 
   <td>Als u de cluster van uw organisatie wilt opzoeken, raadpleegt u <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Het cluster- en Workfront-plan van uw organisatie weergeven</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Je Workfront-abonnement</td> 
   <td> <p>Als u het plan van uw organisatie wilt opzoeken, raadpleegt u <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Bekijk het cluster van uw organisatie en het plan van Workfront.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Uw domein</td> 
   <td> <p>Als u uw domein wilt zoeken, bekijkt u het webadres dat u gebruikt om verbinding te maken met Workfront.</p> <p>Voorbeeld: in het webadres <code>greatcompany.my.workfront.com</code>, het domein is "groot bedrijf"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere Adobe Workfront-producten</td> 
   <td> <p>Stel uw netwerkbeheerder op de hoogte als u licenties hebt voor een van de volgende opties:</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-integratie</td> 
   <td>Stel uw netwerkbeheerder op de hoogte als u een van de volgende methoden gebruikt:
    <ul>
     <li><p>Workfront voor Jira</p></li>
     <li><p>Workfront for G Suite</p></li>
     <li><p>Workfront for Microsoft Teams</p></li>
     <li><p>Workfront for Outlook</p></li>
     <li><p>Workfront voor Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aanvullende functionaliteit</td> 
   <td> <p>Stel uw netwerkbeheerder op de hoogte als u het volgende gebruikt:</p> 
    <ul> 
     <li> <p>Een Workfront-teststation</p> </li> 
    </ul> </td>
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Als u om het even welk van deze producten, integratie, of functionaliteiten op een recentere datum toevoegt, moet u uw netwerkbeheerder contacteren zodat kunnen zij de lijst van gewenste personen aanpassen.

### Het cluster- en Workfront-plan van uw organisatie weergeven {#view-your-organization-s-cluster-and-workfront-plan}

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront of (indien beschikbaar) op de knop **[!UICONTROL Main Menu]** pictogram ![Hoofdmenu](/help/_includes/assets/main-menu-icon-left-nav.png) in de linkerbovenhoek klikt u op **[!UICONTROL Setup]** ![Pictogram Instellen](/help/_includes/assets/gear-icon-setup.png).

1. Klikken **Systeem** in het linkerdeelvenster
1. Selecteer **Klantgegevens**.

   Uw cluster wordt in de rechterbovenhoek van het dialoogvenster weergegeven **Basisinformatie** sectie.

   ![](assets/locate-cluster.png)

1. Als u uw Workfront-abonnement wilt bekijken, selecteert u **Licenties**.

   Uw abonnement wordt onder aan de pagina weergegeven.

   ![](assets/locate-plan.png)
