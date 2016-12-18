#Iniciando com banco de dados!
______________________________

###Criando o banco de dados

```javascript
create database wallmart
```

###Criando a tabela jogos

```javascript
create table jogos (
	id INT(10) AUTO_INCREMENT PRIMARY KEY,
	nome VARCHAR(100) NOT NULL,
	genero VARCHAR(50) NOT NULL,
	preco DECIMAL(10.2) NOT NULL,
	plataforma VARCHAR(50) NOT NULL);
```
	
###Inserindo os dados na tabela jogos

```javascript
INSERT INTO jogos VALUES(NULL,'God of War','Ação',199.00,'Playstation 3'),
(NULL,'Skyrim','RPG',130.00,'XBOX, PS4, PC'),
(NULL,'Halo','Ação',199.00,'XBOX 360'),
(NULL,'Forza','Corrida',129.00,'XBOX ONE'),
(NULL,'Gran Turismo','Corrida',180.00,'PS4'),
(NULL,'Crash N sane Trilogy','Aventura',199.00,'PS4'),
(NULL,'Final Fantasy XV','RPG',199.00,'XBOX ONE,PS4'),
(NULL,'Playboy the Mansion','Pegadinha',110.00,'PC'),
(NULL,'Counter Strike GO','Tiro',25.00,'PC'),
(NULL,'Left 4 Dead 2','Tiro',10.00,'PC');
```
============================================================

###Criando a tabela remedios

```javascript
create table remedios (
	id INT(10) AUTO_INCREMENT PRIMARY KEY,
	nome VARCHAR(100) NOT NULL,
	laboratorio VARCHAR(50) NOT NULL,
	preco DECIMAL(10.2) NOT NULL,
	generico VARCHAR(2) NOT NULL);
```

###Inserindo os dados na tabela remedios

```javascript
 INSERT INTO remedios  VALUES(NULL,'Berotec','WW Industries',33.00,'N'),
    (NULL,'Besectasil','WW Industries',10.00,'N'),
    (NULL,'Remedio pra Fimose','WW Industries',50.00,'N'),
    (NULL,'Dipirona','WW Industries',5.00,'S'),
    (NULL,'Coristina D','WW Industries',33.00,'N'),
    (NULL,'Busonid','WW Industries',33.00,'S'),
    (NULL,'Soro Fisiologico','WW Industries',33.00,'N'),
    (NULL,'AAS','WW Industries',07.00,'S'),
    (NULL,'Eno Guaraná','WW Industries',35.00,'S'),
    (NULL,'Gardenal','WW Industries',22.00,'N');
```
===========================================================

###Verificando os dados

```javascript
SELECT * FROM jogos;
```

###Resultado da query

```javascript
+----+----------------------+-----------+-------+---------------+
| id | nome                 | genero    | preco | plataforma    |
+----+----------------------+-----------+-------+---------------+
|  1 | God of War           | Ação      |   199 | Playstation 3 |
|  2 | Skyrim               | RPG       |   130 | XBOX, PS4, PC |
|  3 | Halo                 | Ação      |   199 | XBOX 360      |
|  4 | Forza                | Corrida   |   129 | XBOX ONE      |
|  5 | Gran Turismo         | Corrida   |   180 | PS4           |
|  6 | Crash N sane Trilogy | Aventura  |   199 | PS4           |
|  7 | Final Fantasy XV     | RPG       |   199 | XBOX ONE,PS4  |
|  8 | Playboy the Mansion  | Pegadinha |   110 | PC            |
|  9 | Counter Strike GO    | Tiro      |    25 | PC            |
| 10 | Left 4 Dead 2        | Tiro      |    10 | PC            |
+----+----------------------+-----------+-------+---------------+
10 rows in set (0,00 sec)
```
____________________________________________________________

```javascript
SELECT * FROM remedios;
```

###Resultado da query

```javascript
+----+--------------------+---------------+-------+----------+
| id | nome               | laboratorio   | preco | generico |
+----+--------------------+---------------+-------+----------+
|  1 | Berotec            | WW Industries |    33 | N        |
|  2 | Besectasil         | WW Industries |    10 | N        |
|  3 | Remedio pra Fimose | WW Industries |    50 | N        |
|  4 | Dipirona           | WW Industries |     5 | S        |
|  5 | Coristina D        | WW Industries |    33 | N        |
|  6 | Busonid            | WW Industries |    33 | S        |
|  7 | Soro Fisiologico   | WW Industries |    33 | N        |
|  8 | AAS                | WW Industries |     7 | S        |
|  9 | Eno Guaraná        | WW Industries |    35 | S        |
| 10 | Gardenal           | WW Industries |    22 | N        |
+----+--------------------+---------------+-------+----------+
10 rows in set (0,00 sec)
```
