# DW_editoraSecauth
Integração das apis para mudar os dados da editora com o Cognito através de uma interface de usuário.

## Membors da equipe
Igor Hilgemberg RA: 17162426
Eduardo Patrick RA:17219226
Josmario da Silva Junior RA: 18015526

## Sobre o trabalho

Trabalho realizado para a disciplina de Desenvolvimento Web, que consiste em desenvolver um sistema utilizando o sistema de login Cognito da Amazon, junto com um CRUD e integrando as apis para listar, criar, editar e deletar artigos.

## Pacotes e descrição das apis
### model
*Artigo.java
Os modelos desenvolvidos contém todas as instâncias dos atributos, os setters e os getters para cada atributo, métodos construtores, método ToSring, além de utilizar notações do Spring para determinar regras de Bando de dados, como chaves primárias e estrangeiras, e também o valor lógico de um atributo.

### repository
*ArtigoRepository.java
No repositório de artigo criado, extendemos o Repositório JPA que contém vários métodos para utilizarmos no Controller e além disso pode-se criar novos metódos.

### controllers
*CriarController.java
*DeletarController.java
*EditarController.java
*HomeController.java
*ListarController.java
*SecController.java
Nos controladores criados as regras de negócio do nosso sistema, podendo utilizar os métodos do Repositório ArtigoRepository.java. Essas regras são criação, edição, deleção e listagem de artigos.

#### Funcionalidades
As funcionalidades são de um crud básico: criar, ler, atualizar e excluir.

## Banco de dados
*Foi usado o MYSQL para gravar manter as informações.
*As tabelas do banco de dados são criadas automaticamente ao iniciar a aplicação.
*As configurações do banco de dados se encontram no arquivo application_properties. O comando create-drop foi usado para que as informações não fiquem gravadas no banco após o término da aplicação.

#### Routes
Para conferir se os arquivos estavam sendo armazenados corretamente no banco foi criado o frontend, também podendo verificar esses mesmos dados através do MYSQL Workbench.
