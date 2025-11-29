# Mapping template variables → Huly env

HULY_VERSION -> image tags: hardcoreeng/account:${HULY_VERSION}, hardcoreeng/front:${HULY_VERSION}, ...
MINIO_ROOT_USER -> MINIO_ROOT_USER (minio service)
MINIO_ROOT_PASSWORD -> MINIO_ROOT_PASSWORD (minio service)
SECRET -> SERVER_SECRET (account/transactor/front)
MONGO_URL -> mongodb://mongo:27017
ELASTIC_URL -> http://elasticsearch:9200

Notes:
- Utiliser les noms de services Railway (ex: mongo, minio, account) comme hôtes dans les URLs.
- Laisser l'utilisateur remplir OPENAI / LIVEKIT si nécessaire.
