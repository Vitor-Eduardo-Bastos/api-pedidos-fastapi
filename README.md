API de Pedidos com FastAPI
API REST desenvolvida para gerenciamento de usuários, autenticação e pedidos utilizando FastAPI.

Tecnologias utilizadas
Python
FastAPI
SQLAlchemy
Alembic
SQLite
JWT (JSON Web Token)
Passlib (bcrypt)
Pydantic
Funcionalidades
Autenticação
Criação de conta
Login com JWT
Renovação de token
Proteção de rotas com autenticação
Pedidos
Criar pedido
Cancelar pedido
Finalizar pedido
Visualizar pedido
Listar pedidos
Adicionar itens ao pedido
Remover itens do pedido
Controle de acesso
Usuários autenticados
Permissões de administrador
Validação de proprietário do pedido
Estrutura do projeto
api-pedidos-fastapi/
│
├── auth_routes.py
├── dependencies.py
├── main.py
├── models.py
├── order_routes.py
├── schemas.py
│
├── .env.example
├── .gitignore
Instalação
Clone o repositório:

git clone https://github.com/Vitor-Eduardo-Bastos/api-pedidos-fastapi.git
Entre na pasta:

cd api-pedidos-fastapi
Instale as dependências:

pip install -r requirements.txt
Crie um arquivo .env baseado no .env.example:

SECRET_KEY=sua_chave_secreta
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=30
Executando a aplicação
uvicorn main:app --reload
Documentação automática
Swagger:

http://127.0.0.1:8000/docs
Redoc:

http://127.0.0.1:8000/redoc
Aprendizados
Durante o desenvolvimento deste projeto foram praticados conceitos como:

Desenvolvimento de APIs REST
Autenticação JWT
SQLAlchemy ORM
Relacionamentos entre tabelas
Alembic para migrações
Modelagem de banco de dados
Dependency Injection com FastAPI
Organização de projetos Python
