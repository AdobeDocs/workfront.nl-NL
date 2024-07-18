---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: De Workfront for Adobe Experience Manager verbeterde connector verwijderen
description: U moet de installatie van de Workfront met Adobe Experience Manager Enhanced-aansluiting ongedaan maken voor de meest recente geïntegreerde verbinding tussen Workfront en Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# De Workfront verwijderen met de Adobe Experience Manager Enhanced-aansluiting

U moet de installatie van de Workfront met Adobe Experience Manager Enhanced-aansluiting ongedaan maken voor de meest recente geïntegreerde verbinding tussen Workfront en Adobe Experience Manager Assets as a Cloud Service.

## Vereisten

* (Optioneel) Herstel indien nodig de wijzigingen die zijn aangebracht in de configuratie van de Workfront-firewall en de AEM-verzendinstellingen.

## De verbeterde aansluiting verwijderen

1. Open en kloon uw AEM as a Cloud Service-opslagplaats vanuit Cloud Manager.

1. Open de gekloonde opslagplaats voor kompassen in de IDE van uw keuze.

1. De vertakking uitchecken waar de verbeterde aansluiting is geïnstalleerd.

1. Navigeer naar het volgende pad en verwijder het verbeterde ZIP-bestand voor de connector:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Verwijder de volgende afhankelijkheid van het bestand pom.xml van de hoofdmap van het project.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Controleer of de versie waarnaar in het bovenstaande codeblok wordt verwezen, namelijk 1.8.0, de versie weergeeft die uit de code wordt verwijderd.

1. Verwijder het volgende gebiedsdeel uit het pom.xml- dossier van submodule van het project genoemd **allen**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Verwijder het volgende ingebedde uit het pom.xml- dossier van submodule van het project genoemd allen.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Voorwaardelijk) verwijder de bewaargegevensconfiguratie uit het pom.xml- dossier van de wortel van het project.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Voorwaardelijk) verwijder de serverconfiguratie uit settings.xml, aanwezig in de volgende weg./cloudmanager/maven/settings.xml in de hoofdmap van het project.&#39;

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Leg de wijzigingen vast en druk de code naar de Cloud Manager-opslagplaats

1. Voer de Cloud Manager-pijplijn uit om de wijzigingen op uw Cloud Servicen-instantie te implementeren
