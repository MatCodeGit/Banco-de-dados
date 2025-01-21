# Banco-de-dados

Create database Banco_de_dados;

CREATE TABLE nomes (
	id int IDENTITY (1,1) Primary key, 
	nome varchar (50),
	data_nascimento date,
	email varchar(50)
	);

ALTER TABLE nomes
	ADD 
	telefone varchar(50),
	estado varchar (10);

DROP TABLE nomes;

INSERT INTO nomes (nome, data_nascimento, email)

VALUES ('Matheus', '2000-03-03','matheus@gmail.com'),
	   ('Lucas','1993-05-22','lucas@gmail.com'),
	   ('Aline', '1990-09-11','aline@gmail.com');

UPDATE nomes
SET telefone = '1258243248', estado = 'RJ'
WHERE nome = 'Aline';

SELECT nome, estado 
FROM nomes
ORDER BY nome;


INSERT INTO nomes (nome, data_nascimento, email, telefone, estado)

VALUES ('Adriano', '2001','adriano@gmail.com','1125346897','MG'),
	   ('Gabriel','1998-05-12','gabriel@gmail.com','1235486795','RJ'),
	   ('Maria', '2002-09-13','maria@gmail.com','1196654231','SP');


SELECT *
FROM nomes;

Create table Cargos (
	id int identity(1,1) primary key,
	nome varchar(50),
	salario decimal(10,2)
	);
 
select * from Cargos;
