==========================================================
IATI Publisher Docs
==========================================================

Deployed to: https://docs.publisher.iatistandard.org/en/latest/

Docs should build automatically upon pull request.

Features of the docs
--------------------

Uses https://github.com/OpenDataServices/sphinx-base, but without markdown or json support.
See the `examples <https://sphinx-base.readthedocs.io/en/latest/examples/>`__ and `kitchen sink <https://sphinx-base.readthedocs.io/en/latest/kitchen-sink/>`__ sections for some directives you can use.


Build the docs locally
----------------------
  
Assuming a unix based system:

.. code-block:: bash

  # Make sure you have python3 venv, e.g. for Ubuntu
  # If you're not sure, try creating a venv, and see if it errors
  sudo apt-get install python3-venv
  
  # Create a venv
  python3 -m venv .ve    
  
  # Enter the venv, needs to be run for every new shell
  source .ve/bin/activate
  
  # Install requirements
  pip install -r requirements.txt
  
  # Build the docs
  cd docs
  make dirhtml


Built docs are in `docs/_build/dirhtml`.


To view the built docs:

.. code-block:: bash

  cd _build/dirhtml
  python -m http.server


Then go to http://localhost:8000/ in a browser.


Using VS Code
-------------

A devcontainer.json and launch.json are supplied which add sphinx-autobuild as a Run option


Contributing
============

In order to contribute to this documentation, create a new branch and make your suggested changes. Then, open a Pull Request; this will build a preview of your changes and let you see what the complete site will look like. 



Translations
============

The process for getting documentation translated is:

* Extract English strings into a .pot file
* Send the .pot file for translation
* Recieve .po files from the translation process
* Check the .po files into the repo
* Re-run the build process with the translations


Extract Strings
---------------

.. code-block:: bash

  cd docs
  make gettext
  # .pot files are in _build/locale


Send for translation & Receive translations
-------------------------------------------

Nothing automated here, sorry. Ask @robredpath for details. 

Check the files into the repo
-----------------------------

Place the files into `docs/locale/fr/LC_MESSAGES/` (replacing fr with the appropriate langauge code as required)

Re-run the build
----------------

On ReadTheDocs, projects that are translations don't auto-build on Pull Request. If you want to preview the documentation in another language, you can create a Version via the RTD interface and set it up to build the branch that you're working on. Translated versions will automatically rebuild when the Pull Request is merged, however. 

If building locally: 

.. code-block:: bash

  cd docs
  make -e SPHINXOPTS="-D language='fr'" dirhtml

Built docs are in `docs/_build/dirhtml`.




