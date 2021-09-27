# conversao-peso

## Docker Build

```bash
docker image build -t roanfranklin/conversaopeso:v1 .
```

## Docker Run

```bash
docker run -d -p 8080:8080 --rm --name conversaopeso roanfranklin/conversaopeso:v1
```

## INFORMAÇÕES

### error:

```bash
[roanfranklin@zatanna conversao-peso]$ docker build -t roanfranklin/conversaopeso:v1 .
error checking context: 'syntax error in pattern'.
```

Ainda estou trabalhando nisso!