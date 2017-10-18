# MongoDB - Aula 01 - Exercício

autor: Samuel Fonseca Verneck

## Importando os restaurantes

```sh
samuel@openthecode:~/Documentos/bemean$ mongoimport --db bemean --collection restaurantes --drop restaurantes.json
2017-10-18T18:55:23.457-0200	connected to: localhost
2017-10-18T18:55:23.457-0200	dropping: bemean.restaurantes
2017-10-18T18:55:25.159-0200	imported 25359 documents
```
## Contando os restaurantes

```sh
openthecode(mongod-3.4.4) test> use bemean
switched to db bemean
openthecode(mongod-3.4.4) bemean> db.restaurantes.find({}).count()
25359
```
