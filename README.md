# Docker

## Anotações

Executar uma imagem do docker. Caso não exista localmente, ele tenta buscar no Docker Hub.
```docker
docker run hello-world
```

Lista containers em execução no momento.
```docker
docker ps
```

Lista todos containers inclusive parados.
```docker
docker ps -a
```

Inicia um container com a imagem do ubuntu e executa o comando fornecido.
```docker
docker run ubuntu echo "Olá Mundo"
```

Inicia o container em modo interativo.
```docker
docker run -it ubuntu
```
Inicia um container parado.
```docker
docker start f20ddb50fe3d
```

Para um container em execução.
```docker
docker stop f20ddb50fe3d
```

Inicia um container em modo interativo.
```docker
docker start -ai f20ddb50fe3d
```

Apaga um container parado.
```docker
docker start -ai f20ddb50fe3d
```

Apaga todos containers parados.
```docker
docker container prune
```

Lista imagens baixadas.
```docker
docker images
```

Apaga uma imagem.
```docker
docker rmi 405f6ec369dd
```

Inicia o container em background
```docker
docker run -d dockersamples/static-site
```

Associa portas do computador com as portas utilizadas pelos serviços rodando no container.
```docker
docker run -d -P dockersamples/static-site
```

Lista as portas em uso por um container.
```docker
docker port 30594b7d54ab
```

Cria um container especificado um nome para ele.
```docker
docker run -d -P --name meu-site dockersamples/static-site
```

Define manualmente a associação de portas do computador com o do container.
```docker
docker run -d -p 12345:80 dockersamples/static-site
```

Inicia o container criando uma variavel de ambiente.
```docker
docker run -d -P -e AUTHOR="Caique Portela" dockersamples/static-site
```

Listar apenas IDs.
```docker
docker ps -q
```

Parar todos containers em execução.
```docker
docker stop $(docker ps -q)
```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```

```docker

```
