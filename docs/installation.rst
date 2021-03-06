Installation
============

The only officialy supported method of installing this plugin is via composer.

Using `Composer <http://getcomposer.org/>`__
--------------------------------------------

`View on
Packagist <https://packagist.org/packages/josegonzalez/cakephp-annotation-control-list>`__,
and copy the json snippet for the latest version into your project's
``composer.json``. Eg, v. 3.0.0 would look like this:

.. code:: json

    {
        "require": {
            "josegonzalez/cakephp-annotation-control-list": "3.0.0"
        }
    }

This plugin has the type ``cakephp-plugin`` set in its own
``composer.json``, composer knows to install it inside your ``/Plugins``
directory, rather than in the usual vendors file. It is recommended that
you add ``/Plugins/Upload`` to your .gitignore file. (Why? `read
this <http://getcomposer.org/doc/faqs/should-i-commit-the-dependencies-in-my-vendor-directory.md>`__.)

Enable plugin
-------------

You need to enable the plugin your ``config/bootstrap.php`` file:

.. code:: php

    <?php
    Plugin::load('Josegonzalez/AnnotationControlList');

If you are already using ``Plugin::loadAll();``, then this is not
necessary.
