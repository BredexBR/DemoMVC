# Iniciando ASP.NET MVC
Este reposit�rio tem como objetivo servir como um ponto de partida para quem deseja aprender 
e aplicar os principais conceitos do ASP.NET MVC, incluindo pr�ticas essenciais como Razor Pages,
Blazor e Web API. Ao longo deste projeto, exploraremos como o padr�o MVC (Model-View-Controller) pode 
ser implementado na pr�tica, abordando a constru��o de interfaces din�micas e interativas com Razor 
Pages, al�m de entender o poder do Blazor para aplica��es web modernas. Tamb�m veremos como criar e 
consumir APIs robustas usando ASP.NET Web API, tornando este reposit�rio uma base s�lida para o 
desenvolvimento de aplica��es web completas.

<br>

![Execu��o1](imgs/inicial.png)

<br>

## Criando uma Controller
Para criar uma controller a partir de um model nova criada(exemplo aluno.cs):
1. Clique com o bot�o direito do mouse na pasta "Controllers" -> add -> new scaffolded item... -> MV controller 
with views - using entity Framework.
2. Ap�s isso selecione a model criada(nesse exemplo Aluno.cs)
3. Utilize a data do projeto utilizado
4. O nome da controler
5. Sera gerado o AlunosController.cs na pasta Controllers
6. Tambem sera criado o "CRUD" de alunos na Pasta Views

## Configurando o banco de dados ap�s inclus�o da Model
- Sera necess�rio rodar no terminal(Package Manager Console) o comando 
para fazer as migra��es da model Aluno:
	```bash
	Add migration Aluno

- E posteriormente para atualizar o banco de dados:
	```bash
	update-database