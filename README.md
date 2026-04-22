Sistema de Gestão de Vendas

Descrição:
Sistema web para gerenciamento de clientes, produtos e vendas. Permite controle de estoque, registro de transações e geração de relatórios, utilizando arquitetura em camadas, API REST e interface web em Django.

Tecnologias Utilizadas
* Python
* Django
* Django REST Framework
* SQLite ou MySQL
* JWT (autenticação)

Arquitetura
O sistema segue o padrão de arquitetura em camadas:

* Apresentação: interface web (Django)
* API REST: comunicação via JSON
* Negócio: regras do sistema
* Dados: persistência no banco de dados

 Segurança
* Autenticação via token JWT
* Proteção de rotas
* Controle de acesso por perfil (ADMIN, FUNCIONARIO)

Funcionalidades

Clientes
* Cadastro, listagem e atualização
* CPF único
* Validação de email

Produtos
* Cadastro e controle de estoque
* Preço não pode ser negativo
* Bloqueio de venda sem estoque

Vendas
* Registro de vendas com múltiplos itens
* Cálculo automático do valor total
* Atualização de estoque

 Relatórios
* Vendas por período
* Vendas por cliente

API REST

Autenticação:
POST /auth/login
Retorna token JWT

Endpoints:
GET /clientes
GET /produtos
GET /vendas

Banco de Dados

Tabelas principais:
* usuarios
* clientes
* produtos
* vendas
* itens_venda

/src
/docs
/database
README.md


Documentação:
Os diagramas e documentos estão disponíveis na pasta /docs

Alunos:
Marina Borel
Lucas Flores
Gabriel Guedes
Marcos Vinicius
