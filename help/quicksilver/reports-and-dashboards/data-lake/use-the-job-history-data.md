---
product-area: reports and dashboards
navigation-topic: data-connect
title: De weergave Taakhistorie gebruiken in Data Connect
description: Met Data Connect kunnen Workfront-beheerders toegang krijgen tot gedetailleerde records van elke vernieuwingstaak voor gegevens in de weergave Taakgeschiedenis.
author: Jenny
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
source-git-commit: 79e8b2b1dd3b7374173c2a930abdf8a0bca2cda6
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# De weergave Taakhistorie gebruiken in Data Connect

In de weergave Taakgeschiedenis hebben Workfront-beheerders toegang tot gedetailleerde records van elke gegevensupdate. Deze records bieden waardevolle insight in de taken die uw gegevens up-to-date houden en helpen u ideale tijdsbestekken te maken voor het uitvoeren van processen en het vernieuwen van uw zakelijke visualisaties.

![ de mening van de Geschiedenis van de Baan ](assets/job-history-tab.png)

De de meningskolommen van de Geschiedenis van de Baan bevatten de volgende informatie:

* **OBJECT_NAME**: Toont de naam van het voorwerp verbonden aan de baan.
* **SCHEDULED_TIME**: Toont de begintijd van de baan.
* **COMPLETED_TIME**: Toont de de voltooiingstijd van de baan.
* **LATEST_FLAG**: Wijst op als de baan deel van meest recente verfrist zich.
* **STAAT**: Toont de status van de baan. Voor meer, zie de volgende sectie in dit artikel: [ Beschikbare baanstatussen ](#available-job-statuses).
* **LAST_UPDATED**: De laatste bijgewerkte timestamp van de baan.

>[!NOTE]
>
>De weergave Taakgeschiedenis bevat gegevens over de vorige 72 uur van geplande taken.


## Beschikbare taakstatussen

Aan elke Data Connect-taak wordt een status toegewezen die aangeeft of deze is gelukt, overgeslagen of mislukt.

<table>
    <tr>
        <td><b>Taakstatus</b></td>
        <td><b>Definitie</b></td>
    </tr>
    <tr>
        <td>Geslaagd</td>
        <td>De baan verwerkte met succes elke beschikbare update, en alle updates voor dat verslagtype worden nu weerspiegeld in het gegevensmeer.</td>
    </tr>
    <tr>
        <td>Overgeslagen</td>
        <td>De taak is overgeslagen omdat er geen updates in de wachtrij stonden die voor het recordtype moesten worden verwerkt.</td>
    </tr>
    <tr>
        <td>Mislukt</td>
        <td>De taak kan niet worden uitgevoerd. In deze gevallen, is het waarschijnlijk dat geen gegevens in rij aan het gegevens meer werden begaan. De verslagen die in rij blijven zullen in de volgende geplande baan voor dat verslagtype worden verwerkt. </td>
    </tr>
   </table>


## Overwegingen bij het uitvoeren van taken en het registreren van gedrag

Snowflake gebruikt een hulpprogramma voor het optimaliseren van taakplanners dat van invloed kan zijn op de manier waarop het uitvoeren van taken wordt verwerkt en wordt aangemeld in de weergave Taakgeschiedenis. Dit registrerengedrag kan variëren afhankelijk van of er gegevens zijn om te verwerken.

Wanneer er bijvoorbeeld geen nieuwe rijen zijn die voor een bepaald object moeten worden verwerkt, kan een van de volgende resultaten optreden:

* **de Baan voert uit en is duidelijk als Overgeslagen**: Snowflake ontdekt dat er geen rijen zijn om te verwerken, voert de baan uit, en registreert het met een Overgeslagen status in de lijst.

* **de Baan voert niet uit**: Snowflake bepaalt er geen rijen om te verwerken zijn, voert niet de baan uit, en registreert het met een Overgeslagen status in de lijst.

  >[!NOTE]
  >
  >In het tweede scenario waarin de taak niet wordt uitgevoerd, kan de meest recente record voor dat object een tijdstempel weerspiegelen die niet overeenkomt met het verwachte schema.

Met andere woorden, een baan kan als uitgevoerd worden beschouwd zelfs als geen rijen werden verwerkt, en het kan of niet worden geregistreerd afhankelijk van het gedrag van de baanplanner voor die bepaalde baan.