---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: ongeldige parameter: conversiewaarde'
description: 'U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld op een bestaand aangepast formulier te wijzigen: ''Ongeldige parameter: conversiewaarde &grave;&lt;..&gt;'''''
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '311'
ht-degree: 0%

---

# Foutbericht: Ongeldige parameter: conversiewaarde

## Probleem

U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld te wijzigen op een bestaand aangepast formulier: &quot;Ongeldige parameter: conversiewaarde &quot;&lt;...>&quot;&quot;\
![&#x200B; custom_field_format_invalid_parameter_error.png &#x200B;](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Oorzaak

Dit bericht komt in het volgende scenario voor:

U hebt bijvoorbeeld een aangepast veld dat als tekst is opgemaakt.  Nu wilt u de indeling van het aangepaste veld wijzigen in Valuta. ergens in uw Adobe Workfront-instantie is dit veld al gekoppeld aan een object en bevat het al opgegeven informatie. De bestaande informatie in ten minste één dergelijk veld is al opgemaakt als tekst. Daarom kan de opmaak van het veld niet worden gewijzigd in Valuta.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Alle</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licentie</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Configuraties op toegangsniveau</td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Voor informatie, zie [&#x200B; vereisten van de Toegang in de documentatie van Workfront &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

Ga als volgt te werk:

1. Stel rapporten samen voor alle objecten waaraan dit veld is gekoppeld met hun aangepaste Forms.\
   Voor informatie over de bouw van een rapport, zie [&#x200B; een douanerapport &#x200B;](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Neem het aangepaste veld dat u wilt bewerken op in de weergave van het rapport, zodat u kunt zien welk object dit veld bevat dat is gevuld met een tekstwaarde.
1. Corrigeer de aangepaste veldwaarden van de objecten die in een tekstindeling worden weergegeven en geef deze de waarde Valuta en probeer vervolgens het veld Opmaak opnieuw te wijzigen in het aangepaste formulier.\
   of\
   Als u te veel veldwaarden hebt die al zijn gevuld met informatie met tekstopmaak, kunt u overwegen een nieuw aangepast veld toe te voegen aan uw aangepaste formulier en dit op te maken als Valuta.
