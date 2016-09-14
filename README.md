## Démarrage

Pour lancer les containers :

```
# Clone Repository and startup all docker container
git clone https://gitlab.com/jerome.dumas/docker-ci-stack.git
cd docker-ci-stack.git
docker-compose up
```

## Post-installation

```
sudo chown 1000 ~/docker-volumes/jenkins
sudo chown 200 ~/docker-volumes/nexus
```

## Accès aux outils

| *Outils* | *Lien* | *Credentials* |
| ------------- | ------------- | ------------- |
| Jenkins | http://localhost/jenkins | no login required |
| Sonar | http://localhost/sonar | admin/admin |
| Nexus | http://localhost/nexus | admin/admin123 |

> **Attention** : Lors de la première connexion à Jenkins, le mot de passe doit être récupéré depuis les logs.


## Mise à jour des containers

```
# Lancer docker-compose avec une image à jour
docker-compose rm -f
docker-compose pull
docker-compose up --build -d
```
