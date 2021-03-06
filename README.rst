.. Request data &middot; [![Build Status](https://travis-ci.org/ViderumGlobal/ckanext-saasportal_quote.svg?branch=master)](https://travis-ci.org/ViderumGlobal/ckanext-saasportal_quote)  [![Coverage Status](https://coveralls.io/repos/github/ViderumGlobal/ckanext-saasportal_quote/badge.svg?branch=master)](https://coveralls.io/github/ViderumGlobal/ckanext-saasportal_quote?branch=master)

.. You should enable this project on travis-ci.org and coveralls.io to make
   these badges work. The necessary Travis and Coverage config files have been
   generated for you.

.. image:: https://travis-ci.org/ViderumGlobal/ckanext-saasportal_quote.svg?branch=master
     :target: https://travis-ci.org/ViderumGlobal/ckanext-saasportal_quote

.. image:: https://coveralls.io/repos/github/ViderumGlobal/ckanext-saasportal_quote/badge.svg?branch=master
    :target: https://coveralls.io/github/ViderumGlobal/ckanext-saasportal_quote?branch=master


=============
ckanext-saasportal_quote
=============

This extension provides 'Get a quote' button in the header that redirects to Quote register form in Viderum page.

------------
Installation
------------

.. Add any additional install steps to the list below.
   For example installing any non-Python dependencies or adding any required
   config settings.

To install ckanext-saasportal_quote:

1. Activate your CKAN virtual environment, for example::

     . /usr/lib/ckan/default/bin/activate

2. Install the ckanext-saasportal_quote Python package into your virtual environment::

     pip install ckanext-saasportal_quote

3. Add ``saasportal_quote`` to the ``ckan.plugins`` setting in your CKAN
   config file (by default the config file is located at
   ``/etc/ckan/default/production.ini``).

4. Restart CKAN. For example if you've deployed CKAN with Apache on Ubuntu::

     sudo service apache2 reload


---------------
Config Settings
---------------


------------------------
Development Installation
------------------------

To install ckanext-saasportal_quote for development, activate your CKAN virtualenv and
do::

    git clone https://github.com/jgulic_/ckanext-saasportal_quote.git
    cd ckanext-saasportal_quote
    python setup.py develop
    pip install -r dev-requirements.txt


-----------------
Running the Tests
-----------------

To run the tests, do::

    nosetests --nologcapture --with-pylons=test.ini

To run the tests and produce a coverage report, first make sure you have
coverage installed in your virtualenv (``pip install coverage``) then run::

    nosetests --nologcapture --with-pylons=test.ini --with-coverage --cover-package=ckanext.saasportal_quote --cover-inclusive --cover-erase --cover-tests


---------------------------------
Registering ckanext-saasportal_quote on PyPI
---------------------------------

ckanext-saasportal_quote should be availabe on PyPI as
https://pypi.python.org/pypi/ckanext-saasportal_quote. If that link doesn't work, then
you can register the project on PyPI for the first time by following these
steps:

1. Create a source distribution of the project::

     python setup.py sdist

2. Register the project::

     python setup.py register

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the first release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.1 then do::

       git tag 0.0.1
       git push --tags


----------------------------------------
Releasing a New Version of ckanext-saasportal_quote
----------------------------------------

ckanext-saasportal_quote is availabe on PyPI as https://pypi.python.org/pypi/ckanext-saasportal_quote.
To publish a new version to PyPI follow these steps:

1. Update the version number in the ``setup.py`` file.
   See `PEP 440 <http://legacy.python.org/dev/peps/pep-0440/#public-version-identifiers>`_
   for how to choose version numbers.

2. Create a source distribution of the new version::

     python setup.py sdist

3. Upload the source distribution to PyPI::

     python setup.py sdist upload

4. Tag the new release of the project on GitHub with the version number from
   the ``setup.py`` file. For example if the version number in ``setup.py`` is
   0.0.2 then do::

       git tag 0.0.2
       git push --tags
