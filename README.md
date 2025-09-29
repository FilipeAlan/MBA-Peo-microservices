[![.NET](https://github.com/jonataspc/MBA-Peo-microservices/actions/workflows/dotnet.yml/badge.svg)](https://github.com/jonataspc/MBA-Peo-microservices/actions/workflows/dotnet.yml)

# **PEO - Plataforma de Educa��o Online**

## **Apresenta��o**

Bem-vindo ao reposit�rio do projeto **Peo**. Este projeto � uma entrega do MBA DevXpert Full Stack .NET e � referente ao terceiro m�dulo do MBA Desenvolvedor.IO.

O objetivo principal � desenvolver uma plataforma educacional online com m�ltiplos bounded contexts (BC), aplicando DDD, TDD, CQRS e padr�es arquiteturais para gest�o eficiente de conte�dos educacionais, alunos e processos financeiros. 


### **Autores**
- **Eduardo Gimenes**
- **Filipe Alan Elias**
- **Jonatas Cruz**
- **Joseleno Santos** 
- **Leandro Andreotti** 
- **Paulo Cesar Carneiro**

## **Proposta do Projeto**

O projeto consiste em:

- **API RESTful:** Exposi��o dos endpoints necess�rios para os casos de uso.
- **Autentica��o e Autoriza��o:** Implementa��o de controle de acesso, diferenciando administradores e alunos.
- **Acesso a Dados:** Implementa��o de acesso ao banco de dados atrav�s de ORM.

## **Tecnologias Utilizadas**

- **Linguagem de Programa��o:** C#
- **Frameworks:**
  - ASP.NET Core MVC
  - ASP.NET Core Web API
  - Entity Framework Core
- **Banco de Dados:** SQL Server / SQLite
- **Autentica��o e Autoriza��o:**
  - ASP.NET Core Identity
  - JWT (JSON Web Token) para autentica��o na API
- **Documenta��o da API:** Swagger

## **Estrutura do Projeto**

A estrutura do projeto � organizada da seguinte forma:

- src: c�digos-fonte da solu��o  
- tests: testes de integra��o e de unidade.
- docs: [documenta��o do projeto](./docs/README.md) e requisitos
	
- README.md: Arquivo de Documenta��o do Projeto
- FEEDBACK.md: Arquivo para Consolida��o dos Feedbacks
- DEVELOPMENT.md: Notas de apoio para o desenvolvimento
- .gitignore: Arquivo de Ignora��o do Git
- .gitattributes: Atributos do Git
- .editorconfig: Prefer�ncias de Estilo de C�digo

## **Como Executar o Projeto**

### **Pr�-requisitos**

- .NET SDK 9.0 ou superior
- SQL Server ou SQLite
- Visual Studio 2022 ou superior (ou qualquer IDE de sua prefer�ncia)
- Git

### **Passos para Execu��o**

1. **Clone o Reposit�rio:**
   - `git clone https://github.com/jonataspc/MBA-Peo-microservices.git`
   - `cd MBA-Peo`

2. **Configura��o do Banco de Dados:**
   - No arquivo `\src\Peo.Web.Api\appsettings.json`, configure a string de conex�o do SQL Server.
   - Rode o projeto para que a configura��o do Seed crie o banco e popule com os dados b�sicos


3. **Executar a API:**
   - `cd src\Peo.Web.Api`
   - `dotnet run --launch-profile "https"`
   - Acesse a documenta��o da API em: https://localhost:7113/

## **Instru��es de Configura��o**

- **JWT para API:** As chaves de configura��o do JWT est�o no `\src\Peo.Web.Api\appsettings.json`.
- **Migra��es do Banco de Dados:** As migra��es s�o gerenciadas pelo Entity Framework Core. N�o � necess�rio aplicar manualmente devido a configura��o do seed de dados. 

## **Documenta��o da API**

A documenta��o da API est� dispon�vel atrav�s do Swagger. Ap�s iniciar a API, acesse a documenta��o em https://localhost:7113/

## **Documenta��o do projeto**
Uma documenta��o extensiva pode ser obtida [aqui](./docs/README.md).


## **Code coverage e CI**
A cobertura de c�digo pode ser gerada manualmente/localmente atrav�s do script `\scripts\run-tests-with-coverage.ps1` (que utiliza dotCover) e pode ser visualizada no caminho `\scripts\report.html`. 

No reposit�rio GitHub a action de compila��o executa a compila��o e os testes, al�m de gerar o relat�rio de cobertura de c�digo e armazena-lo como artefato, que pode ser obtido: 
- Acesse a aba "Actions" do reposit�rio.
- Escolha o �ltimo workflow executado.
- Na se��o Artifacts, baixar o arquivo ZIP, contendo o relat�rio em HTML.
 




## **Avalia��o**

- Este projeto � parte de um curso acad�mico e n�o aceita contribui��es externas. 
- Para feedbacks ou d�vidas utilize o recurso de Issues
- O arquivo `FEEDBACK.md` � um resumo das avalia��es do instrutor e dever� ser modificado apenas por ele.
