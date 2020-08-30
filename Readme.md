Step 1: start the mongo databases

docker-compose up
or
docker-compose up -d

Step 2: basic secuirty steps

openssl rand -base64 700 > file.key
chmod 400 file.key

Step 3 : docker exec mongo-0 /scripts/setup.sh

Step 4 : try to use the single node connection in robo3t on port loalhost:27017 with admin auth database.
