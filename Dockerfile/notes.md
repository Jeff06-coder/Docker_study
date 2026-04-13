## FROM
Sets the base image

## WORKDIR
Sets the working directory inside the container

## COPY
Copy files from host to container

## RUN
Execute commands during build

## CMD
Sets the default command when running the container

# Build and Analysis Layers
Control your own image and analyze it
(Constroi sua propria imagem e analisa ela)

### docker build -t nameSet-app:v1
Builds on top of the commands placed in the Dockerfile
(Constroi encima dos comandos colocados no Dockerfile)

### docker history nameSet-app:v1
Inspect image layers
(Inspecione camadas da imagem)

### docker run --rm nameSer=t-app:v1
Running the conteiner and remove after stopped

### docker images | grep nameSet-app
Comparing existing images with each other
(Comparando as imagens existentes com a outra)

## && \
Add to the RUN structure if you wanted to execute more than one terminal code while executing the Dockerfile
(Adicione à estrutura RUN se você quiser executar mais de um código de terminal enquanto executa o Dockerfile)