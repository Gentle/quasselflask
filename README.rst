=====================================================
Quasselflask - a work in progress quasselcore utility
=====================================================

currently, this tool only can do one-shot password changes,
but more features are planned.

since Flask-SQLAlchemy-1.0 has broken reflection,
this tool currently requires said package from git :(

Installation:
=============

::

   pip install -r requirements.txt

create a config file, see example file.

::

   SQLALCHEMY_DATABASE_URI = 'postgresql+psycopg2://quassel:yourpassword@localhost/quassel'
   SECRET_KEY = 'set this to something secret'

Running it:
===========

::

   export QUASSELFLASK_SETTINGS=/path/to/config.cfg
   python manage.py runserver
