Exercice 1: Accès aux logs

1.1 Créez un nouveau Pod à partir du fichier suivant

k apply -f webapp.yaml

1.2 Observez les logs de webapp et découvrez pourquoi l’utilisateur USER5 n’arrive pas à se connecter

C'est parce que le USER5 a tenté de se connecter à plusieurs reprises sans succès et le compte est donc bloqué

1.3  Pourquoi l’utilisateur USER7 n’arrive pas à passer commande ? 

C'est parce que le produit que il commande n'est pas en stock

Exercrice 2: Limitation des ressources

2.1  Créez un nouveau Pod via le manifeste suivant que vous écrirez dans le fichier stress.yaml

k apply -f stress.yaml

2.2 Inspectez l’état de votre Pod, dans quel état se trouve-t-il ? Quelle en est la raison ?

Le pod est en état de waiting à cause d'un CrashLoopBackOff. Ca veut dire qu'il est en attente de redémarrge continu  



