# Projet Challenge - README

Ce projet a été créé pour le défi Pull Request, Tag, Workflow Dispatch, et un schedule.

## Étape 1: Fork et Configuration Initiale

- Tout d'abord, j'ai créé du le repo du défi : [https://github.com/sameddemet/challenge-s10-e02/tree/demo](https://github.com/sameddemet/challenge-s10-e02/tree/demo).
- Ensuite, sur le repo, j'ai créé un script Python (`hello_world.py`) et un fichier `requirements.txt`.

## Étape 2: Création du Workflow

- J'ai créé un fichier de workflow GitHub Actions `.github/workflows/main.yml`.
- Le workflow inclut les déclencheurs Pull Request, Tag, Workflow Dispatch et Scheduled.

## Étape 3: Test du Workflow

- J'ai créé une branche `demo` et j'ai testé le déclencheur Pull Request en créant une pull request.
- J'ai testé le déclencheur Tag en ajoutant une étiquette (v1.1) à mon dépôt et en vérifiant le déclenchement du workflow.
```
git tag -a v1.1 -m "Release v1.1"
git push origin v1.1
```

- J'ai déclenché manuellement le workflow via l'interface GitHub en utilisant le Workflow Dispatch.

---
## Diffucuilties 
Le main.yml, basé sur l'événement workflow_dispatch, n'est même pas affiché pendant que le code n'est pas sur la branche main (ou branche par défaut).
Une fois que j'ai fait merge demo avec la branche main, workflow_dispatch foncionne.