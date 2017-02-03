cookiecutter-salt-formula
=========================

A cookiecutter template for Salt Formula.

Installation
============

.. code-block:: bash

    pip install cookiecutter

    cd cookiecutter

    cookiecutter salt-formula


Init Kitchen CI
===============

Install prerequisites.
- `envtpl` is renders jinja2 templates on the command line with shell environment variables.
- gems required dpends on driver configured to be used (docker by default)

.. code-block:: bash

    pip install envtpl
    gem install kitchen-docker kitchen-vagrant kitchen-salt kitchen-openstack kitchen-inspec busser-serverspec

Once you create your `tests/pillar` structure (required if you want to auto populate kitchen test suites)

.. code-block:: bash

    pip install envtpl
    ./kitchen-init.sh

Instantly for latest version or on existing formulas:

.. code-block:: bash

    curl -skL "https://raw.githubusercontent.com/salt-formulas/salt-formulas/master/cookiecutter/salt-formula/kitchen-init.sh" | bash -s --

