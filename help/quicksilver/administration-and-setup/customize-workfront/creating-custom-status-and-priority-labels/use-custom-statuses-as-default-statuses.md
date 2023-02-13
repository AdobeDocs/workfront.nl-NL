---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Aangepaste statussen gebruiken als standaardstatussen
description: Wanneer een douanestatus als standaardstatus wordt geplaatst, wordt de nieuwe standaardstatus gebruikt door het systeem op diverse manieren. De manieren waarin het wordt gebruikt hangt af van of het als standaardsysteem-vlakke status, of een standaardgroep-vlakke status wordt geplaatst.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '833'
ht-degree: 0%

---

# Aangepaste statussen gebruiken als standaardstatussen

Wanneer een douanestatus als standaardstatus wordt geplaatst, wordt de nieuwe standaardstatus gebruikt door het systeem op diverse manieren. De manieren waarin het wordt gebruikt hangt af van of het als standaardsysteem-vlakke status, of een standaardgroep-vlakke status wordt geplaatst.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een Workfront-beheerder zijn.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aangepaste statussen op systeemniveau

Wanneer u een aangepaste status instelt als een standaardsysteemstatus, nemen nieuwe groepen die in het systeem zijn gemaakt die status over.

Groepen die al bestonden toen u de nieuwe standaardsysteemstatus instelde, nemen deze niet automatisch over.

Stel dat er al twee groepen zijn gemaakt in uw Adobe Workfront-omgeving (marketing en verkoop). U maakt een nieuwe aangepaste status die gelijk is aan Huidig en roept de status In proces aan. U creeert nu een nieuwe groep genoemd Techniek. In dit scenario, erft de groep van de Techniek de nieuwe standaardstatus; De groepen Marketing en Verkoop doen dat niet.

## Aangepaste standaardstatussen op groepsniveau

In de volgende omstandigheden wordt een aangepaste status gebruikt die u instelt als standaardgroepsstatus:

* **Wanneer het Workfront-systeem automatisch een status kiest, wordt de standaardgroepsstatus gebruikt:** De aangepaste status die u instelt als de standaardgroepsstatus wordt gebruikt wanneer het Workfront-systeem automatisch een status toewijst aan een object.

   Bijvoorbeeld, kan een taak worden gevormd om automatisch in Volledige status te veranderen wanneer het percentage voltooide 100% bereikt. Als u een aangepaste status maakt die gelijk is aan Voltooid en u die aangepaste status instelt als standaardstatus, wijzigt Workfront de status van de taak in de nieuwe standaardstatus.

   Aangepaste statussen worden op deze manier alleen gebruikt met groepsstatussen die zijn gekoppeld aan een taak of uitgave. Aangepaste statussen kunnen op deze manier niet worden gebruikt voor statussen die aan een project zijn gekoppeld.

* De **status van een project wordt bepaald door de groep die bij het project is betrokken**: Als de groep verbonden aan een bepaald project verandert, verandert het statuut van het project afhankelijk van de standaardstatussen die voor de groep worden bepaald. (Een groep kan met een project via het gebied van Groepen worden geassocieerd wanneer het uitgeven van het project.)

   Als die groep verandert, verandert het statuut van het project als de nieuwe groep een verschillende bepaalde standaardstatus heeft die met de huidige status van het project evenaart.

   Bijvoorbeeld, kan een project met de groep van de Marketing worden geassocieerd, en het statuut van het project wordt geplaatst aan Planning. Het project wordt uitgegeven zodat het nu met de groep van de Verkoop wordt geassocieerd. De groep van de Verkoop heeft een status van de douane standaardgroep genoemd Dinking (en deze status is met Planning gelijk). Omdat de Groep op het project werd veranderd, verandert het statuut van het project nu in het Dinken.

Als u een groepsbeheerder bent, zie [Een status instellen als standaardstatus voor een groep](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Uitgiftestatus

Als de aangepaste status de status Uitgave is, moeten alle vier de uitgiftetypen hiervoor zijn ingeschakeld (Foutenrapport, Wijzigingsvolgorde, Uitgave en Verzoek). In de onderstaande status van de uitgave kan de status Opnieuw geopend bijvoorbeeld niet als standaardstatus worden gebruikt omdat het type Uitgave volgorde wijzigen niet is geselecteerd:

![](assets/all-4-issue-types-enabled.png)

## Een aangepaste status instellen als standaardstatus

1. Klik op de knop **Hoofdmenu** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van Adobe Workfront klikt u op **Instellen** ![](assets/gear-icon-settings.png).
1. Klik in het linkerdeelvenster op **Projectvoorkeuren** > **Statussen**.
1. (Voorwaardelijk) als u een standaardstatus voor een groep plaatst, begin het typen van de naam van de groep in het menu in de hoger-juiste hoek, dan selecteer het wanneer het verschijnt.
1. Open de **Project**, **Taken**, of **Problemen** , afhankelijk van het type status dat u als standaardstatus wilt instellen.
1. Klik op de knop **Standaardstatussen instellen** vervolgkeuzemenu.
1. Selecteer in het vervolgkeuzemenu dat wordt weergegeven, naast de status waar u de standaardstatus wilt instellen, de gewenste standaardstatus.
1. Klikken **Opslaan**.
1. Koppel het project aan de groep waar de status zich bevindt.

   >[!NOTE]
   >
   >Als u de douanestatus voor een groep plaatst, en u later het project aan een verschillende groep toewijst, zal de projectstatus opnieuw laden en kon veranderen.

   1. Ga naar het project waar u de douanestatus wilt gebruiken.
   1. Klik op het menu Meer ![](assets/more-icon.png)en klik vervolgens op **Bewerken**.
   1. In de **Project bewerken** in het vak dat wordt weergegeven in het dialoogvenster **Groep** veld onder **Projectkoppeling** selecteert u de groep waar de status zich bevindt.
   1. Klikken **Wijzigingen opslaan**.
