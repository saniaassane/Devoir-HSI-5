# Devoir-HSI-5
PROJET : SOUSTRA MONEY - API GATEWAY &
STANDARDISATION
1. Contexte
Soutra Money est une fintech qui travaille avec plusieurs opérateurs mobile money (Orange, MTN,
Moov, Wave). Chaque opérateur possède ses propres API, formats de données et règles de
transaction.
2. Diagnostic des problèmes
Cette diversité crée plusieurs problèmes : intégration longue, erreurs fréquentes, maintenance
difficile et forte dépendance aux développeurs. Chaque modification nécessite des adaptations
multiples.
3. Risques sans harmonisation
Sans standardisation, le système devient instable, difficile à faire évoluer, coûteux et peu fiable.
L’ajout d’un nouvel opérateur devient complexe et lent.
4. Solution proposée : API Gateway
Mettre en place un API Gateway qui sert de point d’entrée unique. Les applications communiquent
uniquement avec ce gateway, qui se charge de traduire les requêtes vers les opérateurs.
5. Architecture simple
Applications → API Gateway → Opérateurs. Cette architecture centralise les échanges et simplifie
les connexions.
6. Standardisation
Définir un format unique pour les transactions (montant, client, opérateur), un identifiant client
unique et un format de réponse standard pour tous les opérateurs.
7. Sécurité
Mettre en place une authentification (API Key), sécuriser les échanges avec HTTPS, valider les
données et surveiller les activités avec des logs.
8. Gestion des erreurs
Prévoir des messages d’erreur clairs, un système de retry automatique et des alertes en cas de
problème.
9. Suivi des performances
Utiliser des outils de monitoring pour suivre les transactions en temps réel et détecter rapidement
les anomalies.
10. Bénéfices
Réduction des erreurs, gain de temps, simplification du système, meilleure maintenance et
possibilité d’ajouter facilement de nouveaux opérateurs.
Conclusion
L’utilisation d’un API Gateway permet d’harmoniser le système de Soutra Money, d’améliorer sa
performance et de faciliter son évolution.
