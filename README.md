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
## 📦​Instalação
## 1. Clonar o Repositório

Abra o terminal e execute os comandos abaixo:

```bash
git clone https://github.com/alefhbr123/desafio-login.git
cd desafio-login
```
## 2. Crie e Ative um Ambiente Virtual
```bash
python -m venv venv
```
Ative o ambiente:
- No Windows:
```bash
venv\Scripts\activate
```
- No macOS/Linux:
```bash
  source venv/bin/activate
```
## 3. Instale as Dependências
instale o Django:
```bash
pip install django
```
## 4. Acessar a pasta com manage.py
```bash
cd src/projeto_login
```
## 5. Aplique as Migrações do Banco de Dados
Crie o banco de dados e configure o schema:
```bash
python manage.py migrate
```
## 6.Execute o Servidor de Desenvolvimento
Inicie o servidor:
```bash
python manage.py runserver
```
Acesse a aplicação pelo navegador em: http://127.0.0.1:8000/

## 🔗Funcionalidades
- ✅Tela de Login:
  - Validação de e-mail e senha.
  - Tratamento de erros específicos ("E-mail inexistente" e "Senha inválida").
  - Redirecionamento para a tela de Menu após login.
- ✅Tela de Registrar:
  - Formulário com campos: nome, e-mail, senha e confirmar senha.
  - Validações:
    - Nome aceita apenas letras.
    - E-mail deve conter “@”.
    - Senha com no mínimo 8 caracteres, 1 caractere especial, 1 número e 1 letra maiúscula.
    - Confirmação de senha idêntica.
  - Botão para alternar a visualização dos campos de senha.
  - Botões "Registrar" e "Cancelar" (este último redireciona para a tela de Login).
- ✅Extra:
  - Envio de e-mail de confirmação (Obs: A confirmação aparecerá no terminal).

  ## 📌Estrutura do Repositório
  
```text
projeto_login/                        # Diretório raiz do projeto
│
├── app_projeto_login/                # Aplicação principal do Django
│   ├── __pycache__/  
│   ├── migrations/                   # Diretório para arquivos de migração do banco de dados
│   │   ├── __pycache__/  
│   │   ├── __init__.py  
│   ├── static/app_projeto_login/     # Diretório para arquivos estáticos
│   │   ├── style.css  
│   ├── templates/accounts/           # Diretório para templates HTML
│   │   ├── login.html  
│   │   ├── menu.html  
│   │   ├── register.html  
│   ├── __init__.py  
│   ├── admin.py                      # Arquivo gerado pelo Django (vazio por padrão)
│   ├── apps.py                       # Configuração da aplicação
│   ├── forms.py                      # Formulários Django
│   ├── models.py                     # Arquivo gerado pelo Django (vazio por padrão)
│   ├── tests.py                      # Arquivo gerado pelo Django (vazio por padrão)
│   ├── urls.py                       # Rotas da aplicação
│   ├── views.py                      # Views da aplicação
│
├── projeto_login/                    # Diretório de configuração do projeto Django
│   ├── __pycache__/  
│   ├── __init__.py  
│   ├── asgi.py                       # Configuração ASGI
│   ├── settings.py                   # Configurações gerais do projeto
│   ├── urls.py                       # Rotas do projeto
│   ├── wsgi.py                       # Configuração WSGI
│
├── db.sqlite3                        # Banco de dados SQLite
├── manage.py                         # Script de gerenciamento do Django
```

## 📌Considerações Finais
- Estrutura Modular: Organização clara com diretórios separados para configurações, app, templates e arquivos estáticos.
- Validações Robústas: Formulários com validações que garantem dados íntegros e feedback imediato ao usuário.
- Funcionalidades Avançadas: Envio de e-mail de confirmação (via console).
