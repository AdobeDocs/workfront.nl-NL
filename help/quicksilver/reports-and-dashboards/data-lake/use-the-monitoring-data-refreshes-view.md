---
product-area: reports and dashboards
navigation-topic: data-connect
title: De weergave Gegevensvernieuwingen controleren in Data Connect gebruiken
description: Met Data Connect kunnen Workfront-beheerders toegang krijgen tot gedetailleerde records van de recente updates die tijdens de meest recente vernieuwingen zijn aangebracht op de datum van het datumpigment.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# De weergave Gegevensvernieuwingen controleren in Data Connect gebruiken

De mening van de Verfrissingen van Gegevens van de Controle toont de recente updates die aan de datum van het gegevensmeer tijdens meest recente verfrissen werden gemaakt. De gegevens van deze weergave worden bijgewerkt nadat de gegevens zijn geladen.

Vanwege het grote gegevensvolume en de complexiteit van de aggregaties worden in de weergave Gegevens controleren alleen de objectweergaven weergegeven die in de afgelopen twee weken zijn bijgewerkt. Als een specifiek recordtype niet aanwezig is in deze weergave, is dit mogelijk te wijten aan een gebrek aan activiteit binnen die tijdsperiode.

>[!NOTE]
>
>Deze mening toont een gedetailleerde inzameling van de gegevens die door de toepassing worden verstrekt en verfrist activiteiten in tegenstelling tot een dagelijkse geschiedenis of gebeurtenismening die toont verfrist activiteitengeschiedenis. Om historische verfrissingsactiviteitendetails te verkrijgen, kunt u <code> gebruiken DL_LOAD_TIMESTAMP</code> datumobject.

## Weergavekolommen voor gegevensvernieuwingen controleren

De weergavekolommen voor het vernieuwen van monitoringgegevens bevatten de volgende informatie:

<table>
    <tr>
        <td><b>Kolomnaam</b></td>
        <td><b>Type</b></td>
        <td><b>Beschrijving</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      Het objecttype dat is gekoppeld aan de Workfront-records die naar het datumpeer zijn verzonden. 
        </ul></td>
    </tr>
    <tr>
        <td>CALENDAR_DATE </td>
        <td>Datum</td>
        <td>
   De datum van de laatste succesvolle gegevens verfrissen zich voor het objecten type dat in de kolom OBJ_TYPE wordt getoond. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ</td>
        <td>
 De datum en de tijd van de meest recente gegevens verfrissen zich voor het objecten type dat in de kolom OBJ_TYPE wordt getoond.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Timestamp_NTZ </td>
        <td>
       De datum en de tijd van de tweede meest recente gegevens verfrissen zich voor het objecten type dat in de kolom OBJ_TYPE wordt getoond. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Getal</td>
        <td>
     De hoeveelheid tijd in minuten die is verstreken sinds de laatste gegevens voor het objecttype zijn vernieuwd. </td>
    </tr>
            <tr>
        <td>GEMAAKT </td>
        <td>Getal </td>
        <td>Een telling van CREATE verslaggebeurtenissen die tussen vorige en recentste gegevensvernieuwingen voor het objecten type worden gevangen.  </td>
    </tr>
                <tr>
        <td>BIJGEWERKT</td>
        <td>Getal </td>
        <td>Een telling van de UPDATE-recordgebeurtenissen die zijn vastgelegd tussen de vorige en laatste gegevensvernieuwingen voor het objecttype.</td>
    </tr>
                <tr>
        <td>VERWIJDERD</td>
        <td>Getal </td>
        <td>Een telling van de DELETE-recordgebeurtenissen die zijn vastgelegd tussen de vorige en laatste gegevensvernieuwingen voor het objecttype. </td>
    </tr>
                <tr>
        <td>TOTAAL</td>
        <td>Getal </td>
        <td>Een telling van het totale aantal gebeurtenissen tussen het vorige en recentste gegevensvernieuwingen voor het objecttype. 
        <br> 
        <br><b> Nota </b>: Dit is niet het zelfde als het totale aantal verslagen die door CREATE, UPDATE, of de gebeurtenissen van DELETE worden beïnvloed aangezien het zelfde verslag kon worden gecreeerd en worden bijgewerkt veelvoudige tijden binnen het interval tussen vernieuwingen.  </td>
    </tr>
   </table>

