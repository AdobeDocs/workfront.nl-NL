---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Andere tags toepassen op updates
description: Wanneer u updatecommentaren op een Adobe Workfront-object opgeeft, kunnen alle gebruikers van het project de verzonden informatie zien. Er kunnen zich echter situaties voordoen waarin gebruikers die zich niet bij het project bevinden, baat zouden hebben bij het bekijken van deze informatie. In plaats van deze gebruikers op te nemen in het project, kunt u ze labelen op de update om deze met hen te delen. Gelabelde gebruikers ontvangen een gebeurtenismelding.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Andere tags toepassen op updates

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
U kunt gebruikers tags toewijzen wanneer u een update uitvoert naar een object als u de aandacht wilt vestigen op een object dat ze anders wellicht niet volgen.
In plaats van deze gebruikers op het object te plaatsen door ze eraan toe te wijzen of door ze ertoe te brengen zich erop te abonneren, kunt u ze in de update labelen om het met hen te delen. Gelabelde gebruikers ontvangen een melding over de update die u invoert.

>[!NOTE]
>
>Een gebeurtenismelding moet zijn ingeschakeld voordat een gebruiker het e-mailbericht kan ontvangen. Beheerders kunnen meldingen inschakelen voor het hele systeem of voor een groep op hoofdniveau. Een gebruiker kan individuele gebeurtenisberichten in zijn eigen gebruikersprofiel ook toelaten en onbruikbaar maken. Raadpleeg de volgende secties voor meer informatie:
>
>* [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [Gebeurtenismeldingen voor een groep weergeven en configureren](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


Voor informatie over het toevoegen van updates aan Workfront-objecten raadpleegt u [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>Wanneer een kwestie in een project of een taak wordt omgezet, worden de updates gekopieerd aan het nieuwe project of de taak, maar de geëtiketteerde gebruikers niet. Om het gesprek voort te zetten, moet u de deelnemers opnieuw etiketteren.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>een verzoek of hoger indienen voor kwesties en documenten; Reviseren of hoger voor alle andere objecten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>de aanvrager of hoger voor kwesties en documenten; Revisor of hoger voor alle andere objecten</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Toegang tot het object weergeven</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Neem contact op met uw Workfront-beheerder om te weten te komen welk abonnement, licentietype of toegang u hebt.

## Andere tags toepassen op updates

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. Beginnen met het bijwerken van een tijdelijk item, zoals beschreven in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In de **Waarschuwen** typt u de naam van de gebruiker of het team dat u wilt opnemen en klikt u op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   of

   Typ het @-symbool in het dialoogvenster **Een nieuwe update starten** typt u de naam van de gebruiker of het team dat u in de update wilt opnemen en klikt u vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   >[!TIP]
   >
   >Als u de juiste gebruiker wilt identificeren wanneer er gebruikers met vergelijkbare of identieke namen zijn, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze in een update codeert.

   ![](assets/tag-users-in-update.png)

1. (Optioneel) Schakel de optie **Privé voor mijn bedrijf** in de rechterbenedenhoek van het updatevak. Hierdoor is de update alleen zichtbaar voor gebruikers in uw bedrijf.

   >[!NOTE]
   >
   >Gelabelde gebruikers buiten het bedrijf konden nog steeds een melding in de app of een e-mail ontvangen, ook al zullen ze de persoonlijke opmerkingen op het tabblad Updates niet zien. We raden u aan geen tags toe te wijzen aan externe gebruikers tijdens een update als u de gegevens niet met hen wilt delen.

1. (Optioneel) Herhaal stap 2 om meerdere gebruikers en teams toe te voegen.

   >[!NOTE]
   >
   >Alle gebruikers en teamleden die in het veld Waarschuwen worden vermeld, ontvangen een melding in de app voor de update en ontvangen mogelijk een e-mail, afhankelijk van de configuratie van hun instellingen voor e-mailmeldingen. Gebruikers die zichzelf in een opmerking of antwoord labelen, ontvangen een melding voor die opmerking of reactie en kunnen hun naam voor de rest van de thread in het veld Waarschuwen weergeven, maar ontvangen geen andere melding tenzij ze zichzelf opnieuw labelen. Zie voor meer informatie [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) en [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klikken **Bijwerken**.\
   Aan gebruikers die zijn opgenomen in de update, wordt automatisch weergavemachtiging toegekend aan het object en deze gebruikers kunnen updates die aan het object zijn toegevoegd, weergeven en erop reageren.

   U kunt zien wie in elk antwoord bij de bovenkant van de updatedraad is geëtiketteerd. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord.

   ![](assets/tagging-transparency-350x192.png)

   Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->