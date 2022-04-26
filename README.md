# SysWSB - Sistema de Venda de Veículos

## Tecnologias:

- Linguagem PHP
- Banco de dados MySQL
- Bootstrap para estilizar as páginas

## Estrutura do projeto:

`index.php`: Arquivo principal que contém o layout da aplicação e é responsável por abrir as páginas internas de cada funcionalidade de acordo com o parâmetro passado na URL.

`\db`: Nesta pasta está o arquivo `conexao.php`, responsável por acessar o banco de dados.

`\paginas`: Nesta pasta há uma subpasta para cada cadastro do sistema (carros, cores, clientes, etc), contendo as páginas para cada operação do CRUD de cada item. Em cada subpasta existem os seguintes arquivos:

- `listagem.php`: Página de listagem de cada item o sistema. 
- `cadastro.php`: Página com o formulário de cadastro do item. Essa página contém um form que envia os dados para o arquivo `cadastrar.php` equivalente dentro da pasta `funcoes`.
- `edicao.php`: Página com o formulário de edição do item. Quando acessamos essa página os dados já vêm preenchidos a partir do código passado na URL. Essa página contém um form que envia os dados para o arquivo `editar.php` equivalente na pasta `funcoes`.
- `exclusao.php`: Página para confirmar a exclusão de um item. Essa página contém um form com um campo que envia apenas o código do item para o arquivo `excluir.php` equivalente na pasta `funcoes`.

`\assets`: Aqui estão os arquivos CSS e JavaScript do Bootstrap, necessários para estilizar as páginas e fazer o menu funcionar.
