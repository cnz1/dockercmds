Raderar alla stoppade containers från systemet
```md
docker container prune
```
Raderar alla oanvända volymer
```md
docker volume prune
```
StandoutScript
```md
 bin/setup_docker_compose
```
Startar containers i bakgrunden(detached)
```md
 docker compose up -d
```
Stoppar och tar bort containers etc, för att sedan starta upp dem igen i detachedmode
```md
docker compose down && docker compose up -d
```
Stoppar och tar bort containers etc, bygger sedan om containers och startar upp dem igen i detachedmode
```md
docker compose down && docker compose build && docker compose up -d
```
Raderar oanvända data inklusive containers, nätverk, images (både hängande och oanvända), samt alla oanvända volymer.
```md
docker system prune --volumes
```
 listar alla miljövariabler i containern
```md
docker compose exec web env
```
Visar en lista över alla körande containers, inklusive information som container-id, image, skapelsestatus, och portar.
```md
docker ps
```
Kör rails console i en interaktiv terminal inuti en specifik container. 
```md
docker exec -it <container_namm_eller_id> rails console
```
