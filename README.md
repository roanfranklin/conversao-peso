# conversao-peso

## Docker Build

```bash
docker image build -t roanfranklin/conversaopeso:v1 .
```

## Docker Run

```bash
docker run -d -p 8080:80 --rm --name conversaopeso roanfranklin/conversaopeso:v1
```

## INFORMAÇÕES

### error:

```bash
[roanfranklin@zatanna conversao-peso]$ docker build -t roanfranklin/conversaopeso:v1 .
error checking context: 'syntax error in pattern'.
```

Ainda estou trabalhando nisso!

### resolution:

tinha encontrado uma ajuda de como criar o Dockerfile para aplicações dotNET em [Docs Microsoft - ASPNET+Docker](https://docs.microsoft.com/pt-br/aspnet/core/host-and-deploy/docker/building-net-docker-images?view=aspnetcore-5.0), poremtinha criado o .dockerignore e tinha adicionar o "bin\" e "obj\", por isso não estava funcionando. Ao comentar essas 2 linhas/dir o build funcionou 100% e a aplicação rodou beleza!