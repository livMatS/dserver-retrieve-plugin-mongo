dserver Retrieve Plugin Mongo
=============================

.. |dtool| image:: https://github.com/jic-dtool/dserver-retrieve-plugin-mongo/blob/main/icons/22x22/dtool_logo.png?raw=True
    :height: 20px
    :target: https://github.com/jic-dtool/dserver-retrieve-plugin-mongo
.. |pypi| image:: https://img.shields.io/pypi/v/dserver-retrieve-plugin-mongo
    :target: https://pypi.org/project/dserver-retrieve-plugin-mongo/
.. |tag| image:: https://img.shields.io/github/v/tag/jic-dtool/dserver-retrieve-plugin-mongo
    :target: https://github.com/jic-dtool/dserver-retrieve-plugin-mongo/tags
.. |test| image:: https://img.shields.io/github/actions/workflow/status/jic-dtool/dserver-retrieve-plugin-mongo/test.yml?branch=main&label=tests
    :target: https://github.com/jic-dtool/dserver-retrieve-plugin-mongo/actions/workflows/test.yml
.. |zenodo| image:: https://zenodo.org/badge/564037054.svg
    :target: https://zenodo.org/doi/10.5281/zenodo.12702159

|dtool| |pypi| |tag| |test| |zenodo|

Retrieve plugin for dserver using mongodb

To install the ``dserver-retrieve-plugin-mongo`` package.

.. code-block:: bash

    cd dserver-retrieve-plugin-mongo
    python setup.py install

To configure the connection to the mongo database.

.. code-block:: bash

    export RETRIEVE_MONGO_URI="mongodb://localhost:27017/"
    export RETRIEVE_MONGO_DB="dserver"
    export RETRIEVE_MONGO_COLLECTION="datasets"


Testing
^^^^^^^

Testing requires a minimal ``dserver`` installation including a
functional search plugin, i.e.

.. code-block:: bash

    pip install dservercore
    pip install dserver-search-plugin-mongo

Installation with the ``[test]`` extension

.. code-block:: bash

    pip install .[test]

installs these essential testing dependencies as well.

Run tests from within repository root with ``pytest``.
