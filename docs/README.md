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
sudo docker compose --profile auto-cpu up --build

sudo docker tag 4a6987588fa1 yiluxiangbei/stable-diffusion-webui-docker:v1
sudo docker push yiluxiangbei/stable-diffusion-webui-docker:v1

wget --cut-dirs=5 -nH -r --no-parent --reject "index.html*" https://the-eye.eu/public/AI/models/GPT-NeoX-20B/full_weights/ -P 20B_checkpoints
wget --no-check-certificate --cut-dirs=5 -nH -r --no-parent --reject "index.html*" https://the-eye.eu/public/AI/models/GPT-NeoX-20B/full_weights/ -P 20B_checkpoints

docker rmi `docker images|grep none |  awk '{print $3}'`
```
