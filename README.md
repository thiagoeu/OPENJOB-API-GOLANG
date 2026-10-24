# ⚡ OpenJob API — High Performance Job Management

[![Go](https://img.shields.io/badge/Go-1.2x-00ADD8?style=for-the-badge&logo=go&logoColor=white)](https://go.dev/)
[![Gin](https://img.shields.io/badge/Gin-Web_Framework-008ECF?style=for-the-badge&logo=go&logoColor=white)](https://gin-gonic.com/)
[![GORM](https://img.shields.io/badge/GORM-ORM-blue?style=for-the-badge)](https://gorm.io/)
[![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)

API RESTful concorrente e de alta performance desenvolvida em **Go (Golang)** para cadastro, consulta e gerenciamento de vagas de emprego. Construída com o framework **Gin** e persistência via **GORM**.

---

## 🚀 Funcionalidades

- **CRUD Completo de Oportunidades:** Cadastro, listagem, atualização e remoção de vagas.
- **Roteamento Ultrarrápido:** Construído sobre o engine HTTP do Gin.
- **Camada ORM Fluente:** Mapeamento de dados e migrações automáticas com GORM.
- **Tratamento Estruturado de Erros:** Respostas padronizadas em JSON com validações de campos.

---

## 🛠️ Stack Tecnológica

- **Linguagem:** Go (Golang)
- **Framework Web:** [Gin Web Framework](https://github.com/gin-gonic/gin)
- **Persistência / ORM:** [GORM](https://gorm.io/)
- **Database:** SQLite / PostgreSQL
- **Validação de Schemas:** Gin Binding & Validation

---

## 📦 Como Rodar o Projeto

### Pré-requisitos
- [Go 1.20+](https://go.dev/dl/) instalado na máquina.

### Passo a Passo

```bash
# 1. Clonar o repositório
git clone https://github.com/thiagoeu/OPENJOB-API-GOLANG.git
cd OPENJOB-API-GOLANG

# 2. Baixar dependências
go mod tidy

# 3. Executar o servidor
go run main.go
```

A API estará disponível em: `http://localhost:8080`

---

## 🛣️ Endpoints da API

| Método | Endpoint | Descrição |
| :--- | :--- | :--- |
| `GET` | `/api/v1/jobs` | Retorna a listagem de todas as vagas cadastradas |
| `GET` | `/api/v1/job?id={id}` | Detalhes de uma vaga específica |
| `POST` | `/api/v1/job` | Cadastra uma nova vaga de trabalho |
| `PUT` | `/api/v1/job?id={id}` | Atualiza dados de uma vaga existente |
| `DELETE` | `/api/v1/job?id={id}` | Remove uma vaga do sistema |

### Exemplo de Payload (`POST /api/v1/job`)

```json
{
  "role": "Senior Go Engineer",
  "company": "Tech Corp",
  "location": "Remoto (Brasil)",
  "remote": true,
  "link": "https://company.com/careers/go-engineer",
  "salary": 16000
}
```

---

## 📄 Licença
Distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.
