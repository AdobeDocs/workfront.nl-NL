---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Foutbericht: ongeldige parameter: conversiewaarde"
description: '"U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld op een bestaand aangepast formulier te wijzigen: ''Ongeldige parameter: conversiewaarde ''&lt;..&gt;'''''
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Foutbericht: Ongeldige parameter: conversiewaarde

## Probleem

U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld te wijzigen op een bestaand aangepast formulier: &quot;Ongeldige parameter: conversiewaarde &quot;&lt;...>&quot;&quot;\
![ custom_field_format_invalid_parameter_error.png ](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Oorzaak

Dit bericht komt in het volgende scenario voor:

U hebt bijvoorbeeld een aangepast veld dat als tekst is opgemaakt.  Nu wilt u de indeling van het aangepaste veld wijzigen in Valuta. ergens in uw Adobe Workfront-instantie is dit veld al gekoppeld aan een object en bevat het al opgegeven informatie. De bestaande informatie in ten minste één dergelijk veld is al opgemaakt als tekst. Daarom kan de opmaak van het veld niet worden gewijzigd in Valuta.

## Toegangsvereisten

+++ Breid uit om de toegangseisen voor de functionaliteit in dit artikel weer te geven.

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licentie</td> 
   <td>
   <p>Nieuw: Standaard</p>
   <p>of</p>
   <p>Huidig: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul>
  </tr> 
 </tbody> 
</table>

Voor meer detail over de informatie in deze lijst, zie [ vereisten van de Toegang in de documentatie van Workfront ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Oplossing

Ga als volgt te werk:

1. Stel rapporten samen voor alle objecten waaraan dit veld is gekoppeld met hun aangepaste Forms.\
   Voor informatie over de bouw van een rapport, zie [ een douanerapport ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) creëren.

1. Neem het aangepaste veld dat u wilt bewerken op in de weergave van het rapport, zodat u kunt zien welk object dit veld bevat dat is gevuld met een tekstwaarde.
1. Corrigeer de aangepaste veldwaarden van de objecten die in een tekstindeling worden weergegeven en geef deze de waarde Valuta en probeer vervolgens het veld Opmaak opnieuw te wijzigen in het aangepaste formulier.\
   of\
   Als u te veel veldwaarden hebt die al zijn gevuld met informatie met tekstopmaak, kunt u overwegen een nieuw aangepast veld toe te voegen aan uw aangepaste formulier en dit op te maken als Valuta.
