# sql_consultas

select * from [cursos].curso

INSERT INTO [cursos].curso (id, ativo, fechado, nome, data_inicio, data_termino, carga_horaria, id_categoria, id_modalidade, id_cidade, pontuacao_cfc, mostrar_pontuacao, codigo_cfc, publico_alvo, objetivo)
VALUES (1, 1, 0, 'Curso para teste', '2023-08-03', '2024-08-10', 40, 2, 1, 5, 20, 1, 'ABC123', 'teste modailidade', 'Aprender teste');


SELECT * from ead_aulas

EXEC [Cursos].[Buscar.Cursos] 1, 100, NULL, NULL


SELECT ordem, imagem, link, texto_card FROM [Cursos].[Banner]

INSERT INTO Cursos.Banner (ordem, imagem, link, texto_card)
VALUES (4, 'https://www.cursoslefisc.com.br/banners/banner_curso_04.svg', '#', '')

ALTER TABLE [Cursos].[Banner]
ADD titulo_card VARCHAR(180);

SELECT * FROM [Cursos].[Banner]


ALTER TABLE [Cursos].[Banner]
ALTER COLUMN titulo_card NVARCHAR(180);

DELETE FROM [Cursos].[Banner]
WHERE id = 5;

UPDATE [Cursos].[Banner]
SET titulo_card = 'ACOMPANHE NOSSA AGENDA SEMANAL! RECEBA CONDIÇÕES ESPECIAIS NO NOSSO WHATSAPP!'
WHERE id = 4;

UPDATE [Cursos].[Banner]
SET titulo_card = 'VOCÊ CONHECE O YOUTUBE DA LEFISC?'
WHERE id = 3;

UPDATE [Cursos].[Banner]
SET titulo_card = 'ACOMPANHE NOSSA AGENDA SEMANAL! RECEBA CONDIÇÕES ESPECIAIS NO NOSSO WHATSAPP!'
WHERE id = 1;

UPDATE [Cursos].[Banner]
SET titulo_card = 'GARANTA SUA PONTUAÇÃO NO PROGRAMA DE EDUÇÃO CONTINUADA'
WHERE id = 2;

UPDATE [Cursos].[Banner]
SET titulo_card = 'Na LEFISC você pode completar sua pontuação do PEPC sem sair de casa. Oferecemos cursos que pontuam até 40 pontos em diversas áreas.'
WHERE id = 2;

UPDATE [Cursos].[Banner]
SET titulo_card = 'GARANTA SUA PONTUAÇÃO NO PROGRAMA DE EDUÇÃO CONTINUADA'
WHERE id = 2;

UPDATE [Cursos].[Banner]
SET titulo_card = 'CURSOS ESPECIALIZANTES FEITOS SOB MEDIDA PARA SUA EMPRESA'
WHERE id = 4;

SELECT * FROM [Cursos].[Banner]
