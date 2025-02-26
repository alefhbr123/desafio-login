# Desafio Login - Fidelity Pesquisas Cadastrais

## Sobre o Projeto
Este projeto implementa uma aplicação Django com as funcionalidades de **Login** e **Registrar** conforme os requisitos do desafio técnico da Fidelity Pesquisas Cadastrais.

## 🚀Tecnologias Utilizadas
- ``Python``
- ``Django``
- ``SQLite``
- ``HTML``
- ``CSS``
- ``JavaScript``

## Funcionalidades
- Tela de Login:
  - Validação de e-mail e senha.
  - Tratamento de erros específicos ("E-mail inexistente" e "Senha inválida").
  - Redirecionamento para a tela de Menu após login.
- Tela de Registrar:
  - Formulário com campos: nome, e-mail, senha e confirmar senha.
  - Validações:
    - Nome aceita apenas letras.
    - E-mail deve conter “@”.
    - Senha com no mínimo 8 caracteres, 1 caractere especial, 1 número e 1 letra maiúscula.
    - Confirmação de senha idêntica.
  - Botão para alternar a visualização dos campos de senha.
  - Botões "Registrar" e "Cancelar" (este último redireciona para a tela de Login).
- Extra:
  - Envio de e-mail de confirmação (necessário configurar o backend de e-mail).

  ## 📌Estrutura do Repositório
desafio-login/                     # Diretório raiz do projeto
├── README.md                     # Documentação e instruções do projeto
├── .gitignore                    # Arquivo para ignorar arquivos/pastas no Git
├── manage.py                     # Script de gerenciamento do Django
├── projeto_login/                # Diretório do projeto (configurações gerais)
│   ├── __init__.py
│   ├── settings.py               # Configurações do projeto (inclui STATIC_URL, EMAIL_BACKEND etc.)
│   ├── urls.py                   # URLs globais do projeto
│   ├── wsgi.py                   # Configuração do servidor WSGI
│   └── asgi.py                   # (Opcional) Configuração do servidor ASGI
└── app_projeto_login/            # Seu app principal
    ├── __init__.py
    ├── admin.py                  # Registro de modelos no admin
    ├── apps.py                   # Configuração do app
    ├── forms.py                  # Formulários (LoginForm, RegisterForm, etc.)
    ├── models.py                 # Modelos (se houver, ou pode ficar vazio)
    ├── tests.py                  # Testes do app
    ├── urls.py                   # URLs específicas do app
    ├── views.py                  # Views (login_view, register_view, menu_view, etc.)
    ├── migrations/               # Diretório das migrações do banco de dados
    │   └── __init__.py
    ├── templates/                # Templates do app
    │   └── accounts/             # Templates relacionados às contas de usuário
    │       ├── login.html        # Template da tela de login
    │       ├── register.html     # Template da tela de registro
    │       └── menu.html         # Template da tela de menu
    └── static/                   # Arquivos estáticos do app
        └── app_projeto_login/    # Organiza os arquivos estáticos por app
            └── style.css         # Arquivo CSS para o projeto
