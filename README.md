# Challenge Spring To-Do List ✅

Aprenda de forma prática as etapas para resolver um desafio real para uma vaga de **Backend Júnior**, utilizando o melhor do **Java** e **Spring Boot**.

Este projeto implementa uma **API REST** para gerenciamento de tarefas (**To-Do List**) com foco em **boas práticas de código**, seguindo princípios de design e arquitetura.

---

## 🚀 Tecnologias e Práticas Utilizadas

- **Java 17+**
- **Spring Boot** (Web, Validation, DevTools)
- **Spring Data JPA**
- **Banco de Dados** (H2 ou substituível por MySQL/PostgreSQL)
- **Swagger / OpenAPI 3** para documentação automática
- **Boas práticas de desenvolvimento**:
  - **SOLID**
  - **DRY** (Don't Repeat Yourself)
  - **YAGNI** (You Aren't Gonna Need It)
  - **KISS** (Keep It Simple, Stupid)

---

## 📌 Funcionalidades

- Criar nova tarefa
- Listar todas as tarefas
- Buscar tarefa por ID
- Atualizar informações de uma tarefa
- Marcar tarefa como concluída
- Deletar tarefa
- Respostas padronizadas de erro

---

## 📂 Estrutura do Projeto

\`\`\`
src/
├── main/
│ ├── java/com/seuusuario/todolist
│ │ ├── controller/ # Endpoints REST
│ │ ├── service/ # Regras de negócio
│ │ ├── model/ # Entidades e DTOs
│ │ └── repository/ # Integração com o banco de dados
│ └── resources/
│ ├── application.properties
│ └── data.sql # Dados iniciais (opcional)
└── test/ # Testes automatizados
\`\`\`

---

## ⚙️ Como Executar o Projeto

1. **Clonar o repositório**
   \`\`\`bash
   git clone https://github.com/Mikael-Kobama/Challenge-spring-todolist.git
   cd Challenge-spring-todolist
   \`\`\`

2. **Rodar a aplicação** (Maven)
   \`\`\`bash
   mvn spring-boot:run
   \`\`\`

3. **Acessar a API**
   - API: [http://localhost:8080](http://localhost:8080)
   - Swagger UI: [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

---

## 📖 Documentação da API

A documentação é gerada automaticamente pelo **Swagger** via **OpenAPI 3**.  
Nela você pode:

- Testar os endpoints
- Visualizar modelos de requisição/resposta
- Conferir códigos de status e parâmetros

---

## 🛠 Exemplos de Requisições

### Criar tarefa

\`\`\`http
POST /tasks
Content-Type: application/json

{
"title": "Estudar Spring Boot",
"description": "Praticar criação de API REST",
"dueDate": "2025-08-15"
}
\`\`\`

### Resposta de sucesso

\`\`\`json
{
"id": 1,
"title": "Estudar Spring Boot",
"description": "Praticar criação de API REST",
"dueDate": "2025-08-15",
"completed": false
}
\`\`\`

---

## 📜 Licença

Este projeto está sob a licença MIT — sinta-se livre para usar e modificar.

---

## 💡 Aprendizados

- Como estruturar uma API REST seguindo boas práticas
- Aplicação de princípios **SOLID** no backend
- Uso do **Spring Data JPA** para consultas simples e complexas
- Documentação interativa com Swagger
- Tratamento padronizado de erros para o cliente
