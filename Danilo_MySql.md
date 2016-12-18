## Database
create database dpsp;
show databases;

## Criando tabela
create table jogos (id int(10), nome varchar(50), tipo varchar(50), valor decimal(6,2), plataforma varchar(50));
create table remedios (id int(10), nome varchar(50), tipo varchar(50), genero varchar(50), valor decimal(6,2));
show tables;

## Inserindo jogos

insert into jogos values (1, 'Crash Bandicoot', 'Aventura', 27.99, 'Playstation');
insert into jogos values (2, 'Crash Bandicoot 2', 'Aventura', 26.99, 'Playstation');
insert into jogos values (4, 'Crash CTR', 'corrida', 25.99, 'Playstation');
insert into jogos values (3, 'Crash Bandicoot 3', 'Aventura', 29.99, 'Playstation');
insert into jogos values (5, 'Crash Bash', 'Aventura', 22.99, 'Playstation');
insert into jogos values (6, 'PES', 'Futebol', 30.00, 'Playstation');
insert into jogos values (7, 'FIFA', 'Futebol', 20.99, 'Playstation');
insert into jogos values (8, 'Call of Duty black ops 1', 'Tiro', 20.99, 'Playstation');
insert into jogos values (9, 'Call of Duty black ops 2', 'Tiro', 20.99, 'Playstation');
insert into jogos values (10, 'Call of Duty black ops 3', 'Tiro', 20.99, 'Playstation');

## Inserindo remedios

insert into remedios values (11, 'Resfenol', 'anti-gripal', 'referencia', 15.00);
insert into remedios values (11, 'Benegrip', 'anti-gripal', 'referencia', 10.00);
insert into remedios values (11, 'cimegrip', 'anti-gripal', 'similar', 5.00);
insert into remedios values (11, 'Dorflex', 'antiinflamatorio', 'referencia', 9.99);
insert into remedios values (11, 'Salonpas', 'antiinflamatorio', 'referencia', 8.48);
insert into remedios values (11, 'Tandrilax', 'antiinflamatorio', 'referencia', 22.63);
insert into remedios values (11, 'Naproxeno', 'antiinflamatorio', 'generico', 7.99);
insert into remedios values (11, 'Eno', 'azia', 'referencia', 3.89);
insert into remedios values (11, 'Gastrol', 'azia', 'similar', 4.08);
insert into remedios values (11, 'Engov', 'ressaca', 'referencia', 4.76);
## Selecionando as tabelas jogos e remedios

select * from jogos;
+------+--------------------------+----------+-------+-------------+
| id   | nome                     | tipo     | valor | plataforma  |
+------+--------------------------+----------+-------+-------------+
|    1 | Crash Bandicoot          | Aventura | 20.00 | Playstation |
|    2 | Crash Bandicoot 2        | Aventura | 26.99 | Playstation |
|    3 | Crash Bandicoot 3        | Aventura | 29.99 | Playstation |
|    3 | Crash Bandicoot 3        | Aventura | 29.99 | Playstation |
|    5 | Crash Bash               | Aventura | 22.99 | Playstation |
|    6 | PES                      | Futebol  | 30.00 | Playstation |
|    7 | FIFA                     | Futebol  | 20.99 | Playstation |
|    8 | Call of Duty black ops 1 | Tiro     | 20.99 | Playstation |
|    9 | Call of Duty black ops 2 | Tiro     | 20.99 | Playstation |
|   10 | Call of Duty black ops 3 | Tiro     | 20.99 | Playstation |
+------+--------------------------+----------+-------+-------------+

select * from remedios;
+------+-----------+------------------+------------+-------+
| id   | nome      | tipo             | genero     | valor |
+------+-----------+------------------+------------+-------+
|   11 | Resfenol  | anti-gripal      | referencia | 15.00 |
|   11 | Benegrip  | anti-gripal      | referencia | 10.00 |
|   11 | cimegrip  | anti-gripal      | similar    |  5.00 |
|   11 | Dorflex   | antiinflamatorio | referencia |  9.99 |
|   11 | Salonpas  | antiinflamatorio | referencia |  8.48 |
|   11 | Tandrilax | antiinflamatorio | referencia | 22.63 |
|   11 | Naproxeno | antiinflamatorio | generico   |  7.99 |
|   11 | Eno       | azia             | referencia |  3.89 |
|   11 | Gastrol   | azia             | similar    |  4.08 |
|   11 | Engov     | ressaca          | referencia |  4.76 |
+------+-----------+------------------+------------+-------+