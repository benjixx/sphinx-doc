sphinx-doc
==========

Docker image for building documentation via Sphinx_.

This image has been primarily created for generating PDF documentation
via LaTeX, but may support other builders as well.

If you have a need to use it with a builder that is currently not supported
feel free to open a PR.

.. _Sphinx: http://www.sphinx-doc.org/


Usage
-----

.. code-block:: bash

    $ docker run -v path/to/your/sphinx/docs:/docs benjixx/sphinx-doc make latexpdf
