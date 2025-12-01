# taski-docker
Была проблема:

Traceback (most recent call last): File "/home/anastasia/Dev/taski-docker/backend/manage.py", line 11, in main from django.core.management import execute_from_command_line File "/home/anastasia/Dev/taski-docker/venv/lib/python3.12/site-packages/django/init.py", line 1, in <module> from django.utils.version import get_version File "/home/anastasia/Dev/taski-docker/venv/lib/python3.12/site-packages/django/utils/version.py", line 6, in <module> from distutils.version import LooseVersion ModuleNotFoundError: No module named 'distutils'
The above exception was the direct cause of the following exception:
Traceback (most recent call last): File "/home/anastasia/Dev/taski-docker/backend/manage.py", line 22, in <module> main() File "/home/anastasia/Dev/taski-docker/backend/manage.py", line 13, in main raise ImportError( ImportError: Couldn't import Django. Are you sure it's installed and available on your PYTHONPATH environment variable? Did you forget to activate a virtual environment?

Решилась установкой данной библиотеки:
pip install setuptools