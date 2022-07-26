## PRÉ REQUISITOS
- Python == 3.10


## CRIAÇÃO
- Para criar um ambiente virtual em Python, no console digite python -m venv venv ou python3 -m venv venv.

- Para executar o ambiente virtual em Python, no console digite venv\Scripts\activate para Windows ou . venv/bin/activate para Linux e MacOs.

- Para instalar as dependências do projeto, no console digite pip install django, e depois no console digite pip install django psycopg2.

- Para configurar o banco de dados local, pois o banco de dados está sendo hospedado localmente, para configurar os acessos, entre no diretório (mysite), 
depois entre no arquivo (settings.py) e na linha 77 (DATABASES) insira as informações de acesso do seu banco local.

Exemplo de Configuração (Postgresql)

    'default': { 
        'ENGINE': 'django.db.backends.postgresql', 
        'NAME': Nome do banco de dados, 
        'USER': Usuário do banco de dados, 
        'PASSWORD': Senha do banco de dados, 
        'HOST': Hospedagem do banco, 
        'PORT': 5432, 
    } 


## Uso
- Para passar os modelos para o banco de dados, no console digite python manage.py makemigrations ou python3 manage.py makemigrations, e depois no console 
digite python manage.py migrate ou python3 manage.py migrate.

- Para rodar o servidor, no console digite python manage.py runserver ou python3 manage.py runserver, assim no console aparecerá uma URL para você
conseguir acessar http://127.0.0.1:8000.
