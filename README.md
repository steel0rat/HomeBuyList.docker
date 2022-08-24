###Контейнер для развертки HomeBuyList

### команды:
#### поднять контейнер 
sudo docker-compose -f docker-compose.yml up -d

#### поднять контейнер и сбилдить контейнер (при первом запуске)
sudo docker-compose -f docker-compose.yml -f build.yml up -d --build

#### поднять контейнер с локальным репозиторием 
sudo docker-compose -f docker-compose.yml -f build.yml -f dev.yml up -d --build