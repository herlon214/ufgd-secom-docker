# Swarm Visualizer

### Preparando host
Abra o arquivo de hosts para inserirmos um novo dominio.
```
$ sudo vim /etc/hosts
```

Insira o dominio `visualizer.ufgd` apontando para `127.0.0.1`

```
# ... configurações atuais do arquivo
127.0.0.1 visualizer.ufgd
```

### Deploy de stack
```
$ docker stack deploy visualizer --compose-file=service.yml
```

### Atualizando stack
```
$ docker stack deploy visualizer --compose-file=service.yml
```