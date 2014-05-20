SuperBar
========

A (WIP) python progress bar


Installing
----------

.. code-block:: python

    pip install superbar

Usage
-----

.. code-block:: python

    import superbar
    import time

    for i in superbar(range(100)):
        time.sleep(0.05)

SuperBar can be customized
--------------------------

.. code-block:: python

    bar = superbar.format('Time left: {bar} {eta}')

    for i in superbar(range(100)):
        time.sleep(0.05)

The following widgets are avaliable

* ``{bar}`` The progress bar
* ``{time_ellapsed}`` The time ellapsed
* ``{eta}`` The estimated time to finish
* ``{counter}`` 0 of 100