---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Andere tags toepassen op updates
description: Wanneer u updatecommentaren op een Adobe Workfront-object opgeeft, kunnen alle gebruikers van het project de verzonden informatie zien. Er kunnen zich echter situaties voordoen waarin gebruikers die zich niet bij het project bevinden, baat zouden hebben bij het bekijken van deze informatie. In plaats van deze gebruikers op te nemen in het project, kunt u ze labelen op de update om deze met hen te delen. Gelabelde gebruikers ontvangen een gebeurtenismelding.
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: bbd99435bb07d68bf9058bcd3e8c6ef5d9df75a9
workflow-type: tm+mt
source-wordcount: '1370'
ht-degree: 0%

---

# Andere tags toepassen op updates

<!--take "Beta" references out when we remove the beta-->


<span class="preview">De gemarkeerde informatie op deze pagina verwijst naar functionaliteit die nog niet algemeen beschikbaar is. Deze optie is alleen beschikbaar in de voorvertoningsomgeving.

>[!NOTE]
>
>De ervaring met opmerkingen wordt momenteel opnieuw ontworpen in Adobe Workfront.
>Ga voor meer informatie over de nieuwe ervaring met bijwerken naar [Nieuwe ervaring met opmerkingen](../updating-work-items-and-viewing-updates/unified-commenting-experience.md).
>
>U hebt toegang tot het nieuwe ontwerp voor de volgende objecten:
> * <span class="preview">Problemen bij het inschakelen van het bètabestand voor opmerkingen. </span>
   >
   >     <span class="preview">Deze functionaliteit is alleen beschikbaar voor de sectie Updates van problemen en is niet beschikbaar voor de volgende gebieden:</span>
   >
   >     * <span class="preview">Home</span>
   >     * <span class="preview">Samenvattingspaneel in lijsten</span>
   >     * <span class="preview">Samenvattingspaneel in tijdbladen</span>
>
> * Doelen
   >   De nieuwe ervaring met opmerkingen is de standaardeigenschap voor doelen. U moet een extra licentie hebben om toegang te krijgen tot Workfront Goals. Zie voor meer informatie [Vereisten voor het gebruik van Workfront-doelen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

   >
   >    Zie voor informatie over opmerkingen over doelen [Doelopmerkingen beheren in Adobe Workfront-doelen](../../workfront-goals/goal-management/manage-goal-comments.md).



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

Het labelen van anderen in een update is afhankelijk van de ervaring en het object dat u selecteert.

### Andere tags toepassen op updates in de sectie Huidige updates

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

<div class="preview">

### Andere tags toepassen op updates in de bètaervaring voor opmerkingen

1. Beginnen met het bijwerken van een tijdelijk item, zoals beschreven in [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In de **Tags toewijzen aan personen of teams** typt u de naam van de gebruiker of het team dat u wilt opnemen en klikt u op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   of

   Typ het @-symbool in het dialoogvenster **Een opmerking schrijven** typt u de naam van de gebruiker of het team dat u in de update wilt opnemen en klikt u vervolgens op de naam wanneer deze wordt weergegeven in de vervolgkeuzelijst.

   >[!TIP]
   >
   >Als u de juiste gebruiker wilt identificeren wanneer er gebruikers met vergelijkbare of identieke namen zijn, ziet u de avatar, de primaire rol van de gebruiker of hun e-mailadres. Gebruikers moeten aan ten minste één taakrol zijn gekoppeld om deze te kunnen bekijken terwijl u ze in een update codeert.

   ![](assets/tag-others-unified-commenting.png)

1. (Optioneel) Schakel de optie **Privé voor mijn bedrijf** in de rechterbenedenhoek van het updatevak. Hierdoor is de update alleen zichtbaar voor gebruikers in uw bedrijf.

   >[!NOTE]
   >
   >* Deze optie toont slechts wanneer de gebruiker met een Bedrijf wordt geassocieerd.
   >* Gelabelde gebruikers buiten het bedrijf konden nog steeds een melding in de app of een e-mail ontvangen, ook al zullen ze de persoonlijke opmerkingen op het tabblad Updates niet zien. We raden u aan geen tags toe te wijzen aan externe gebruikers tijdens een update als u de gegevens niet met hen wilt delen.


1. (Optioneel) Herhaal stap 2 om meerdere gebruikers en teams toe te voegen. <!--insure this stays accurate-->

   >[!NOTE]
   >
   >Alle gebruikers en teamleden die in het veld &quot;Tagpersonen of -teams&quot; worden vermeld, ontvangen een melding in de app voor de update en ontvangen mogelijk een e-mail, afhankelijk van de configuratie van hun instellingen voor e-mailmeldingen. Gebruikers die zichzelf in een opmerking of antwoord labelen, ontvangen een melding voor die opmerking of reactie en kunnen hun naam als lid van de thread voor de rest van de thread zien, maar ontvangen geen andere melding tenzij ze zichzelf opnieuw labelen. Zie voor meer informatie [Uw eigen gebeurtenismeldingen activeren of deactiveren](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) en [Gebeurtenismeldingen configureren voor iedereen in het systeem](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Klikken **Verzenden**.\
   Aan gebruikers die zijn opgenomen in de update, wordt automatisch weergavemachtiging toegekend aan het object en deze gebruikers kunnen updates die aan het object zijn toegevoegd, weergeven en erop reageren.

   U kunt zien wie in elk antwoord onder de tekst van de update is gelabeld, in het gebied Leden. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord.
1. (Optioneel) Klik op het nummer van **Leden** opgenomen in de update om een lijst weer te geven met entiteiten waarmee de update die u hebt ingevoerd, wordt gedeeld.

   ![](assets/members-icons-expanded-unshimmed.png)

   Voor informatie over de extra functionaliteit die beschikbaar is wanneer het bijwerken van een het werkpunt, zie [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).