# Ambiente de testes!

Disponibiliza-se os arquivos configurados para testes - localhost.

## 1ª Etapa - Infraestrutura

### Sequência de passos 
>1. Habilitar IIS -> Imagens de exemplo.
>2. Instalar os arquivos da pasta dependências.

## 2ª Etapa - Base de dados

### Sequência de passos 
> 1.  Criar banco de dados **sisgp**.
> 2.  Executar o script “1. Criação da estrutura do banco de dados.sql"
> 3.  Executar o script “2. Inserir dados de domínio.sq"
> 4.  Executar o script “3. Inserir dados de teste.sql"
> 5.  Criar o usuário de aplicação **sisgp_con** com permissões de leitura e escrita -> Imagens de exemplo.

### VALIDAÇÃO DA INSTALAÇÃO –1ª ETAPA

Após instalação e configuração da base de dados, recomenda-se a validação da conexão com a base:

> **Insira os dados da conexão no seguinte arquivo:** Arquivo de validação BD

## 3ª Etapa - Aplicação

### Sequência de passos (.NET)

> 1.  Criar um Pool de Aplicativos chamado “sisgp”.
> 2.  Criar um novo site vinculado ao pool “sisgp” e apontando para o caminho físico da pasta “api”.
> 3.  Criar um novo site vinculado ao pool “sisgp” e apontando para o caminho físico da pasta “gateway”.
> 4.  Criar um novo site vinculado ao pool “sisgp” e apontando para o caminho físico da pasta “app”.

## Aplicação

>**Endereço:** http://localhost
	
	> Usuários já configurados no ldap de testes. Senha para todos os usuários: 12345678.
	> usuario.gestor
	> usuario.coordenador
	> usuario.diretor
	> usuario.servidor1
	> usuario.servidor2