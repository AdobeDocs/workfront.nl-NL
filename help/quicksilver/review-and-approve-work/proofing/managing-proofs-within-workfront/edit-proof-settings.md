---
product-area: documents;user-management;resource-management
navigation-topic: manage-proofs-within-workfront
title: Proefdrukinstellingen bewerken
description: Nadat u een proefdruk hebt gemaakt, kunt u de proefdrukinstellingen op elk gewenst moment bewerken.
author: Courtney
feature: Digital Content and Documents
exl-id: ee30ce2c-e3dc-4863-a69b-cbc1b8747362
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Proefdrukinstellingen bewerken

Nadat u een proefdruk hebt gemaakt, kunt u de proefdrukinstellingen op elk gewenst moment bewerken.

## Toegangsvereisten

U moet de volgende toegang hebben om de stappen in dit artikel uit te voeren:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-abonnement*</td> 
   <td> <p>Huidig plan: Pro of hoger</p> <p>of</p> <p>Ouder plan: Premium</p> <p>Voor meer informatie over het proefdrukken van toegang met de verschillende plannen, zie <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Toegang tot proefdrukfunctionaliteit in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licentie*</td> 
   <td> <p>Huidig plan: Werken of plannen</p> <p>Ouder plan: Willekeurig (proefdrukken moet zijn ingeschakeld voor de gebruiker)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bewijs van machtigingsprofiel </td> 
   <td>Manager of hoger</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rol proefdrukken</td> 
   <td>Auteur of moderator</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraties op toegangsniveau*</td> 
   <td> <p>Toegang tot documenten bewerken</p> <p>Opmerking: Als u nog steeds geen toegang hebt, vraagt u de Workfront-beheerder of deze aanvullende beperkingen op uw toegangsniveau instelt. Voor informatie over hoe een beheerder van Workfront uw toegangsniveau kan wijzigen, zie <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Aangepaste toegangsniveaus maken of wijzigen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Neem contact op met de beheerder van de Workfront of Workfront-proefdrukken als u wilt weten welk plan, welke rol of welk proefdrukprofiel u hebt.

## Proefdrukinstellingen bewerken

Sommige instellingen zijn mogelijk vergrendeld als uw Workfront-beheerder deze op accountniveau heeft uitgeschakeld.

1. Ga naar het project, de taak, of de kwestie waar u het proef wilt, dan klik **Documenten** tab.
1. Plaats de muis boven de proefdruk en klik vervolgens op **Documentdetails**.
1. Klik in het linkerdeelvenster op **Instellingen van viewer proefdrukken**.
1. Pas de volgende instellingen aan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aanmelding vereist. Dit bewijs kan niet met gastgebruikers worden gedeeld</td> 
      <td> <p>Als u hogere veiligheidsniveaus voor uw overzicht en goedkeuringsproces vereist, kunt u login aan de proef gebruiken. Dit betekent dat alleen Workfront-gebruikers aan de proefdruk kunnen worden toegevoegd. Ze moeten hun e-mail en wachtwoord invoeren voordat ze deze kunnen openen.</p> <p>Opmerking: <em style="font-style: normal;">Als Aanmelding vereist is ingeschakeld, kunnen abonnementen niet worden ingeschakeld.</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vereisen dat besluiten elektronisch worden ondertekend</td> 
      <td> <p>U kunt een elektronische handtekening eisen van elke controleur die een besluit neemt over het bewijs. Wanneer een revisor een beslissing neemt, verschijnt er een vraag om de controleur te vragen zijn e-mail en wachtwoord in te voeren en zijn beslissing te bevestigen. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information, see 
          <a href="../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md" class="MCXref xref">Understanding electronic signatures in Workfront Proof</a>
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bewijs vergrendelen wanneer alle vereiste beslissingen zijn genomen</td> 
      <td> <p>U kunt een proefstaat instellen om te vergrendelen wanneer de uiteindelijke fiatteur zijn beslissing neemt. Dit is handig als u ervoor wilt zorgen dat de controleurs niet naar de proefdruk kunnen terugkeren en extra opmerkingen kunnen toevoegen of hun beslissingen kunnen wijzigen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Downloaden van het oorspronkelijke bestand toestaan</td> 
      <td> <p>U kunt de controleurs op een proefdruk toestaan om het originele dossier te downloaden waarvan een proef werd gecreeerd. Dit is standaard ingeschakeld.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Delen van proefdrukken via openbare URL of insluitcode toestaan</td> 
      <td>U kunt gebruikers toestaan om de proef met een openbare URL te delen of code in te bedden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abonneren op proefdrukken via openbare URL of insluitcode toestaan</td> 
      <td> <p>Als u een abonnement op de proefdruk inschakelt, kunnen personen die niet expliciet aan de proefdruk zijn toegevoegd, zich bij de proefdruk abonneren (door zich aan de proefdruk toe te voegen). Vervolgens krijgen ze de rol en e-mailwaarschuwing toegewezen die u voor hen selecteert in de Abonnementsinstellingen.</p> <p>Als Subscription is ingeschakeld op een proefdruk, worden de onderstaande velden geactiveerd:</p> 
       <ul> 
        <li><strong>Validatie van abonnee vereist</strong> - Abonnees moeten op een koppeling in een e-mailbericht klikken om een proefafdruk te openen<br>Als u deze optie selecteert, krijgt de persoon die zich abonneert geen directe toegang tot de proefdruk, maar een koppeling naar de proefdruk in een e-mail. Het doel van abonneevalidering is ervoor te zorgen dat de persoon een correct e-mailadres heeft ingevoerd waartoe hij toegang heeft.</li> 
        <li><strong>Standaardrol voor nieuwe abonnees -</strong> Dit is de standaardproefrol die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li> 
        <li><strong>Standaard-e-mailwaarschuwing voor nieuwe abonnees</strong> - Dit is de standaard e-mailwaarschuwing die wordt toegewezen aan alle revisoren die zich op de proefdruk abonneren.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klikken **Opslaan**.

 
