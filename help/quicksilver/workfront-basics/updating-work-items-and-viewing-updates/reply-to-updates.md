---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Reageren op updates
description: Wanneer iemand toevoegt of op een update op een het werkvoorwerp antwoordt, verschijnt hun antwoord in de communicatie draad in de sectie van Updates voor het voorwerp. U kunt een antwoord toevoegen aan een update of als u toegang tot het object hebt met Weergave.
author: Lisa and Alina
feature: Get Started with Workfront
role: User
topic: Collaboration
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: d93d42322d62ff5eb927ca13febcb763cbec3f13
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%

---

# Reageren op updates

<!--take "Beta" references out when we remove the beta and change "current" to "legacy" after October 26-->

<!--after August 17: 
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases. </span>  
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/enable-fast-release-process.html?lang=en ). </span>  
<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span>-->

<!--replace the note below with this at August 17: 
>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>Depending on what environment and what objects you access the commenting experience from, you might see different functionality in the Updates section. 
>For more information about the new commenting experience and its availability, see [New commenting experience](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
>
>The new commenting experience is available only for the Updates section, and it is not available for the following areas:
>
> * Home
> * Summary panel in lists
> * Summary panel in timesheets

-->

>[!NOTE]
>
>De ervaring met opmerkingen wordt momenteel opnieuw ontworpen in Adobe Workfront.
>
>Ga voor meer informatie over de nieuwe opmerkingervaring naar [Nieuwe ervaring met opmerkingen](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
>
>U hebt toegang tot de nieuwe ervaring voor de volgende objecten:
> * Kwesties, projecten, taken, en documenten.
>
>     Deze optie is beschikbaar wanneer u de bètaervaring voor opmerkingen inschakelt.
>
>     Deze functionaliteit is alleen beschikbaar voor de sectie Updates en is niet beschikbaar voor de volgende gebieden:
>
>     * Home
>     * Samenvattingspaneel in lijsten
>     * Samenvattingspaneel in tijdbladen
>
> * Doelen, kaarten in het gebied van de raden
>
>   De nieuwe ervaring met opmerkingen is de enige ervaring voor doelen en kaarten. U moet een extra licentie hebben om toegang te krijgen tot Workfront Goals. Zie voor meer informatie [Vereisten voor het gebruik van Workfront-doelen](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
>
>     U kunt updates aan kaarten in het gebied van Boards toevoegen en bekijken wanneer u de Commentaren en de secties van de Activiteit van het Systeem op een kaart toelaat. Zie voor meer informatie [Een ad-hockaart aan een kaart toevoegen](../../agile/get-started-with-boards/add-card-to-board.md).


Wanneer iemand op een commentaar of een systeemupdate op een het werkvoorwerp antwoordt, verschijnt hun antwoord in de communicatie draad in de sectie van Updates voor het voorwerp.

>[!IMPORTANT]
>
>Het is niet mogelijk te reageren op systeemupdates in de nieuwe opmerkingervaring. Zie voor meer informatie [Nieuwe ervaring met opmerkingen](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).


## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-abonnement*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licentie*</strong></td> 
   <td> <p>Vragen of hoger voor problemen en documenten; controleren of hoger voor alle andere objecten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraties op toegangsniveau*</strong></td> 
   <td> <p>Aanvrager of hoger voor uitgaven en documenten; revisor of hoger voor alle andere objecten</p> <p><b>OPMERKING</b>

Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objectmachtigingen</strong></td> 
   <td> <p>Toegang tot het object weergeven</p> <p>Voor informatie over het aanvragen van aanvullende toegang raadpleegt u <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Toegang tot objecten aanvragen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met uw Workfront-beheerder om te weten te komen welk plan, licentietype of toegang u hebt.

## Reageren op een update of een antwoord in Workfront

U kunt reageren op een opmerking in de thread van een object dat u kunt weergeven, of u kunt zich aanmelden als Workfront of groepsbeheerder en reageren op een opmerking namens een andere gebruiker. Zie voor meer informatie [Aanmelden als een andere gebruiker](../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).

Het antwoord op een opmerking of antwoord is afhankelijk van de ervaring en het object dat u selecteert.

### Reageren op een update of antwoord in de huidige sectie Updates

1. Ga naar het object waaraan u een antwoord wilt toevoegen.
1. Op de **Updates** zoekt u de update of het antwoord waarop u wilt antwoorden.

1. (Optioneel) Voer een van de volgende handelingen uit om een afbeelding weer te geven in de bestaande update:

   * Klik op de knop **Voorvertoning** pictogram ![](assets/previewimageicon-31x31.png) op de miniatuur van de afbeelding om de afbeelding op volledige grootte te openen in een nieuw browsertabblad.
   * Klik op de knop **Downloaden** pictogram ![](assets/downloadimageicon.png) op de miniatuur van de afbeelding om de afbeelding te downloaden.

1. Klikken **Antwoord** in de update typt u een antwoord in het vak dat wordt weergegeven.

   U kunt de gebruikers zien die actief in het gesprek betrokken zijn of in elk antwoord bij de bovenkant van die updatedraad geëtiketteerd. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord. U kunt ook tags toewijzen aan meer gebruikers om deze in uw antwoord op te nemen.  Als u meer gebruikers wilt labelen, raadpleegt u [Andere tags toepassen op updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. (Optioneel) Als u tekst uit een vorige update wilt opnemen in uw antwoord, klikt u op de knop **Meer** menu naast de update of het antwoord dat u wilt citeren, en klik dan **Aanhalingsreactie**. De tekst van de vorige update wordt weergegeven in het invoergebied, gemarkeerd met een verticale grijze lijn.
1. (Optioneel) Gebruik opmaak, emojis, neem koppelingen of afbeeldingen op zoals wordt uitgelegd in de sectie &#39;Rijke tekst gebruiken in een Workfront-update&#39; in het artikel [Werk bijwerken](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. Klikken **Antwoord** om het antwoord op te slaan.

### Reageren op een opmerking bij gebruik van de nieuwe opmerkingervaring

Ga voor meer informatie over de functies die beschikbaar zijn in de nieuwe opmerkingervaring en voor welke objecten [Nieuwe ervaring met opmerkingen](../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

1. Ga naar het object waaraan u een antwoord wilt toevoegen.
1. Klikken **Updates** en klik vervolgens op de knop **Opmerkingen** voor het object en zoek naar de opmerking of het antwoord waarop u wilt reageren.
1. (Optioneel) Als u tekst uit een vorige update wilt opnemen in uw antwoord, klikt u op de knop **Meer** menu naast de update of het antwoord dat u wilt citeren <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>-->en klik vervolgens op **Offerteantwoord**. De tekst van de vorige update wordt weergegeven in het invoergebied, gemarkeerd met een verticale grijze lijn.
1. Klikken **Antwoord**.

   U kunt de gebruikers zien die actief in het gesprek bij de bodem van zijn betrokken **Nieuwe opmerking** en kunt u meer toevoegen of verwijderen van de niet-relevante vakken. Deze gebruikers ontvangen, samen met gebruikers die op het object zijn geabonneerd, een melding wanneer het object wordt bijgewerkt of geantwoord. U kunt ook tags toewijzen aan meer gebruikers om deze in uw antwoord op te nemen.  Als u meer gebruikers wilt labelen, raadpleegt u [Andere tags toepassen op updates](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. Begin uw antwoord te typen en gebruik om het even welke extra opties van de Rich toolbar van de Tekst. Voor informatie over het gebruiken van RTF of andere het bijwerken mogelijkheden, zie [Werk bijwerken](../updating-work-items-and-viewing-updates/update-work.md).

1. Klikken **Verzenden** om het antwoord op te slaan.

1. (Optioneel) Klik op de knop **Meer** menu ![](assets/more-menu.png) naast de update <!--(replace placing of the More menu - August 17) <span class="preview">in the upper-right corner of the comment you want to reply to</span>--> voor meer opties om het antwoord te beheren. Zie voor meer informatie [Werk bijwerken](../updating-work-items-and-viewing-updates/update-work.md).


## Reageren op een update van een e-mailbericht

Afhankelijk van de configuratie van uw e-mailberichten, ontvangt u mogelijk een e-mailmelding wanneer een update wordt uitgevoerd naar bepaalde objecten waartoe u toegang hebt.

U kunt op de volgende manieren reageren op een update van een e-mailmelding:

* Reageren op het e-mailbericht dat u ontvangt. Uw antwoordbericht wordt toegevoegd als Workfront-antwoord op de oorspronkelijke opmerking.
* Gebruik de knop Opmerking in het e-mailbericht om terug te navigeren naar Workfront en de update te beantwoorden in het gedeelte Updates.

Hieronder ziet u een voorbeeld van een e-mailmelding die wordt geactiveerd als gevolg van een update op het tabblad Updates van een taak:

![email.png](assets/email-350x202.png)

Zie voor meer informatie [E-mailberichten beantwoorden](../updating-work-items-and-viewing-updates/reply-to-email-notifications.md).






