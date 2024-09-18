Cadastro de Produtos - Arquitetura Hexagonal

Bem-vindo ao projeto MyHexagonalApp! Este é um exemplo de uma aplicação web utilizando ASP.NET Core com uma arquitetura hexagonal e SQLite.

🚀 Como Executar o Projeto
1. Clonar o Repositório
Primeiro, clone o repositório para sua máquina local:

bash
Copiar código
git clone https://github.com/usuario/meu-repositorio.git
cd meu-repositorio

2. Restaurar Pacotes
Restaure os pacotes NuGet para todos os projetos:

bash
Copiar código
dotnet restore
3. Aplicar Migrações
Crie e aplique as migrações para o banco de dados:

bash
Copiar código
dotnet ef migrations add InitialCreate --project Infrastructure --startup-project Api
dotnet ef database update --project Infrastructure --startup-project Api
4. Executar a Aplicação
Inicie a aplicação:

bash
Copiar código
dotnet run --project Api
A aplicação estará disponível em https://localhost:5001 ou http://localhost:5000.

5. Testar a API
Abra o Swagger UI em https://localhost:5001/swagger para testar os endpoints da API.

📁 Estrutura do Projeto
Api: Contém a API Web ASP.NET Core.
Application: Contém a lógica de aplicação e serviços.
Domain: Contém as entidades e interfaces de domínio.
Infrastructure: Contém a implementação de repositórios e o contexto do banco de dados.
🛠️ Tecnologias Usadas
ASP.NET Core
Entity Framework Core
SQLite
Swagger
