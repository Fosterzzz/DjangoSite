# Fusion Website

Projeto feito no meu primeiro curso de Django.

## 🚀 Começando

Essas instruções permitirão que você obtenha uma cópia do projeto em operação na sua máquina local para fins de desenvolvimento e teste.

```
git clone https://github.com/JoaoViana1/DjangoSite.git
```

### 📋 Pré-requisitos

De que coisas você precisa para instalar o software e como instalá-lo?

```
apt install python3-pip
```

### 🔧 Instalação

Uma série de exemplos passo-a-passo que informam o que você deve executar para ter um ambiente de desenvolvimento em execução.

Crie o ambiente virtual:
```
python -m venv venv
ou
python3 -m venv venv
```
Acesse o ambiente virtual criado:
```
Linux: source venv/bin/active
Windows: .\venv\Scripts\active
```
Instale os pacotes python do projeto
```
pip install -r requirements.txt
or
pip3 install -r requirements.txt
```

E repita:

```
python manage.py makemigrations
python manage.py migrate
```



## 📦 Desenvolvimento

Mude as configurações no settings
```
EMAIL_HOST_USER = 'Coloque seu email aqui'
ALLOWED_HOSTS = ['dominio.com']
```

Crie um superuser:
```
python manage.py createsuperuser
ou
python3 manage.py createsuperuser
```


Modifique e escolha o banco de dados desejado. Opções:

SQLite:
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
    }
}
```
MySQL:
Digite no seu terminal:
```
pip install mysqlclient
```
Modifique no settings:
```
DATABASES = {
    'default': {
        'ENGINE'  : 'django.db.backends.mysql', # <-- Modifique essa linha
        'NAME'    : 'mytestdb',                 # <-- Modifique essa linha 
        'USER'    : 'test',                     # <-- Modifique essa linha
        'PASSWORD': 'Secret_1234',              # <-- Modifique essa linha
        'HOST'    : 'localhost',                # <-- Modifique essa linha
        'PORT'    : '3306',
    }
}
```

PostgreSQL:
Digite no seu terminal:
```
pip install psycopg2-binary
```
Modifique no settings:
```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2', # <-- Modifique essa linha
        'NAME'    : 'mytestdb',                 # <-- Modifique essa linha 
        'USER'    : 'test',                     # <-- Modifique essa linha
        'PASSWORD': 'Secret_1234',              # <-- Modifique essa linha
        'HOST'    : 'localhost',                # <-- Modifique essa linha
        'PORT'    : '5432',
    }
}
```

## 🛠️ Construído com

* [Django](https://docs.djangoproject.com/en/4.0/) - O framework web usado
* [Python](https://docs.python.org/3.7/) - Linguagem Usada

## 🖇️ Colaborando

## 📌 Versão

* Python 3.7
* Django 2.2.5
## ✒️ Autores


* **João** - *Todo o projeto* - [João](https://www.linkedin.com/in/jo%C3%A3o-guilherme-viana-de-medeiros-b903251a3/)



