# desafio-minimal-api

Projeto desenvolvido para o desafio da trilha .NET da Digital Innovation One (DIO).

## Descrição

API mínima em .NET 9 para gerenciamento de tarefas. Permite cadastro, consulta, edição e remoção de tarefas com filtragem por título, data e status.

## Funcionalidades

- Criar nova tarefa
- Consultar tarefa pelo ID
- Atualizar tarefa pelo ID
- Remover tarefa pelo ID
- Listar todas as tarefas
- Filtrar tarefas por título, data ou status

## Tecnologias Utilizadas

- .NET 9 Minimal API
- Entity Framework Core
- SQL Server (ou outro banco relacional)
- Swagger para documentação

## Endpoints

| Método | Endpoint               | Descrição                      |
|--------|------------------------|-------------------------------|
| GET    | /Tarefa/{id}           | Obter tarefa por ID           |
| GET    | /Tarefa/ObterTodos     | Listar todas as tarefas       |
| GET    | /Tarefa/ObterPorTitulo | Consultar tarefas por título  |
| GET    | /Tarefa/ObterPorData   | Consultar tarefas por data    |
| GET    | /Tarefa/ObterPorStatus | Consultar tarefas por status  |
| POST   | /Tarefa                | Criar nova tarefa             |
| PUT    | /Tarefa/{id}           | Atualizar tarefa por ID       |
| DELETE | /Tarefa/{id}           | Remover tarefa por ID         |

## Como executar

1. Clone o repositório:

git clone https://github.com/GustavoMimoso/desafio-minimal-api.git

text

2. Acesse a pasta do projeto:

cd desafio-minimal-api

text

3. Restaure as dependências:

dotnet restore

text

4. Atualize o banco de dados com as migrações:

dotnet ef database update

text

5. Execute o projeto:

dotnet run

text

6. Acesse a documentação interativa via Swagger em:

https://localhost:<porta>/swagger

text

## Modelo de Tarefa (JSON)

{
"id": 0,
"titulo": "string",
"descricao": "string",
"data": "yyyy-MM-ddTHH:mm:ss",
"status": "Pendente"
}

text
