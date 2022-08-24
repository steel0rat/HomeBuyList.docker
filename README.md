### Контейнер для развертки HomeBuyList

### команды:
#### поднять контейнер 
sudo docker-compose -f docker-compose.yml up -d

#### поднять контейнер и сбилдить контейнер (при первом запуске)
sudo docker-compose -f docker-compose.yml -f build.yml up -d --build

#### поднять контейнер с локальным репозиторием 
склонировать репозиторий 
https://github.com/steel0rat/HomeBuyList
в путь /var/www/projects/homebuylist

sudo docker-compose -f docker-compose.yml -f build.yml -f dev.yml up -d --build
sudo docker exec -ti homebuylist_api_1 composer install