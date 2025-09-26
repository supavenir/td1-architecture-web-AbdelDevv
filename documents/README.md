## Titre
Le GET sert à récupérer des donneés et POST sert seulement à envoyer des donneés, exemple de GET car on cherche à avoir des données sur quelque chose https://example.com/api/utilisateur?nom=Jean&age=30 et GET POST https://example.com/api/utilisateur 
| Critère                    | Méthode GET                                       | Méthode POST                                        |
|---------------------------|---------------------------------------------------|-----------------------------------------------------|
| **Visibilité des données**| Visible dans l'URL (paramètres en clair)          | Cachées dans le corps de la requête                 |
| **Idempotence**           | Oui (répétable sans effet secondaire)             | Pas toujours (peut modifier l'état du serveur)      |
| **Mise en cache**         | Oui (souvent mise en cache par navigateurs/proxies)| Rarement mise en cache                             |
| **Longueur utile**        | Limitée (~2048 caractères selon navigateurs/serveurs)| Pratiquement illimitée (dépend du serveur)       |
| **Cas d’usages typiques** | Requêtes de lecture, recherches, navigation       | Soumission de formulaires, envoi de données sensibles |
| **Sécurité (surface)**    | Moins sûre : données exposées dans l’URL, logs, historique | Plus sûre : données non visibles, mieux pour   les données sensibles |


test