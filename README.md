# Inicio Academia

Projeto inicial de gerenciamento de academia feito com Django.

## Requisitos

- Python 3.10 ou superior
- pip

## Configuração

No PowerShell, na pasta do projeto:

```powershell
py -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
Copy-Item .env.example .env
python manage.py migrate
python manage.py runserver
```

Abra <http://127.0.0.1:8000/> no navegador.

Para criar um usuário administrador e acessar o painel do Django em
<http://127.0.0.1:8000/admin/>:

```powershell
python manage.py createsuperuser
```

As configurações locais podem ser ajustadas no arquivo `.env`. O arquivo `.env`
não deve ser enviado ao controle de versão.

## Testes

```powershell
python manage.py test
```

## Estrutura inicial

- `academia_project/`: configurações e rotas do projeto.
- `core/`: aplicação inicial, página principal e testes.
- SQLite: banco de dados padrão para desenvolvimento local.
