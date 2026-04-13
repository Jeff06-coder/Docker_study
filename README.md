# Docker_study
## Storing and annotating my studies on Docker (Armazenando e anotando meus estudos no Docker)

### Commands
*whoami / sudo whoami*;

Shows the main user who is logged in/acting
(Mostra o usuário principal que esta logado/atuando)

*pwd*;

Confirm which current folders you are in
(Confirma em quais atuais pastas você está)

*sudo apt update*;

Update the Linux package list
(Atualiza a lista de pacotes do linux)

*cat script_simulator.sh*;

Checks content within the document
(Verifica conteúdo dentro do documento)

*chmod +x script_simulator.sh*;

Giving this permission for execution

*grep "Ok" resultado.txt*;

Looking for documents with this written
(Procurando documentos com isso escrito)

*tail -n 5 file.log*;

Shows the last 5 lines of a file
(Mostra as 5 últimas linhas de um arquivo)

*sudo usermod -aG docker $USER*;

Making docker commands not need to use "sudo" for them to be executed
(Fazendo os comandos do docker não precisem usar o "sudo" para que sejam executados)

*docker pull [image:tag]* | *docker images* | *docker rmi [ID or name:tag]*

Download of image in the docker | Look at the images in your machine | Remove the image 

*docker run -d [image]*

Runs the image/server and leads the terminal to be used: for long processes
(Executa a imagem/servidor e lidera o terminal para ser usado: para processos longos)

*docker run --name [new-name] [image]*

Set new name for image

*docker ps -a*

List all images, until execution stops

*docker inspect [conteiner]*

Returns information about the container (ip, variaveis de ambiente, volumes montados)

*docker container prune*

Deleted all containers stopped

*docker logs -f [conteiner]*

Shows container logs/execution

*docker exec -it [container] /bin/sh*

Access terminal inside the container
(Acessar terminal dentro do contêiner)

*docker run -d --name my-nginx -p 8080:80 nginx:alpine*

Running the container in detached mode, naming it and mapping its port
(Executando o contêiner em modo desanexado, nomeando-o e mapeando sua porta)

*docker volume create database_docker*

You create a space in Docker so that you can store data in it
(Você cria um espaço no Docker para poder armazenar dados nele)

*docker run -d --name the_container -e POSTGRES_PASSWORD=mysecretpassword -v database_docker:/var/lib/postgresql/data postgres:16*

Running the container with the volume, putting Postgres to work in the container, passing the mandatory password, storing it in the mandatory Postgres folders, downloading its image
(Executar o container com o volume, colocar o Postgres para funcionar no container, passar a senha obrigatória, armazenar nas pastas obrigatórias do Postgres, baixar sua imagem)

*docker exec -it the_container psql -U postgres*

Placing the data in the database
(Colocando os dados no banco de dados)

*docker run -d --name dev_nginx -p 8080:80 -v $(pwd):/usr/share/nginx/html nginx:latest*

Bind Mount is running, synchronizing the current folder ($(pwd)) with the nginx docker folder
(Bind Mount está em execução, sincronizando a pasta atual ($(pwd)) com a pasta nginx docker)