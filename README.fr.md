# NoMore

**Rendre les progrès visibles. Avancer sans culpabiliser.**

[English presentation](README.md) · [Feuille de route](ROADMAP.md) · [Architecture envisagée](ARCHITECTURE.md) · [Contribuer](CONTRIBUTING.md)

NoMore est un projet en phase initiale visant à créer une plateforme multilingue, avec un accès gratuit, consacrée à **l’auto-suivi, à la motivation et à l’orientation vers des ressources adaptées** pour les personnes préoccupées par leurs conduites addictives.

L’ordre de développement retenu est **l’alcool, puis le tabac, puis les jeux d’argent**.

## État actuel

Ce dépôt présente le projet, son périmètre et ses exigences de développement. Il ne fournit **pas encore une application NoMore installable**, un service d’accompagnement opérationnel ou une intervention dont l’efficacité clinique aurait été validée.

Les fonctionnalités décrites ci-dessous sont **prévues**, et non présentées comme développées ou vérifiées. Le projet ne revendique ni communauté d’utilisateurs établie, ni chiffres d’adoption, ni certification de sécurité, ni efficacité médicale démontrée.

Les éléments du projet NoMore publiés dans ce dépôt sont placés sous **GNU Affero General Public License, version 3 uniquement (AGPL-3.0-only)**, sous réserve des notices distinctes des composants tiers. Le texte complet figure dans [LICENSE](LICENSE) et les précisions de périmètre dans [LICENSING.md](LICENSING.md). La mise sous licence de cette documentation ne signifie pas qu’une application a déjà été développée ou livrée.

## Intention du projet

L’objectif est de rendre compréhensibles les évolutions des habitudes personnelles, sans réduire le parcours à un compteur de réussite ou d’échec.

Un journal quotidien privé, des graphiques lisibles et des comparaisons financières explicites doivent aider à observer les changements. L’interface doit permettre de reprendre après une journée difficile, sans jugement, classement entre utilisateurs ou effacement des progrès antérieurs.

NoMore a vocation à compléter l’accès à un accompagnement professionnel, sans s’y substituer.

## Premiers modules envisagés

| Ordre | Module | Périmètre prévu |
| --- | --- | --- |
| 1 | Alcool | Consommation déclarée, tendances personnelles, estimations de dépenses, notes facultatives et ressources d’aide adaptées au pays. Aucun programme automatique de sevrage. |
| 2 | Tabac | Consommation déclarée, comparaison avec une référence personnelle, estimations financières explicites et synthèses de progression. |
| 3 | Jeux d’argent | Dépenses déclarées, temps passé, envies et objectifs personnels, avec ressources d’aide. Aucun conseil de pari, aucune promotion du jeu, aucune promesse de récupération des pertes. |

Le socle commun doit prévoir un compte personnel, une saisie quotidienne courte, un tableau de bord accessible, des objectifs choisis par l’utilisateur, l’export et la suppression des données, ainsi qu’une administration des contenus, traductions et ressources validés.

Une journée non renseignée ne doit jamais être confondue avec une journée sans consommation ou sans jeu. Les estimations financières doivent préciser leurs hypothèses et ne pas être présentées comme des économies effectivement réalisées sans éléments suffisants.

## Dimension internationale

Le français, l’anglais et l’espagnol sont les premières langues d’interface prévues. Les autres langues constituent un objectif ultérieur, et non des versions déjà disponibles.

La langue et le pays doivent être des réglages distincts. Les devises, dates, fuseaux horaires, unités de mesure et ressources d’aide nécessitent une localisation adaptée. Les contenus de sécurité doivent être relus, et non uniquement traduits automatiquement.

L’ambition est internationale ; une disponibilité effective dans tous les pays n’est pas encore annoncée.

## Confidentialité et sécurité : exigences de conception

La conception envisagée repose sur la minimisation des données, le recours possible à un pseudonyme, la limitation des accès administratifs et la maîtrise des données par l’utilisateur.

Aucune donnée personnelle réelle, aucun identifiant secret, aucune copie de base de données et aucune configuration privée ne doivent être publiés dans ce dépôt. Les exemples et tests doivent employer des données fictives clairement identifiées.

NoMore n’a pas vocation à diagnostiquer, prescrire, calculer une espérance de vie individuelle ou recommander un sevrage non encadré. Les formulations relatives à la santé et les ressources d’orientation doivent faire l’objet d’une relecture qualifiée avant ouverture au public.

Aucun traceur publicitaire, enregistrement de session ou dispositif de prospection comportementale n’est prévu dans les espaces personnels de suivi.

Ces éléments sont des exigences de développement, et non une déclaration de conformité, de certification ou de mise en œuvre déjà achevée.

## Orientation technique envisagée

Le socle proposé est une application PHP structurée, une base MySQL/MariaDB, du HTML sémantique, du CSS moderne et du JavaScript léger.

Les objectifs sont une interface responsive et accessible, un déploiement documenté et une maintenance compréhensible. Les mécanismes de sécurité doivent s’appuyer sur des solutions maintenues et éprouvées, sans cryptographie inventée.

Le document [ARCHITECTURE.md](ARCHITECTURE.md) expose cette proposition et les décisions restant à prendre.

## Développement ouvert

Les premiers échanges peuvent porter sur les besoins, l’accessibilité, la localisation, la documentation et les exigences de confidentialité ou de sécurité. Les contributions au code devront ensuite suivre un périmètre, des tests et des critères de revue documentés.

Les modalités figurent dans [CONTRIBUTING.md](CONTRIBUTING.md) et les précautions de signalement dans [SECURITY.md](SECURITY.md).

## Porteur du projet

Projet initié par **Xavier**, avec le compte GitHub **XavierNTZ**.

Les échanges publics de ce dépôt ne doivent pas contenir d’histoires médicales personnelles ni de demandes urgentes d’assistance. Ce dépôt est un espace de développement logiciel, et non un service de soins ou d’urgence.
