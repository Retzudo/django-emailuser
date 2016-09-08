django-emailuser
================

This package implements a custom Django user model and manager that replaces the
default user model with one that *only* has an e-mail field, not username *and*
e-mail.

It's basically a copy&paste of Django 1.10 code with the necessary (small)
adjustments.


Installation
------------

1. `pip install git+https://github.com/Retzudo/django-emailuser.git` (no, it's
   currently not on PyPI)
2. Add `emailuser` to your `INSTALLED_APPS`
3. Add `AUTH_USER_MODEL = 'emailuser.User'` to your Django project's
   `settings.py`
4. `python manage.py migrate`
5. Enjoy a user model without the username field
