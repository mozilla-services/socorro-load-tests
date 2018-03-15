======================
Crash Stats Load Tests
======================

This directory contains load tests for the webapp component of Socorro. We're
using these load tests to do a rough stress check on the webapp in the new
infrastructure we're building.

:License: MPLv2
:Date: March 14th, 2018


Requirements
============

These tests use `pipenv <https://pipenv.readthedocs.io/en/latest/>`_ to manage
dependencies, so please install it.

To install the dependencies and activate the virtual environment, please do the
following:

1. Make sure you are in this directory
2. Use the command `pipenv install` to create the virtual environment and
   install dependencies
3. Use the command `pipenv shell` to activate the virtual environment
4. Use `exit` to leave the virtual environment when you are done running the
   tests

Once you have installed the dependencies, you can always reactivate the virtual
environmenet using `pipenv shell`.


Running The Tests
=================

The tests were built using `Molotov <https://molotov.readthedocs.io/>`_ and
can be run using the following command from inside the virtual environment::

    molotov -p 2 -w 2 -d 600

Helpful arguments:

* ``-p`` - number of processes
* ``-w`` - number of workers
* ``-d`` - duration in seconds to run