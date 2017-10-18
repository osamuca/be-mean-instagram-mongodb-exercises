# MongoDB - Aula 01 - Exercício

autor: Samuel Fonseca Verneck

## Importando os restaurantes

```sh
samuel@openthecode:~/Documentos/bemean$ mongoimport --db bemean --collection restaurantes --drop date.json
2017-10-18T18:29:27.242-0200	connected to: localhost
2017-10-18T18:29:27.242-0200	dropping: bemean.restaurantes
2017-10-18T18:29:27.499-0200	[........................] bemean.restaurantes	0B/11.3MB (0.0%)
2017-10-18T18:29:30.499-0200	[#.......................] bemean.restaurantes	537KB/11.3MB (4.6%)
2017-10-18T18:29:33.499-0200	[##......................] bemean.restaurantes	1.26MB/11.3MB (11.1%)
2017-10-18T18:29:36.499-0200	[##############..........] bemean.restaurantes	6.81MB/11.3MB (60.1%)
2017-10-18T18:29:37.708-0200	[########################] bemean.restaurantes	11.3MB/11.3MB (100.0%)
2017-10-18T18:29:37.713-0200	imported 25359 documents

```
## Contando os restaurantes

```sh
openthecode(mongod-3.4.4) test> use bemean
switched to db bemean
openthecode(mongod-3.4.4) bemean> db.restaurantes.find({}).count()
25359
```