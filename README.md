# Atelier Cluster Redis — Tom Frégonese

<br>

### Prérequis :
- Docker et docker-compose installés 
- npm installé 
- Accès à internet

<br>

## - Partie 1: Installation et Configuration du Cluster Redis

... :

This guy is pretty cool https://selftuts.in/install-redis-using-docker-compose/

```bash 
docker compose up -d
```

```bash 
docker exec -it redis1 bash -c "echo -e 'port 6379\ncluster-enabled yes\ncluster-config-file nodes.conf\ncluster-node-timeout 5000\nappendonly yes\n' > /tmp/redis.conf && redis-server /tmp/redis.conf"
docker exec -it redis2 bash -c "echo -e 'port 6379\ncluster-enabled yes\ncluster-config-file nodes.conf\ncluster-node-timeout 5000\nappendonly yes\n' > /tmp/redis.conf && redis-server /tmp/redis.conf"
docker exec -it redis3 bash -c "echo -e 'port 6379\ncluster-enabled yes\ncluster-config-file nodes.conf\ncluster-node-timeout 5000\nappendonly yes\n' > /tmp/redis.conf && redis-server /tmp/redis.conf"
```

```bash 
docker exec -it redis1 redis-cli --cluster create 127.0.0.1:6379 127.0.0.1:6380 127.0.0.1:6381 --cluster-replicas 0
```

<br>

## - Partie 2: Premiers Pas avec le Cluster Redis 

... :

```bash
npm install
npm run ...
```
<br>

## - Partie 3: Intégration de Redis dans un Projet

... 

<br>

## - Partie 4: Introspection sur l'Intégration de Redis

... 
