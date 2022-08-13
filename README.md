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

## USO
- Para passar os modelos para o banco de dados, no console digite python manage.py makemigrations ou python3 manage.py makemigrations, e depois no console 
digite python manage.py migrate ou python3 manage.py migrate.

- Para rodar o servidor, no console digite python manage.py runserver ou python3 manage.py runserver, assim no console aparecerá uma URL para você
conseguir acessar http://127.0.0.1:8000.
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
## PREREQUISITES
- Python == 3.10

## CREATION
- To create a virtual environment in Python, at the console type python -m venv venv or python3 -m venv venv.

- To run the virtual environment in Python, in the console type venv\Scripts\activate for Windows or . venv/bin/activate for Linux and MacOs.

- To install project dependencies, in the console type pip install django and then in the console type pip install django psycopg2.

- To configure the local database, as the database is being hosted locally, to configure the accesses, enter the directory (mysite), then enter the
file (settings.py) and on line 77 (DATABASES) enter the access information of your local bank.

Configuration Example (Postgresql)

    'default': { 
        'ENGINE': 'django.db.backends.postgresql', 
        'NAME': Nome do banco de dados, 
        'USER': Usuário do banco de dados, 
        'PASSWORD': Senha do banco de dados, 
        'HOST': Hospedagem do banco, 
        'PORT': 5432, 
    } 

## USE
- To pass the models to the database, in the console type python manage.py makemigrations or python3 manage.py makemigrations, then in the console
type python manage.py migrate or python3 manage.py migrate.

- To run the server, in the console type python manage.py runserver or python3 manage.py runserver, so in the console a URL will appear for you
able to access http://127.0.0.1:8000.
