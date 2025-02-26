# Template projet CI/CD : k8s-angular

Ce repo contient le template d'une application développé avec **php**.

## Comment utiliser ce template ?

### Faire un fork du  template

Faite un clique sur le bouton frok pour créer botre repo.

### Déploiements du code source

Les sources du projet sont à déposer dans le repertoire **src**.

Les sources des valeurs ainsi que des services et les ingress ce trouve dans le dossier **charts**

### C'est quoi un helm charts ?

Les Helm Charts sont des packages pour déployer des applications sur Kubernetes. Ils contiennent tous les fichiers de configuration nécessaires pour exécuter une application ou un service dans un cluster Kubernetes.

### Déploiement dans le dossier racine

Pour mettre le deploiement du build dans à la racine du dossier dist, il suffit de retrirer le nom du projet ainsi que le / après dist dans le fichier **angular.json** pour la propriété **outputPath**


### Créer les différentes branches du projet :

Par convention, nous utilisons deux branches la branche `master`ou`main`

Exemple: 

```bash
git checkout -b master
git push -u origin master
```

```bash
git checkout -b main
git push -u origin main

### Cronjob, sidecar, env, ingress, exposer les metrics a travers un plugin prometheus
