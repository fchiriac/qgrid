

This is another qgrid fork from the official Quantopian repo as the project is no longer maintained by Quantopian.
Adding some fixes long the way.

Feel free to test it out locally following the bellow steps.

Running from source & testing your changes
=====

If you'd like to contribute to qgrid, or just want to be able to modify the source code for your own purposes, you'll want to clone this repository and run qgrid from your local copy of the repository. The following steps explain how to do this.

Clone the repository from GitHub and cd into the top-level directory:
=====

git clone https://github.com/fchiriac/qgrid

Go to the cloned project directory:
=====

cd qgrid

Install the current project in editable mode:
=====

pip install -e .

Install the node packages that qgrid depends on and build qgrid's javascript using webpack:
=====

cd js && npm install .

Install and enable qgrid's javascript in your local jupyter notebook environment:
=====

jupyter nbextension install --py --symlink --sys-prefix qgrid && jupyter nbextension enable --py --sys-prefix qgrid

If desired, install the labextension:
=====

jupyter labextension link js/

Run the notebook as you normally would with the following command:
=====

jupyter notebook

=====
qgrid
=====
Qgrid is a Jupyter notebook widget which uses `SlickGrid <https://github.com/mleibman/SlickGrid>`_ to render pandas
DataFrames within a Jupyter notebook. This allows you to explore your DataFrames with intuitive scrolling, sorting, and
filtering controls, as well as edit your DataFrames by double clicking cells.

API Documentation
-----------------
API documentation is hosted on `readthedocs <http://qgrid.readthedocs.io/en/latest/>`_.

If you are looking to start working with the qgrid codebase, navigate to the GitHub issues tab and start looking
through interesting issues.

Feel free to ask questions by submitting an issue with your question.
