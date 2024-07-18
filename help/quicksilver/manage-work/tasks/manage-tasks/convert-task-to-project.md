---
product-area: projects
navigation-topic: manage-tasks
title: Een taak omzetten in een project
description: Wanneer een taak in een project een grotere hoeveelheid inspanning vereist om te voltooien dan u oorspronkelijk gepland, kunt u het in een project omzetten.
author: Alina
feature: Work Management
exl-id: a45f0af4-1768-4f20-80d4-912e6fe0fc03
source-git-commit: b781687b175167784367a2fdec158d97fb3fd6a4
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 0%

---

# Een taak omzetten in een project

Wanneer een taak in een project een grotere hoeveelheid inspanning vereist om te voltooien dan u oorspronkelijk gepland, kunt u het in een project omzetten.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot taken en projecten bewerken</p> <p>Bekijk of hogere toegang tot Malplaatjes, wanneer het omzetten in een project gebruikend een malplaatje</p> <p>Opmerking: als u nog steeds geen toegang hebt, vraag dan aan de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau heeft ingesteld. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref"> tot douanetoegangsniveaus </a> leiden of wijzigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objectmachtigingen</td> 
   <td> <p>Rechten voor een taak beheren</p> <p>De toestemmingen van de mening op een malplaatje, als het omzetten in een project gebruikend een malplaatje</p> <p>Nadat u het project hebt gemaakt, hebt u beheerdersmachtigingen voor het project</p> <p>Voor informatie bij het vragen van om extra toegang, zie <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref"> de toegang van het Verzoek tot voorwerpen </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; om te weten te komen welk plan, vergunningstype, of toegang u hebt, contacteer uw beheerder van Workfront.

## Overwegingen bij het omzetten van taken in projecten

* U kunt een taak in een leeg project of in een project omzetten gebruikend een malplaatje.
* De oorspronkelijke taak wordt verwijderd.
* Alle subtaken, kwesties en nota&#39;s komen tot het nieuwe project.
* Documenten, documentversies en proefdrukken worden naar het nieuwe project verplaatst.
* De status en het percentage voltooide van alle subtaken en kwesties worden bewaard.
* Gedeelde gebruikers van de taak worden gedeelde gebruikers op het project.
* De begindatum van het project is ingesteld op de begindatum van de taak.
* De volgende lijst maakt een lijst van projectinformatie en of het van het malplaatje of van de taak overbrengt:

  <table style="table-layout:auto"> 
  <col> 
  <col> 
  <tbody> 
    <tr> 
    <td>Beschrijving</td> 
    <td> <p>De beschrijving van de taak draagt over naar het nieuwe project. </p> <p> Als er geen beschrijving op de taak is, brengt de Beschrijving van het malplaatje aan het project over. </p> <p>Als het veld Beschrijving zowel voor de taak als voor de sjabloon leeg is, is het veld in het project leeg. </p> </td> 
    </tr> 
    <tr> 
    <td>Status</td> 
    <td> Standaardstatus geselecteerd voor de groep op de sjabloon. Als het malplaatje niet met de groep wordt geassocieerd, wordt de projectstatus geplaatst aan de standaardstatus die door de beheerder van Workfront op het gebied van de Voorkeur van het Project van Opstelling wordt geplaatst. Voor informatie, zie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md"> systeem-brede projectvoorkeur </a> vormen

  De volgende scenario&#39;s bestaan voor het bijwerken van de Status van het project:
  <ul>
    <li> Als de taakstatus 'Nieuw' is, wordt de projectstatus ingesteld op 'Planning'.</li>
    <li> Als de taakstatus 'In uitvoering' is, wordt de projectstatus ingesteld op 'Huidig'.</li>
    <li> Als de taakstatus 'Voltooid' is, wordt de projectstatus ingesteld op 'Voltooid'.</li></ul>

  </td> 
    </tr> 
    <tr> 
    <td>Prioriteit</td> 
    <td>Overdrachten van de taak aan het project, of het brengt van het malplaatje over, als u in de omzetting gebruikt. </td> 
    </tr> 
    <tr> 
    <td>URL</td> 
    <td> <p>De URL van de taak wordt overgedragen naar het nieuwe project. </p> <p> Als er geen URL op de taak wordt gespecificeerd, brengt URL van het malplaatje naar het project over. </p> <p>Als het veld URL zowel voor de uitgave als voor de sjabloon leeg is, is het veld in het project leeg. </p> </td> 
    </tr> 
    <tr> 
    <td>Type projectvoorwaarde</td> 
    <td>Overdrachten uit de sjabloon.</td> 
    </tr> 
    <tr> 
    <td>Projectvoorwaarde</td> 
    <td>Komt overeen met de standaardvoorkeur op systeemniveau zoals bepaald door de Workfront-beheerder in het gedeelte Setup. Voor informatie, zie <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md"> plaats een douanetoewijzing als gebrek voor projecten </a>
    </td> 
    </tr> 
    <tr> 
    <td>Schema vanuit</td> 
    <td>Overdrachten uit de sjabloon.</td> 
    </tr> 
    <tr> 
    <td>Projectdatums</td> 
    <td> 
      <ul> 
      <li> <p><b> Geplande Datum van het Begin </b>: De dichtstbijzijnde arbeidstijd die op de het werktijd van het malplaatjeprogramma wordt gebaseerd zou, volgens de tijdzone van het programma van het malplaatje vooraf moeten worden geselecteerd. Dit veld is uitgeschakeld als het veld Planning van wordt ingesteld op Van voltooiing. </p> </li> 
      <li> <p><b> Geplande Datum van de Voltooiing </b>: De dichtstbijzijnde die arbeidstijd op de de werktijd van het malplaatjeprogramma wordt gebaseerd zou, volgens de tijdzone van het programma van het malplaatje vooraf moeten worden geselecteerd. Dit veld is uitgeschakeld als het veld Planning van wordt ingesteld op Van begin. </p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
    <td>Portfolio</td> 
    <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
    </tr> 
    <tr> 
    <td>Programma</td> 
    <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
    </tr> 
    <tr> 
    <td>Groep</td> 
    <td><p> De volgende scenario's bestaan:</p>
      <ul><li>Als een groep tijdens de omzetting wordt gespecificeerd, wordt dat de groep van het project</li>
      <li>Als u in een project omzet gebruikend een malplaatje, en er een groep op het malplaatje is, en tijdens de omzetting u geen groep specificeert, dan wordt de groep van het malplaatje de groep van het nieuwe project</li>
      <li> Als er geen groep op het malplaatje is en u geen groep tijdens de omzetting specificeert, dan wordt de groep van het oorspronkelijke project van de kwestie de groep van het nieuwe project</li> </ul>
        </td> 
    </tr> 
    <tr> 
    <td>Bedrijf</td>    
    <td>  Overdrachten uit de sjabloon. Anders is dit veld leeg.</td>

  </tr> 
    <tr> 
    <td>Projecteigenaar</td> 
    <td>Overdrachten van het gebied van de Eigenaar van het Malplaatje op het malplaatje. Anders, wordt het geplaatst aan het programma geopende gebruiker die de omzetting uitvoert. </td> 
    </tr> 
    <tr> 
    <td>Projectsponsor</td> 
    <td>Overschrijvingen van het veld Sjabloonsponsor op de sjabloon. Anders is dit veld leeg.</td> 
    </tr> 
    <tr> 
    <td>Resource Manager</td> 
    <td>Overdrachten uit de sjabloon. Anders is dit veld leeg.</td> 
    </tr> 
    <tr> 
    <td>Taakinstellingen</td> 
    <td>Overdracht van de sjabloon.</td> 
    </tr> 
    <tr> 
    <td>Instellingen van uitgave</td> 
    <td>Overdracht van de sjabloon. </td> 
    </tr> 
    <tr> 
    <td>Toegang</td> 
    <td> <p>Overdrachten van de sectie van de Toegang op het malplaatje. </p> </td> 
    </tr> 
    <tr> 
    <td>Goedkeuringen</td> 
    <td>Overdracht van de sjabloon. De goedkeuringen die aan de taak zijn gekoppeld, worden tijdens de conversie verwijderd. </td> 
    </tr> 
  </tbody> 
  </table>


## Een taak omzetten in een project

1. Ga naar de taak die u in een project wilt omzetten.
1. Klik **Meer** pictogram ![](assets/more-icon.png), toen **Bekeerling in Project**.
1. Kies een van de volgende opties:

   * **Nieuw Project**
   * Een malplaatje in **Uitgezocht van de sectie van Malplaatjes**

     ![](assets/convert-task-to-project-template-option-dropdown-nwe-350x209.png)

1. Klik **verdergaan** op het bericht dat verschijnt.
1. In de **Bekeerling aan de doos van het Project**, specificeer het volgende:

   * **Naam**: Noem uw project. De standaardnaam is de naam van de taak.
   * (Facultatief) **Beschrijving**: Beschrijf het doel voor dit project.
   * (Facultatief en voorwaardelijk) als u hebt geselecteerd om een project van een malplaatje tot stand te brengen, werk de beschikbare gebieden in de **Bekeerling in de dialoogdoos van het Project** bij.

     Voor meer informatie over het uitgeven van gebieden op projecten, zie [ projecten ](../../../manage-work/projects/manage-projects/edit-projects.md) uitgeven.

     >[!TIP]
     >
     >Als u velden in het gedeelte Financiën in het vak Converteren naar project wilt bijwerken, moet u toegang tot financiële gegevens op uw toegangsniveau bewerken hebben. Als u toegang van de Mening tot Financiële Gegevens in uw toegangsniveau hebt alle financiële informatie van de malplaatjeoverdrachten aan het nieuwe project en u kunt niet het uitgeven terwijl u de kwestie omzet. Voor informatie, zie [ toegang van de Verlening tot financiële gegevens ](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) en [ Deel een malplaatje ](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * (Facultatief) voeg **Aangepaste Forms** aan het nieuwe project toe.

     >[!TIP]
     >
     >Als een aangepast formulier voor meerdere objecten dat aan de taak is gekoppeld, is geconfigureerd voor zowel taken als projecten, blijft alle informatie die in het formulier is opgeslagen, behouden wanneer u de conversie uitvoert.
     >
     >
     >Als u een sjabloon voor de conversie gebruikt en een aangepast formulier dat aan de sjabloon is gekoppeld, een aangepast veld bevat dat ook wordt gevonden in een aangepast formulier dat aan de taak is gekoppeld, wordt de veldwaarde van de taak gebruikt voor het nieuwe project. Als het aangepaste veld echter leeg is op de taak, wordt de waarde uit de sjabloon gebruikt.

1. Klik **sparen Veranderingen**.
