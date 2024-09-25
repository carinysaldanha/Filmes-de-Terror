# Filmes-de-Terror
Projeto de Banco de Dados de Filmes de Terror
Este projeto consiste em um banco de dados relacional que armazena informações sobre filmes de terror, incluindo detalhes sobre os filmes, diretores, atores, gêneros e mortes nos filmes. O objetivo é criar um sistema organizado para armazenar e consultar dados relevantes sobre filmes de terror.

## Estrutura do Banco de Dados
O banco de dados é composto pelas seguintes tabelas:

### 1. Filmes
id_filme (INT, chave primária): Identificador único do filme.
titulo (VARCHAR(100), não nulo): Título do filme.
ano (INT, não nulo): Ano de lançamento do filme.
id_diretor (INT, chave estrangeira): Referência ao diretor do filme.
id_genero (INT, chave estrangeira): Referência ao gênero do filme.
### 2. Diretores
id_diretor (INT, chave primária): Identificador único do diretor.
nome (VARCHAR(100), não nulo): Nome do diretor.
data_nascimento (DATE): Data de nascimento do diretor.
### 3. Atores
id_ator (INT, chave primária): Identificador único do ator.
nome (VARCHAR(100), não nulo): Nome do ator.
data_nascimento (DATE): Data de nascimento do ator.
### 4. Gêneros
id_genero (INT, chave primária): Identificador único do gênero.
nome (VARCHAR(100), não nulo): Nome do gênero.
### 5. Ator_Filme
id_ator (INT, chave primária, chave estrangeira): Referência ao ator.
id_filme (INT, chave primária, chave estrangeira): Referência ao filme.
### 6. Mortes
id_morte (INT, chave primária): Identificador único da morte.
id_filme (INT, chave estrangeira): Referência ao filme.
numero_mortes (INT, não nulo): Número de mortes retratadas no filme.
## Funcionalidades
Adicionar novos filmes, diretores, atores e gêneros ao banco de dados.
Consultar informações sobre filmes, diretores, atores e suas relações.
Analisar dados sobre o número de mortes em filmes de terror ao longo dos anos.
Tecnologias Utilizadas
SGBD: MySQL (ou outro sistema de banco de dados relacional).
Linguagem SQL: Para a manipulação de dados e estruturação do banco de dados.
Instruções para Configuração

bash
Copiar código
git clone <url-do-repositório>
cd <diretório-do-repositório>
Configurar o Banco de Dados

Crie um novo banco de dados no MySQL.
Execute os scripts SQL fornecidos para criar as tabelas e relacionamentos.
Inserir Dados

Utilize scripts SQL para inserir dados de exemplo nas tabelas.
Consultar Dados

Execute consultas SQL para extrair informações e realizar análises.
Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir um pull request ou relatar problemas.

Licença
Este projeto está sob a Licença MIT.

