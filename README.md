### Instalando Docker
#

###### Linux

##### Instale o Docker
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04
##### Instale o Docker Compose
https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-18-04
#
###### Windows
##### Instale Docker + Docker Compose
https://docs.docker.com/docker-for-windows/install/#about-windows-containers
#

##### Ligar Container

    docker-compose up -d

##### Pegar o ip do Container

    docker inspect CONTAINER_NAME | grep '"IPAddress"'

##### Crie um Novo Host
#
###### Linux
Abra o arquivo de hosts
    
    sudo vim /etc/hosts

Em seguida cole o código abaixo, substituindo CONTAINER_IP_HERE pelo ip do container

	CONTAINER_IP_HERE	wordpress-docker.docker
#
###### Windows
- Abra o arquivo: C:\Windows\System32\Drivers\etc\hosts

- Em seguida cole o código abaixo, substituindo CONTAINER_IP_HERE pelo ip do container

	    CONTAINER_IP_HERE	wordpress-docker.docker
- Salve o arquivo

#
##### Acessar Projeto

Abra seu navegador e cole o seguinte endereÃ§o http://wordpress-docker.docker


## Lista de Comandos Docker

###### Ligar container
    docker-compose up -d 
    
###### Desligar container
    docker-compose down
    
###### Listar container ligados
    docker-compose ps
    
###### Listar todos os containers
    docker-compose ps -a

###### Listar todos os containers
    docker inspect containerid
    
###### Remover um container
    docker rmi containerid
    
###### Listar todas as imagens
    docker images
    
###### Remover uma imagem
    docker rmi imageid
