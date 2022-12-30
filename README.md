# Visualiseur des données

Widget de prévisualisation des données issues de fichiers csv

---

## Résumé

Afin de pouvoir partager et de mettre en valeur toutes les ressources de ce repo il a été proposé de créer un outil numérique de type "widget" : `datami`. En effet un outil de ce type permet de pouvoir intégrer sur des sites tiers (sites de partenaires ou autres) une sélection plus ou moins large de ressources. Cette solution permet à la fois d'éviter aux sites partenaires de "copier-coller" les ressources, d'afficher sur ces sites tiers les ressources toujours à jour, et de permettre aux sites tiers ainsi qu'au site source de gagner en visibilité, en légitimité et en qualité d'information.

L'autre avantage de cette solution est qu'elle n'est déployée qu'une fois, mais que le widget peut être intégré et paramétré/personnalisé sur autant de sites tiers que l'on souhaite... gratuitement.

La solution proposée et réalisée ici s'appuie sur un projet open source porté par la coopérative numérique [**multi**](https://multi.coop) : le projet [Datami](https://datami.multi.coop).

---

## Démo

- Page html de démo : [![Netlify Status](https://api.netlify.com/api/v1/badges/ac24c6a6-9abd-4e5a-bdcb-688c525840aa/deploy-status)](https://app.netlify.com/sites/datami-demo-ping-tiers-lieux/deploys)
- url de démo : https://

---

## Pour aller plus loin

### Datami

Le widget fait partie intégrante du projet [Datami](https://gitlab.com/multi-coop/datami)

### Documentation technique

Un site dédié à la doucmentation technique de Datami est consultable ici : https://datami-docs.multi.coop

---

## Mini server for local development

A mini server is writen in the `server.py` to serve this folder's files.

To install the mini-server :

```sh
pip install --upgrade pip
python3 -m pip install --user virtualenv
python3 -m venv venv
source venv/bin/activate
pip install --upgrade pip
pip install -r requirements.txt
```

or

```sh
sh setup.sh
source venv/bin/activate
```

---

### Run local server

To run the server on `http://localhost:8800`:

```sh
python server.py
```

or

```sh
sh run_server.sh
```

Files will be locally served on :

- `http://localhost:8800/content/<path:folder_path>/<string:filename>`
- `http://localhost:8800/statics/<path:folder_path>/<string:filename>`

---

## Crédits

| | logo | url |
| :-: | :-: | :-: |
| **PiNG** | ![TERNUM](./images/mednumbfc-logo-1.png) | https://ternum-bfc.fr |
| **coopérative numérique multi** | ![multi](./images/multi-logo.png) | https://multi.coop |
