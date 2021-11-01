## Conceitos docker
#### Docker Desktop:
É uma interface para trabalhar no terminal.

#### Container
Container é o docker rodando alguma imagem (utiliza da imagem para poder ser executado) - consequentemente executando algum código proposto por ela.
Os containers do docker não tem conexão com nada de fora deles - por isso precisamos expor portas. 

#### Imagem
É o projeto que será executado pelo container, todas as instruções estarão declaradas nela. Programamos uma imagem e a executamos por meio de um container.

------------------------------------

## Trabalhando com Containers
#### sudo docker-compose up -d
#### docker run - rodar container
#### docker run docker/whalesay cowsay
#### docker run it <image> - executar container com interação
docker ps - ver containers rodando
docker ps -a - ver containers executados
docker run -d <image> - executar container em background
docker stop <NAME> - parar o container
docker run -p 3000:80 <image> -expor porta 3000 do pc na porta 80 é a porta que quero receber do container
docker stop <id ou nome> -parando container
docker start <id> - re/iniciar container
flag --name - definir nome do container ex: docker run -d p 80:80  --name <nomeQueQuero>
docker logs <id> - verificar logs
docker -rm <id> - remover container da máquina
docker rm <id>  -f - forçar a remoção do container rodando

 ------------------------------------
## Containers e imagens