---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Foutbericht: Ongeldige parameter: conversiewaarde'''
description: "U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld te wijzigen op een bestaand aangepast formulier: 'Ongeldige parameter: conversiewaarde `&lt;..&gt;`"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Foutbericht: Ongeldige parameter: conversiewaarde

## Probleem

U ontvangt het volgende foutbericht wanneer u probeert de indeling van een aangepast veld te wijzigen op een bestaand aangepast formulier: &quot;Ongeldige parameter: conversiewaarde &quot;&lt;...>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Oorzaak

Dit bericht komt in het volgende scenario voor:

U hebt bijvoorbeeld een aangepast veld dat als tekst is opgemaakt.  Nu wilt u de indeling van het aangepaste veld wijzigen in Valuta. Ergens in je [!DNL Adobe Workfront] -instantie, is dit veld al gekoppeld aan een object en bevat het al opgegeven informatie. De bestaande informatie in ten minste één dergelijk veld is al opgemaakt als tekst. Daarom kan de opmaak van het veld niet worden gewijzigd in Valuta.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Workfront] plan</a>*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] overzicht van licenties</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Toegangsniveau*</strong> </td> 
   <td> <p>Toegang bewerken tot:</p> 
    <ul> 
     <li> <p>Rapporten, dashboards en kalenders maken</p> </li> 
     <li> <p>Filters, weergaven en groepen maken</p> </li> 
    </ul> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau veranderen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Oplossing

Ga als volgt te werk:

1. Stel rapporten samen voor alle objecten waaraan dit veld is gekoppeld met hun aangepaste Forms.\
   Voor informatie over het samenstellen van een rapport raadpleegt u [Een aangepast rapport maken](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Neem het aangepaste veld dat u wilt bewerken op in de weergave van het rapport, zodat u kunt zien welk object dit veld bevat dat is gevuld met een tekstwaarde.
1. Corrigeer de aangepaste veldwaarden van de objecten die in een tekstindeling worden weergegeven en geef deze de waarde Valuta; Vervolgens probeert u het veld Indeling opnieuw te wijzigen in het aangepaste formulier.\
   of\
   Als u te veel veldwaarden hebt die al zijn gevuld met informatie met tekstopmaak, kunt u overwegen een nieuw aangepast veld toe te voegen aan uw aangepaste formulier en dit op te maken als Valuta.
