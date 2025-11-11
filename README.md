# Project‑JDBC‑DAO

## 📌 Visão Geral
Este projeto ilustra a utilização de JDBC com MySQL em Java 17, aplicando o padrão DAO (Data Access Object). O objetivo é demonstrar operações CRUD (Create, Read, Update, Delete) num banco de dados relacional, separando a lógica de negócio da camada de persistência.

## 🚀 Tecnologias Utilizadas
- Java 17
- JDBC (Driver MySQL)
- MySQL (ou outro banco relacional compatível)
- Padrão DAO para abstração da camada de acesso a dados
- Arquivo de configuração `db.properties` para parâmetros de conexão
- Estrutura de projeto simples (pacotes `model`, `dao`, `util`, etc)

## 📁 Estrutura do Projeto
```
.idea/  
src/  
  ├─ model/        ← Entidades (por exemplo: Cliente, Produto, etc)  
  ├─ dao/          ← Interfaces e implementações DAO  
  ├─ util/         ← Classe utilitária para conexão JDBC, leitura de properties  
db.properties     ← Configuração da conexão (URL, user, password…)  
.gitignore  
ProjetoJDBC‑DAO.iml
```

## 🔧 Configuração Local
1. Clone o repositório:
   ```bash
   git clone https://github.com/PauloEduardo‑Ferreira/Project‑JDBC‑DAO.git
   ```  
2. Acesse a pasta do projeto:
   ```bash
   cd Project‑JDBC‑DAO
   ```  
3. Configure o banco de dados MySQL:
    - Crie o banco (ex: `jdbc_dao_db`)
    - Crie as tabelas necessárias conforme o modelo do projeto (ex: `tb_cliente`, etc)
    - Insira dados de exemplo se desejar
4. Edite o arquivo `db.properties` com suas credenciais de conexão:
   ```properties
   db.url=jdbc:mysql://localhost:3306/jdbc_dao_db?useSSL=false&serverTimezone=UTC
   db.user=seu_usuario
   db.password=sua_senha
   ```  
5. Compile e execute a aplicação usando seu ambiente/método preferido (IDE, linha de comando, Maven/Gradle se aplicável).
6. Teste as operações CRUD disponíveis.

## ✅ Funcionalidades
- Inserir uma nova entidade (por exemplo: cliente)
- Buscar entidade( s ) por ID ou listar todos
- Atualizar dados de uma entidade existente
- Remover uma entidade por ID
- Encapsulamento de operações de acesso a dados via DAO
- Utilização de Properties para configuração de conexão

## 📄 Licença
Este projeto encontra‑se sob a licença MIT. Sinta‑se à vontade para usar, modificar e distribuir.

## 🧑‍💻 Sobre o Autor
Paulo Eduardo - Desenvolvedor Java.
