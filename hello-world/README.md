# Nginx App

### Preparando host
Abra o arquivo de hosts para inserirmos um novo dominio.
```
$ sudo vim /etc/hosts
```

Insira o dominio `hello.ufgd` apontando para `127.0.0.1`

```
# ... configurações atuais do arquivo
127.0.0.1 hello.ufgd
```


### Build
```
$ docker build . -t ufgd/hello
```

### Deploy de stack
```
$ docker stack deploy hello --compose-file=service.yml
```

### Atualizando stack
```
$ docker stack deploy hello --compose-file=service.yml
```