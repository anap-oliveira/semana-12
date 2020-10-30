Exercicio

## Resumo da Semana sobre MongoDB e Banco de Dados 


## Banco de Dados:
 É uma coleção organizada de informações armazenadas em um sistema. 



## Entidades: 
 São as abstrações da vida real que são colocadas no sistema para alguma finalidade.



## Atributos: 
São caracteristicas que formam uma entidade. 



## SGDB: 
Sistemas de Gerenciamento de Banco de Dados s]ao softwares utilizados para gerir as estrutiras de armazenamento de dados, permitem manipulações, bem como controlar as permissões de utilização dos bancos de dados.

Exemplos: MongoDB, MySQL, SQL Server, PostgreSQL


## Diferença de um BD SQL e NoSQL:

SQL: É do tipo relacional estruturado em tabelas (linhas e colunas) pode-se manipular dados, tais como atualizar, adicionar, remover, etc). Uma de suas vantangens é a integridade de dados. 


NoSQL: São do tipo não relacional, estruturado com tipagem dinâmica onde sua estrutura é formada de acordo com sua utilização.



## MONGODB: É do tipo NoSQL, orientado a objetos (documentos), sistema open-source, e BSON. 

Os documentos são formados por registros similares a estrutura Json.

As collections é um conjunto de documentos.

Banco de Dados: É um conjunto de coleções.



Nota 1: Assim que você começar a trabalhar no terminal e digitar este comando, este será o banco de dados que você estará acessando. Você só mudará de banco se digitar o comando novamente com o nome de outro banco. mas, caso tenha dúvidas, só usar o próximo comando.

Nota 2: No ambiente  de trabalho de uma máquina Windows é necessário abrir dois terminais de Prompt de Comando, no primeiro você iniciará o servidor, digitando o comando mongod. N segundo, terminal você digitará apenas o comando mongo e, é neste terminal que você fará suas configurações de documentos.


## Principais Comandos 

## Para criar um banco de dados novo 
use nomeDoBanco



## Mostrar o banco de dados atual 
db.current

## Listar todos os bancos de dados
show databases

## Para criar uma coleção
db.createCollection("collectionNomedaColeção")


## Listar todas as coleções
show collections

## Para buscar todos os registros de uma coleção
db.nomeDaColeção.find() //comando retorna uma espécie de array de objetos.


## Para retornar apenas um registro
db.nomeDaCollection.findOne()

## Para incluir o registro dentro de uma coleção
db.nomeDaCollection.insertOne({Atributos}) //atributos são escritos como a notação de objetos e chaves de um JSON.


## Para incluir vários registros
db.nomeDaCollection.insertMany()

## Apagar uma coleção
db.collection.drop()

## Remover um banco de dados
db.dropDatabase()

Atenção: Não é recomendado remover um banco de dados, pois contém diversas coleções ecom esse comando todas serão excluídas.

## Comando para retornar a coleção com o formato mais legível, do tipo JSON
db.nomeDaColeção.find().pretty()








