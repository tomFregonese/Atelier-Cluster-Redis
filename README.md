# Atelier Cluster Redis — Tom Frégonese

<br>

### Prérequis :
- Docker et docker-compose installés 
- Accès à internet

<br>

## - Partie 1: Installation et Configuration du Cluster Redis

Dans ce TP on utilisera Redis via des conteneurs Docker. Pour les lancer, il faut exécuter la commande suivante :

```bash 
docker compose up -d
```

<br>

## - Partie 2: Premiers Pas avec le Cluster Redis 

Pour interagir avec Redis, on doit d'abord nous connecter à l'un des conteneurs avec la commande :

```bash
docker exec -it redis1 redis-cli
```

Maintenant que l'on est connecté à l'interface en lignes de commandes redis, on peut tester les commandes de base de la manière suivante : 

```bash
SET greeting "Hello world!"
LPUSH cars "Audi R8" "Audi TT"
SADD colors "red" "green" "blue"
HMSET user:tom_fregonese username "tom" password "password" email "tom.fregonese@ynov.com"
ZADD leaderboard 100 "user1" 200 "user2" 300 "user3"
```

On vient ici d'enregister dans la base : 
    - un string contenant du texte ;
    - une liste contenant des éléments ordonnés par insertion ;
    - une collection contenant des éléments non ordonnés ;
    - un hash contenant un ensemble de clés/valeurs pour representer un objet.  

```bash
GET greeting
LRANGE cars 0 -1
SMEMBERS colors
HGETALL user:john_doe
ZRANGE leaderboard 0 -1 WITHSCORES
```

<br>

## - Partie 3: Intégration de Redis dans un Projet

... 

<br>

## - Partie 4: Introspection sur l'Intégration de Redis

... 
