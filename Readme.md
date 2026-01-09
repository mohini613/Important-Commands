to list all docker images <docker image>
to delete any image <docker rmi IMAGENAME>
if unable to dlete like container is still on then 
<docker stop containerID>
<docekr rm containerID>
<docker rmi containerID>

when container now starting 
<docker compose down > to stop
<docker compose up -d> to start

to check container status
<docker compose logs --tail-50> last 50 logs

reset everything and start fresh
<docker compose up -d>
<docker compose down -v>

check docker status fedora
<systemctl status docker>

restart docker service 
<sudo systemctl restart docker>