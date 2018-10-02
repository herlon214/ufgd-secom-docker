# Tweet App

### Preparando host
Abra o arquivo de hosts para inserirmos um novo dominio.
```
$ sudo vim /etc/hosts
```

Insira o dominio `tweetapp.ufgd` apontando para `127.0.0.1`

```
# ... configurações atuais do arquivo
127.0.0.1 tweetapp.ufgd
```


### Build
```
$ docker build . -t ufgd/tweetapp
```

### Deploy de stack
```
$ docker stack deploy tweet --compose-file=service.yml
```

### Atualizando stack
```
$ docker stack deploy tweet --compose-file=service.yml
```