# GreenCodeLab.github.io

Ce projet contient le référentiel des règles du [Green Code Label](https://www.greencode-label.org/), également consultable [ici](https://greencodelab.github.io/).

Les règles sont réparties en différentes catégories :

- [code côté client](#code-client) ;
- [code côté serveur](#code-serveur) ;
- [contenu](#contenu) ;
- [design](#design) ;
- [hébergement](#hebergement) ;
- [mesure](#mesure) ;
- [processus](#processus).

Chaque règle possède deux attributs : *validated* et *level*.

L'attribut *validated* prend la valeur *true* si la règle est validée et utilisée pour les audits de labellisation du Green Code Label.

L'attribut *level* permet de distinguer les règles selon 2 niveaux (1 ou 2). Ces niveaux sont utilisés dans la notation pour l'obtention du label.

## Code - Client

- [Adapter le fonctionnement si l’utilisateur ne visualise pas la fenêtre](/code-client/AdaptProcessingIfWindowNotFocused.md)
- [Proposer une alternative en l'abscence de script](/code-client/AddAlternativeInAbsenceOfScript.md)
- [Proposer un titre de page](/code-client/AddPageTitle.md)
- [Ne pas lancer des contenus de type vidéo, sons sans action de l’utilisateur (dont le passage à la souris)](/code-client/AvoidAutomaticLaunchingOfMultimediaContentWithoutUserAction.md)
- [Ne pas rafraîchir les pages](/code-client/AvoidPageRefresh.md)
- [Ne pas charger de données lourdes si elles ne sont pas visibles](/code-client/DoNotLoadNonVisibleHeavyData.md)
- [Minimiser le nombre d’iframes](/code-client/MinimizeNumberIframes.md)
- [Nommer les liens](/code-client/NameLinks.md)
- [Réduire la profondeur du DOM](/code-client/ReduceDOMDepth.md)
- [Supprimer les lignes vides du HTML](/code-client/RemoveEmptyLinesInHTML.md)
- [Utiliser des timers les plus adéquats aux exigences de performance](/code-client/UseAppropriateTimersToPerformanceRequirements.md)

## Code - Serveur

- [Mettre en cache le bytecode](/code-server/CacheBytecode.md)
- [Mettre en cache les données calculées souvent utilisées](/code-server/CacheOftenUsedCalculatedData.md)
- [Limiter le nombre de résultats des requêtes en base de données](/code-server/LimitNumberResultsForDatabaseRequests.md)
- [Minimiser le nombre de requêtes SQL](/code-server/MinimizeNumberSQLRequests.md)
- [Optimiser les conditions d’itération](/code-server/OptimizeIterationConditions.md)
- [Favoriser les pages statiques](/code-server/PreferStaticPages.md)
- [Libérer de la mémoire les variables qui ne sont plus nécessaires](/code-server/ReleaseUnusedVariablesFromMemory.md)
- [Supprimer le code JavaScript redondant](/code-server/RemoveRedundantJS.md)
- [Préciser la colonne de recherche lors des requêtes](/code-server/SpecifySearchFieldInRequests.md)
- [Utiliser tous les niveaux de cache du CMS](/code-server/UseAllCMSCacheLevels.md)
- [Utiliser un système de cache pour l’accès à la base de données](/code-server/UseCacheSystemForDatabaseAccess.md)
- [Utiliser des variables statiques pour prendre en compte le contexte](/code-server/UseStaticVariablesToTakeIntoAccountContext.md)

## Contenu

- [Adapter les sons aux contextes d'écoute](/content/AdaptSoundsToListeningContext.md)
- [Adapter les vidéos aux périphériques de visualisation](/content/AdaptVideosToDevice.md)
- [Mettre en cache le favicon.ico](/content/CacheFaviconFile.md)
- [Dédoublonner systématiquement les fichiers avant envoi](/content/DeduplicateFilesBeforeSending.md)
- [Ne pas redimensionner les images dans le code HTML](/content/DoNotResizeImagesInHTML.md)
- [Encoder les sons en dehors du CMS](/content/EncodeSoundsOutsideCMS.md)
- [Optimiser les images](/content/OptimizeImages.md)
- [Préférer le texte brut au HTML lors de l’envoi des mails](/content/PreferPlainTextToHTMLForMails.md)
- [Redimensionner les images en dehors du CMS](/content/ResizeImagesOutsideCMS.md)
- [Appliquer une alternative textuelle aux images](/content/UseAlternativeTextToImages.md)
- [N'utiliser que des fichiers double opt-in](/content/UseDoubleOptInProcedure.md)

## Design

- [Préférer les CSS aux images](/design/PreferCSSToImages.md)
- [Favoriser une intégration du design sémantique et efficace](/design/PreferSemanticAndEfficientDesignIntegration.md)
- [Favoriser les polices standard](/design/PreferStandardFonts.md)

## Hébergement

- [Ajouter des entêtes Expires ou Cache-Control](/hosting/AddExpiresOrCacheControlHeaders.md)
- [Choisir un hébergeur "vert"](/hosting/ChooseGreenHostingProvider.md)
- [Compresser la sortie HTML, CSS et JS](/hosting/CompressHTMLCSSAndJS.md)
- [Désactiver les modules qui ne sont pas utilisés](/hosting/DeactivateUnusedModules.md)
- [Installer le minimum d'outil et de programme requis sur le serveur](/hosting/InstallOnlyRequiredToolsAndSoftware.md)
- [Minifier les fichiers CSS](/hosting/MinifyCSSFiles.md)
- [Minifier les fichiers JavaScript](/hosting/MinifyJSFiles.md)
- [Optimiser l'efficacité énergétique des serveurs](/hosting/OptimizeServersEnergyEfficiency.md)
- [Préférer Nginx à Apache lorsque c’est possible](/hosting/PreferNginxToApache.md)
- [Regrouper les JavaScript et les CSS](/hosting/RegroupJSAndCSS.md)
- [Supprimer les règles CSS inutilisées](/hosting/RemoveUnusedCSSRules.md)
- [Utiliser une électricité "verte"](/hosting/UseGreenElectricity.md)
- [Utiliser un serveur avec une technologie non bloquante](/hosting/UseNonBlockingServerTechnology.md)
- [Utiliser un reverse proxy](/hosting/UseReverseProxy.md)

## Mesure

- [La taille de la page principale ne doit pas dépasser la taille moyenne des sites du panel WEA (50)](/measure/HomePageSize.md)
- [Nombre d'anomalies ouvertes par rapport à la charge du projet](/measure/NumberDetectedAnomalies.md)
- [Le nombre de requêtes ne doit pas dépasser le nombre moyen des sites du panel WEA (50)](/measure/NumberRequests.md)
- [Utiliser des outils de qualimétrie : dette technique, complexité...](/measure/UseQualityMeasurementTools.md)
- [Le score WEA du site doit être supérieur ou égal à C](/measure/WEAScore.md)
- [Le score WEA ne doit pas dépasser 20% de la valeur lors de l'audit pendant plus de 2 mois](/measure/WEAScoreEvolution.md)
- [Le site doit pouvoir s'afficher sur une plateforme ancienne](/measure/WebsiteCanBeDisplayedOnOlderPlatforms.md)

## Processus

- [Utiliser des outils d'automatisation : TU, TF, IC...](/process/UseAutomationTools.md)
