```shell
docker compose --profile download up --build
# wait until its done, then:
docker compose --profile [ui] up --build
# where [ui] is one of: invoke | auto | auto-cpu | comfy | comfy-cpu

sudo yum install docker-ce
sudo yum install docker-compose-plugin
docker compose version
sudo docker compose --profile download up --build
sudo docker compose --profile auto up --build
```
