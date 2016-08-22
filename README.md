## Démarrage

Pour lancer les containers :

```
# Clone Repository and startup all docker container
git clone git@gitlab.com:chronolink/chronolink.docker-ci-stack.git
cd chronolink.docker-ci-stack.git
docker-compose up
```

## Post-installation

```
sudo chown 1000 ./jenkins
sudo chown 200 ./nexus
```

## Accès aux outils

| *Outils* | *Lien* | *Credentials* |
| ------------- | ------------- | ------------- |
| Jenkins | http://${docker-machine ip default}:8080/ | no login required |
| SonarQube | http://${docker-machine ip default}:9000/ | admin/admin |
| Nexus | http://${docker-machine ip default}:8081/nexus | admin/admin123 |

> **Attention** : Lors de la première connexion à Jenkins, le mot de passe doit être récupéré depuis les logs.

