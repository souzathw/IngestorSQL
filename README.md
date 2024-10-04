# InjetorSQL
# Injetor de dados para PostgreSQL

Este projeto é um injetor de dados aleatórios em um banco de dados PostgreSQL. Ele gera dados fictícios para tabelas de `Customers`, `Products`, e `Orders`, útil para ambientes de desenvolvimento e testes. Dados aleatórios são gerados utilizando a biblioteca [Faker](https://faker.readthedocs.io/), enquanto as variáveis de ambiente e a conexão com o banco são configuradas com [dotenv](https://pypi.org/project/python-dotenv/).

Ele tem como finalidade popular um banco de dados a fim de testes, semelhante a um seeder no php.

## Tabelas Criadas

- **Customers**: Contém dados de clientes (nome e email).
- **Products**: Lista de produtos com nome, categoria e preço.
- **Orders**: Registra pedidos, com referências a clientes e produtos, quantidade, total, e status do pedido.

### Estrutura das Tabelas
- **Customers**: `id`, `name`, `email`
- **Products**: `id`, `name`, `category`, `price`
- **Orders**: `id`, `customer_id`, `product_id`, `quantity`, `total`, `status`

## Pré-requisitos

- **Python 3.x**
- **PostgreSQL**
- **Bibliotecas Python**: instale com `pip install -r requirements.txt`

### Instalando dependências

```bash
pip install psycopg2 faker python-dotenv



