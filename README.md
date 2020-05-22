#### Boilerplate_Environment_Settings

### Configuration Instructions

* Install these packages in your virtual environment by running these commands:

```sh
pip install django-debug-toolbar
```

```sh
pip install django-heroku
```

* Create the static, staticfiles and media folders in the root directory of your project.

### For development environment usage

* Check the database settings in `dev.py` file within the settings folder, the default database generated by Django is sqlite3. If you'd prefer to work with another database engine, consult the [Django dcumentation](https://docs.djangoproject.com/en/3.0/topics/install/#database-installation) for installation and setup instructions.

### For production environment usage

* Check your database settings in `prod.py` file within the settings folder. Heroku's default database is PostgreSQL, so the database settings in the `prod.py` file should match this.

* Ensure that development settings are not used in production. The code in the `__init__.py` file within the settings folder should clearly reflect the different files to be used depending on the environment.
