# Sobre o projeto Jogoteca

O projeto Jogoteca foi desenvolvido durante o estudo do curso de Flask 1 e 2 da Alura.
Nele o usuário poderá adicionar, editar ou excluir um jogo de sua lista.

# Ferramentas usadas

- Python3
- Flask
- Flask_MySQLdb
- MySQL
- Html
- Bootstrap
- JavaScript

# Navegando no Projeto

### Página Inical

A página mostra uma lista de jogos que vem por padrão do banco de dados e as opções de novo, editar e deletar um
jogo.

### Novo Jogo

Existe três campos de texto para preencher e a incluisão de uma capa de jogo.

![novo_jogo](https://user-images.githubusercontent.com/87434197/153781031-440ad680-65ce-4680-aa94-52a196052df4.gif)

### Editar

Semelhante ao Novo Jogo, nesse caso, o usuário poderá modificar um jogo da lista.

![editando](https://user-images.githubusercontent.com/87434197/153780932-285ca62f-1dc6-40fd-bbeb-d4e96c609dd1.gif)

### Deletar

Apenas exclui o jogo removendo do Banco de Dados e consequentemente da lista.

### Logando

Para ir direto à página de login basta acessar o link: http://127.0.0.1:5000/login

![logando](https://user-images.githubusercontent.com/87434197/153781275-20e42bc8-2d68-4239-a968-a19df316ba69.gif)

Se você clicar em DELETAR, NOVO OU EDITAR, será solicitado que você faça acesso para realizar as operações.

Por padrão o acesso é:

- Usuário: admin
- Senha: admin

### Deslogando

Para deslogar você terá que usar o link: http://127.0.0.1:5000/logout

![deslogando](https://user-images.githubusercontent.com/87434197/153781204-4b31cd5e-173f-409e-bdd9-a469b3864e9e.gif)

# Sobre alguns arquivos

### Arquivo prepara_banco.py

Basicamente o arquivo prepara o banco de dados criando:

- Banco jogoteca;
- As tabela `usuário` e `jogo` com suas colunas respectivamente;
- Dados nas tabelas.

E por fim fecha a conexão.

OBS: É importante que este arquivo esteja de acordo com a configuração de conexão ao banco que será usado.
Vale lembrar que o arquivo `config.py` também tem que ser configurado.

### Arquivo dao.py

É um padrão de objeto utilizado para isolar os códigos relacionados à lógica do banco de dados e o código da aplicação.
Servindo assim para acessar os dados do banco.

