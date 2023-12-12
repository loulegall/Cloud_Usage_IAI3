# Projet Cloud
## Description
Vous allez mettre en œuvre les différentes notions vues au travers des TP pour déployer une
application sous forme de containers docker, dans une infrastructure virtualisée également déployer
par vos soins sur la plateforme de TP OpenStack.
Afin de rendre le déploiment de cette application pertinent dans une infrastructure de type cloud,
cette application devra se composer d’un frontend et d’un backend.

## Ajouter la Stack à OpenStack
1. Dans OpenStack, aller dans le menu "Orchestration" puis "Stacks" et cliquer sur "Launch Stack".
2. Dans le champ "Template URL", mettre l'URL du fichier "ProjetCloud-RU-LLG.yaml" du projet.
3. Dans le champ "Environment Source", mettre l'URL du fichier "ProjetCloud-RU-LLG-env.yaml" du projet.
4. Cliquer sur "Next".
5. Dans le champ "Stack Name", mettre le nom de la stack.
6. Dans le champ "Password", mettre le mot de passe de l'utilisateur.
7. Cliquer sur "Launch".
## Connexion SSH aux VMs
### VM1
```ssh user1@IP_EXT_VM1```
### VM2
```ssh user2@IP_EXT_VM2```

## Accéder aux fichiers des VMs
```ls -la /```

## Vérification du bon fonctionnement de la stack
Faire un  ```docker ps``` sur les deux VMs pour vérifier que les conteneurs sont bien lancés.