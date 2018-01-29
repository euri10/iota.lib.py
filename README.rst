========
Overview
========

.. start-badges

.. list-table::
    :stub-columns: 1

    * - docs
      - |docs|
    * - tests
      - | |travis|


.. |docs| image:: https://readthedocs.org/projects/pyota/badge/?version=latest
    :target: http://pyota.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status

.. |travis| image:: https://travis-ci.org/iotaledger/iota.lib.py.svg?branch=master
    :alt: Travis-CI Build Status
    :target: https://travis-ci.org/iotaledger/iota.lib.py


.. end-badges


=====
PyOTA
=====
This is the official Python library for the IOTA Core.

It implements both the `official API`_, as well as newly-proposed functionality
(such as signing, bundles, utilities and conversion).

Join the Discussion
===================
If you want to get involved in the community, need help with getting setup,
have any issues related with the library or just want to discuss Blockchain,
Distributed Ledgers and IoT with other people, feel free to join our `discord`_.

You can also ask questions on our `dedicated forum`_.

If you encounter any issues while using PyOTA, please report them using the
`PyOTA Bug Tracker`_.

============
Dependencies
============
PyOTA is compatible with Python 3.6, 3.5 and 2.7.

============
Installation
============
To install the latest version::

  pip install pyota

Optional C Extension
====================
PyOTA has an optional C extension that improves the performance of its
cryptography features significantly (speedups of **60x** are common!).

To install this extension, use the following command::

   pip install pyota[ccurl]


.. _readme-installing-from-source:

Installing from Source
======================

#. `Create virtualenv`_ (recommended, but not required).
#. ``git clone https://github.com/iotaledger/iota.lib.py.git``
#. ``pip install -e .``

Running Unit Tests
------------------
To run unit tests after installing from source::

  python setup.py test

PyOTA is also compatible with `tox`_::

  pip install tox
  tox

=============
Documentation
=============
PyOTA's documentation is available on `ReadTheDocs`_.

If you are `installing from source <readme-installing-from-source>`, you
can also build the documentation locally:

#. Install extra dependencies (you only have to do this once)::

      pip install '.[docs-builder]'

   .. tip::

      To install the CCurl extension and the documentation builder tools
      together, use the following command::

         pip install '.[ccurl,docs-builder]'

#. Switch to the ``docs`` directory::

      cd docs

#. Build the documentation::

      make html

.. _Create virtualenv: https://realpython.com/blog/python/python-virtual-environments-a-primer/
.. _PyOTA Bug Tracker: https://github.com/iotaledger/iota.lib.py/issues
.. _ReadTheDocs: https://pyota.readthedocs.io/
.. _discord: https://discordapp.com/channels/397872799483428865/400435228923133959
.. _dedicated forum: https://forum.iota.org/
.. _official API: https://iota.readme.io/
.. _tox: https://tox.readthedocs.io/
