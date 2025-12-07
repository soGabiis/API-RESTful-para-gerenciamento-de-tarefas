# 📝 API RESTful de Gerenciamento de Tarefas

![Java](https://img.shields.io/badge/Java-21-blue)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.2.0-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

API desenvolvida em **Java 21** com **Spring Boot** para gerenciar tarefas, permitindo criar, listar, atualizar e remover tarefas.

---

## 🚀 Tecnologias Utilizadas
- **Java 21**
- **Spring Boot**
- **Spring Data JPA**
- **MySQL**
- **Postman** (para testes)
- **Maven** (para gerenciamento de dependências)

---

## 🏗 Estrutura da API
A entidade principal **Tarefa** possui os seguintes atributos:

| Atributo       | Tipo        | Descrição                    |
|----------------|------------|------------------------------|
| `id`           | Long       | Identificador único          |
| `nome`         | String     | Nome da tarefa               |
| `dataEntrega`  | LocalDate  | Data de entrega da tarefa    |
| `responsavel`  | String     | Pessoa responsável pela tarefa |

---

## 📌 Endpoints

| Método | Endpoint        | Descrição                        |
|--------|----------------|----------------------------------|
| POST   | `/tarefa`       | Criar nova tarefa                |
| GET    | `/tarefa`       | Listar todas as tarefas          |
| PUT    | `/tarefa/{id}`  | Atualizar tarefa pelo ID         |
| DELETE | `/tarefa/{id}`  | Remover tarefa pelo ID           |

### 🔹 Exemplo de requisição POST
```json
{
  "nome": "Desenvolvimento da API",
  "responsavel": "Gabriel Teste",
  "tarefa": "Desenvolver endpoints da API",
  "dataEntrega": "2025-12-12"
}
