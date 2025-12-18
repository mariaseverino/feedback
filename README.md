# 💬 Feedback App

Uma plataforma web moderna projetada para facilitar a cultura de feedback dentro de equipes. O sistema permite que colaboradores enviem e recebam feedbacks de forma anônima ou identificada, promovendo um ambiente de transparência e crescimento profissional.

# 🚀 Tecnologias Utilizadas

O projeto utiliza o que há de mais moderno no ecossistema JavaScript para garantir performance e tipagem segura:

-   Frontend: React, Vite, TailwindCSS e TypeScript.

-   Backend: Node.js, Fastify e TypeScript.

-   Autenticação: Better Auth.

-   Banco de Dados: PostgreSQL

# 🛠️ Como Usar

Para rodar o projeto localmente, você precisará ter o Docker e o Docker Compose instalados em sua máquina.

## 1. Clonar os Repositórios

Ambos os repositórios (Frontend e Backend) devem estar no mesmo diretório pai:

```bash
# Clone o Frontend dentro de uma pasta chamada 'front'
git clone https://github.com/mariaseverino/feedback-front front

# Clone a API dentro de uma pasta chamada 'api'
git clone https://github.com/mariaseverino/feedback-api api

```

## 2. Configuração de Variáveis de Ambiente

Na raiz do projeto (ou dentro da pasta da API, conforme sua estrutura), crie um arquivo .env seguindo o exemplo abaixo:

.env.example

```bash
# Autenticação
BETTER_AUTH_SECRET=seu_secret_aqui
BETTER_AUTH_URL=http://localhost:3000

# Banco de Dados
DATABASE_URL=
POSTGRES_USER=
POSTGRES_PASSWORD=
POSTGRES_DB=
```

3. Executar com Docker
   Após configurar os repositórios e o **.env**, navegue até a pasta onde está o arquivo docker-compose.yml e execute:

```
docker-compose up -d
```

O Docker irá subir os containers do banco de dados, do backend e do frontend simultaneamente.
