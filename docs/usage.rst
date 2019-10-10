=====
Usage
=====

To use dj-webhook-inputs in a project, add it to your `INSTALLED_APPS`:

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
