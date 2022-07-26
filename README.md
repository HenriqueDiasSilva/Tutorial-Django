## PRÉ REQUISITOS
- Python == 3.10


## CRIAÇÃO
- Crie um ambiente Python
No console digite: python -m venv venv ou python3 -m venv venv

- Execute o ambiente Python
 No console digite: venv\Scripts\activate para Windows ou . venv/bin/activate para Linux e MacOs

- Instale as dependências do projeto
No console digite: pip install django
No console digite: pip install django psycopg2

- Configure o banco de dados local
O banco de dados está sendo hospedado localmente, para configurar os acessos, entre no diretório (mysite), depois entre no arquivo (settings.py) 
e na linha 77 (DATABASES) insira as informações de acesso do seu banco local.

Exemplo de Configuração (Postgresql)
DATABASES = { 

    'default': { 
        'ENGINE': 'django.db.backends.postgresql', 
        'NAME': Nome do banco de dados, 
        'USER': Usuário do banco de dados, 
        'PASSWORD': Senha do banco de dados, 
        'HOST': Hospedagem do banco, 
        'PORT': 5432, 
    } 
}


## Uso
- Passe os modelos para o banco de dados
No console digite: python manage.py makemigrations ou python3 manage.py makemigrations
No console digite: python manage.py migrate ou python3 manage.py migrate

- Rode o servidor
No console digite: python manage.py runserver ou python3 manage.py runserver
No console: http://127.0.0.1:8000
