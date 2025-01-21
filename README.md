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

