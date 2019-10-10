=============================
dj-webhook-inputs
=============================

.. image:: https://badge.fury.io/py/dj-webhook-inputs.svg
    :target: https://badge.fury.io/py/dj-webhook-inputs

.. image:: https://travis-ci.org/kverdecia/dj-webhook-inputs.svg?branch=master
    :target: https://travis-ci.org/kverdecia/dj-webhook-inputs

.. image:: https://codecov.io/gh/kverdecia/dj-webhook-inputs/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/kverdecia/dj-webhook-inputs

save and signal webhook data

Documentation
-------------

The full documentation is at https://dj-webhook-inputs.readthedocs.io.

Quickstart
----------

Install dj-webhook-inputs::

    pip install dj-webhook-inputs

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'webhookinputs.apps.WebhookinputsConfig',
        ...
    )

Add dj-webhook-inputs's URL patterns:

.. code-block:: python

    from webhookinputs import urls as webhookinputs_urls


    urlpatterns = [
        ...
        url(r'^', include(webhookinputs_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
