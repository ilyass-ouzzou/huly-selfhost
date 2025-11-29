# Huly — Railway Template (fork pour template)

## But
Ce dépôt est un fork configuré pour être utilisé comme **Railway Template** pour déployer Huly (self-host).

## Quickstart
1. Déployer ce dépôt en tant que Template sur Railway (ou créer un projet depuis ce template).
2. Remplir les variables requises : `HULY_VERSION`, `MINIO_ROOT_USER`, `MINIO_ROOT_PASSWORD`, `SECRET`.
3. Recommandation : **2 vCPU / 4 GB RAM minimum**. Elasticsearch nécessite plus de RAM.

## Variables requises (Railway)
- HULY_VERSION
- MINIO_ROOT_USER
- MINIO_ROOT_PASSWORD
- SECRET
- HOST_ADDRESS (optionnel)
- OPENAI_API_KEY (optionnel)
- LIVEKIT_API_KEY / LIVEKIT_API_SECRET (optionnel)

## Post-deploy
- Attendre que tous les services soient prêts.
- Ouvrir l'URL du service `front`.
- Créer le premier compte et tester upload de fichier.

## Remarques
Testé localement avec `docker compose up`. Si Elasticsearch plante, augmente la RAM ou désactive la recherche.
