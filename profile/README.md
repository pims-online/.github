# :rocket: Plan Individuel de Mise en Sûreté (PIMS) dématérialisé

## :tornado: Le PIMS, qu'est-ce que c'est ?

Pour se tenir prêt à faire face aux risques majeurs (inondation, tempête, accident industriel, …), il est important de se préparer. Le PIMS vous propose une méthode simple, accessible à tous en quelques minutes seulement, en renseignant un document synthétique.

Cette infographie papier a été créée par le Bureau de l'Alerte, de la Sensibilisation et de l'Édication des Publics (BASEP - Gouvernement français).

Plus d'information sont disponibles sur [la page officielle du PIMS](https://mobile.interieur.gouv.fr/Le-ministere/Securite-civile/Nos-missions/La-protection-des-personnes-des-biens-et-de-l-environnement/Le-plan-individuel-de-mise-en-surete-PIMS).

## :cloud: La version dématérialisée

Pour que le PIMS soit de plus en plus utilisé et partagé, il a besoin de rentrer dans l'ère du digital d'aujourd'hui.

Le projet de PIMS dématérialisé a pour objectif de démocratiser la génération de PIMS en délivrant une expérience simple, agréable et rapide. En rentrant quelques données importantes sur la plateforme numérique (télé-procédure), les utilisateurs sont capables de générer un PIMS sous format pdf automatiquement complété et adapté à leur situation.

La version de développement peut être testée à l'adresse suivante : <https://pims-frontend.vercel.app>.

## :japanese_castle: Architecture

Le projet numérique de PIMS dématérialisé est construit sur 3 repository Github :

- [pims-frontend](https://github.com/pims-online/pims-frontend) : Application React pour créer l'interface cliente accessible sur le web. Réalisée avec le framework Vite.
- [pims-proxy](https://github.com/pims-online/pims-proxy) : Des fonctions serverless pour opérer en proxy sur certaines requêtes du client pims-frontend.
- [pims-backend](https://github.com/pims-online/pims-backend) : Application Flask pour gérer la génération de PDF dans un environnement d'AWS Lambda function.
