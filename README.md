# Polls App

Aplicação exemplo usando Python Django para demonstrar uso de bancos de dados em nuvem e deployment em VMs.

Instale as dependências para desenvolvimento:

```
python -m pip install -r requirements/devo.txt
```

Defina as seguintes variáveis de ambiente:

```
DATABASE_ENGINE=django.db.backends.postgresql_psycopg2
DATABASE_NAME=poller
DATABASE_USER=poller
DATABASE_PASSWORD=pollerpasswd
DATABASE_HOST=localhost
DATABASE_PORT=5432
```

Com os valores refletindo seu ambiente.

Caso seja a primeira execução, faça a migração para configurar o estado inicial do banco de dados

```
python manage.py migrate
```

Inicie em modo desenvolvimento com

```
python manage.py runserver 0:8000
```

E acesse o site em `IP:8000`, se estiver rodando localmente `localhost:8000`.

### Autor

donatoaz@ baseado no tutorial https://docs.djangoproject.com/en/3.2/contents/