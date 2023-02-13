---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-system-defaults
title: Aanvraagtypen configureren
description: Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of een taak registreren. U kunt verzoeken ook voorleggen, die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen. Kwesties en verzoeken worden in Adobe Workfront als onderling verwisselbaar beschouwd.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 81e74a70-ea7e-4ed8-8b30-f01df0e73645
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Aanvraagtypen configureren

Tijdens het werken aan een project, zou u kunnen ontdekken dat de onverwachte gebeurtenissen zich voordoen. U kunt die onverwachte gebeurtenissen als kwesties voor een bepaald project of een taak registreren. U kunt verzoeken ook voorleggen, die als kwesties op een project worden geregistreerd dat als Rij van het Verzoek wordt aangewezen. Kwesties en verzoeken worden in Adobe Workfront als onderling verwisselbaar beschouwd.

Voor informatie over het maken van problemen in [!DNL Workfront], zie [Problemen maken](../../../manage-work/issues/manage-issues/create-issues.md). Voor informatie over het maken van aanvragen in [!DNL Workfront], zie [Maken en verzenden [!DNL Adobe Workfront] verzoeken](../../../manage-work/requests/create-requests/create-submit-requests.md). Voor informatie over het associëren van de Types van Verzoek met projecten, zie [Bepaal de Types van Verzoek voor een project](../../../manage-work/requests/create-and-manage-request-queues/define-request-types-for-project.md).

## Toegangsvereisten

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau</td> 
   <td> <p>U moet een [!DNL Workfront] beheerder.</p> <p><b>OPMERKING</b>: Als u nog steeds geen toegang hebt, vraagt u [!DNL Workfront] beheerder als zij extra beperkingen in uw toegangsniveau plaatsen. Voor informatie over hoe een [!DNL Workfront] de beheerder kan uw toegangsniveau wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--
THIS IS DRAFTED IN FLARE
<h2>Set what issue or request types are allowed for a project</h2>
<p>You can organize the kind of issues or requests that are logged in Workfront by Request Types. This organization is useful for reporting reasons and for helping users understand what kind of unexpected work might occur during the lifetime of a project.</p>
<p>You can specify the type of requests that can be logged on a project when you configure the <strong>Queue Details</strong> area for the project. </p>
<ol>
<li value="1"> <p> Click <strong>Projects</strong> in the Main Menu. <img src="assets/main-menu-icon.png"> </p> </li>
<li value="2">Click the name of the project to open it.</li>
<li value="3"> In the left panel, click <strong>Queue Details</strong>. </li>
<li value="4"> <p>In the <strong>Queue Properties</strong> section, select the <strong>Request Types</strong> you want for the project.</p> <note type="note">
You must have at least one request type selected. You can select multiple request types.
</note> </li>
<li value="5"> <p>Click <strong>Save</strong>.</p> <p>The request types you specified will be available to select when you enter a new issue on a task or a project, or when you submit a new request to the project.</p> </li>
</ol>
</div>
-->

## De namen van de aanvraagtypen aanpassen

Als [!DNL Workfront] beheerder, kunt u de namen van de verzoektypes in uw systeem vormen. De nieuwe namen zijn zichtbaar in elk gebied van [!DNL Workfront] waarbij **[!UICONTROL Issue Type]** of **[!UICONTROL Request Type]** weergegeven velden:

* In de **[!UICONTROL Queue Details]** gebied van een project dat de kwesties of verzoeken zal ontvangen.
* Als er meer dan één aanvraagtype is geselecteerd voor een aanvraagwachtrij, gaat u naar **[!UICONTROL New Issue]Formulier** in de **[!UICONTROL Issue Type]** wanneer u een nieuwe uitgave maakt of een nieuwe aanvraag indient.

   Voor meer informatie over het maken van problemen in [!DNL Workfront], zie  [Problemen maken](../../../manage-work/issues/manage-issues/create-issues.md)

   Voor meer informatie over het maken van aanvragen in [!DNL Workfront], zie  [Maken en verzenden [!DNL Adobe Workfront] verzoeken](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Op de **[!UICONTROL Queue Topic Detail]** vorm, wanneer u het Onderwerp van de Rij vormt.\
   Voor meer informatie over het creëren van de Onderwerpen van de Rij, zie [Werkvoorraadonderwerpen maken](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

U kunt als volgt de namen van de aanvraagtypen aanpassen:

1. Klik op de knop **[!UICONTROL Main Menu]** pictogram ![](assets/main-menu-icon.png) in de rechterbovenhoek van [!DNL Adobe Workfront]en klik vervolgens op **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klik op **[!UICONTROL Project Preferences]** > **[!UICONTROL Statuses]**.

1. Klik op de knop **[!UICONTROL Issues]** tab.
1. Aan de bovenkant van de **[!UICONTROL Issues]** , plaatst u de aanwijzer boven de naam van een aanvraagtype en klikt u vervolgens op de knop **[!UICONTROL Edit]** pictogram dat wordt weergegeven.

   ![](assets/edit-request-type-name-nwe.png)

1. Typ een nieuwe naam in het vak dat wordt weergegeven en druk vervolgens op **[!UICONTROL Enter]**.

## Uitgavestatus binnen verschillende aanvraagtypen configureren

U kunt elk aanvraagtype aan verschillende uitgavestatussen koppelen. U kunt ook de volgorde wijzigen waarin de statussen op een uitgave worden weergegeven, afhankelijk van het type uitgave.

Zie voor meer informatie over het wijzigen van de standaardvolgorde van emissiestatus en het configureren van emissiestatus de [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) sectie in [Een status maken of bewerken](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
