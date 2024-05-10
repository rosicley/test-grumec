Researcher projects

We should list the projects that are currently being worked on by the researchers. This will help us to keep track of the projects and to make sure that we are all on the same page.

=====

.. _installation:

Installation
------------

To use Grumec, first install it using pip:

.. code-block:: console

   (.venv) $ pip install grumec

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``grumec.get_random_ingredients()`` function:

.. autofunction:: grumec.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`grumec.get_random_ingredients`
will raise an exception.

.. autoexception:: grumec.InvalidKindError

For example:

>>> import grumec
>>> grumec.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

