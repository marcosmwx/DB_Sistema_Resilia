# DATABASE_Sistema_Resilia

## Proposta do projeto

### Realizar a tarefa de modelagem de Dados do novo sistema de acompanhamento da Resilia, recebi as seguintes instruções e perguntas:

Modelar um banco de dados que vai armazenar seus cursos, turmas e alunos.

⇨ Existem outras entidades além dessas três?
⇨ Quais são os principais campos e tipos?
⇨ Como essas entidades estão relacionadas?

## Respostas

### ⇨ Existem outras entidades além dessas três?

* Sim foi adicionado algumas entendidades que faz sentido ter em um sistema de Banco de Dados de uma instituiçao de ensino, sendo elas: 
Matricula, Disciplinas, Area, Turma e Professor

### ⇨ Quais são os principais campos e tipos?

* id_aluno, curso_id, turma_id sao do tipo Int PK
* nome ( em geral) Varchar ( com varios tamanhos diferentes para cada caso)


### ⇨ Como essas entidades estão relacionadas?

* CURSO estao relacionados a DISCIPLINA no tipo (1:N)
* CURSO esta relacionado a ALUNO no tipo (N:N), Esta relacao faz nos termos uma nova entidade MATRICULA que esta ligada a CURSO e ALUNO
* ALUNO esta relacionado a TURMA, Um aluno pode ter mais de uma turma e uma Turma pode ter mais de Um Aluno, Relacao do tipo (N:N)
* TURMA esta relacionado a professor no tipo (N:N) 
* TURMA esta relacionado a DISCIPLINA do tipo (1:N) A disciplina pode haver apenas uma TURMA
* DISCIPLINA esta relacionado a AREA do tipo (1,N) (Esta entidade foi criada visando uma possivel adicao de novos cursos e também para definir os tipos de cursos por pesquisa, Uma Area pode ter varias disciplinas)


## Requisitos Extras
⇨ Preparar os scripts que vão criar o banco de dados proposto e adicionar uma pasta chamada SQL com os arquivos.

## PRINT do Modelo
 ![schemadbresilia](https://user-images.githubusercontent.com/87791042/212911722-84d0582e-9bf0-43e7-b541-940ee1bd3f08.png)

