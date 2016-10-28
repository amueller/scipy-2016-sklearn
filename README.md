Webstep 2016 Scikit-learn Tutorial
================================

Based on the [SciPy 2016 tutorial](https://github.com/amueller/scipy-2016-sklearn) by [Kyle Kastner](https://kastnerkyle.github.io/), [Sebastian Raschka](http://sebastianraschka.com), and [Andreas Mueller](http://amueller.github.io).


Instructor
-----------

- [Dr. Randy Olson](http://randalolson.com)  [(@randal_olson)](https://twitter.com/randal_olson) - University of Pennsylvania Institute for Biomedical Informatics

---

This repository will contain the teaching material and other information associated with our scikit-learn tutorial.

Parts 1 to 12 make up the day 1 session, while
parts 13 to 23 will be presented in the day 2 session.

### Schedule:

The 2-part tutorial will be held on Saturday and Sunday, October 29-30, 2016.

- Parts 1 to 12: 9:00 AM - 3:00 PM
- Parts 13 to 23: 9:00 AM - 3:00 PM


Obtaining the Tutorial Material
------------------


If you have a GitHub account, it is probably most convenient if you fork the GitHub repository. If you don’t have an GitHub account, you can download the repository as a .zip file by heading over to the GitHub repository (https://github.com/rhiever/webstep-sklearn-quickstart) in your browser and click the green “Download” button in the upper right.

![](images/download-repo.png)

Please note that I may add and improve the material until shortly before the tutorial session, and I recommend that you update your copy of the materials one day before the tutorials. If you have an GitHub account and forked/cloned the repository via GitHub, you can sync your existing fork with via the following commands:

```
git remote add upstream https://github.com/rhiever/webstep-sklearn-quickstart.git
git fetch upstream
git checkout master merge upstream/master
```

If you don’t have a GitHub account, you may have to re-download the .zip archive from GitHub.


Installation Notes
------------------

This tutorial will require recent installations of

- [NumPy](http://www.numpy.org)
- [SciPy](http://www.scipy.org)
- [matplotlib](http://matplotlib.org)
- [pillow](https://python-pillow.org)
- [scikit-learn](http://scikit-learn.org/stable/)
- [pandas](http://pandas.pydata.org/)
- [TPOT](https://pypi.python.org/pypi/TPOT/)
- [Watermark](https://pypi.python.org/pypi/watermark)
- [PyYaml](http://pyyaml.org/wiki/PyYAML)
- [IPython](http://ipython.readthedocs.org/en/stable/)
- [Jupyter Notebook](http://jupyter.org)

The last one is important, and you should be able to type:

    jupyter notebook

in your terminal window and see the notebook panel load in your web browser.
Try opening and running a notebook from the material to see check that it works.

For users who do not yet have these  packages installed, a relatively
painless way to install all the requirements is to use a Python distribution
such as [Anaconda](https://www.continuum.io/downloads), which includes
the most relevant Python packages for science, math, engineering, and
data analysis; Anaconda can be downloaded and installed for free
including commercial use and redistribution.
The code examples in this tutorial should be compatible to Python 2.7,
Python 3.4, and Python 3.5.

After obtaining the material, we **strongly recommend** that you open and execute the Jupyter Notebook
`check_env.ipynb` that is located at the top level of this repository. You can open the notebook
by executing

```bash
jupyter notebook check_env.ipynb
```

inside this repository. Inside the notebook, you can run the code cell by
clicking on the "Run Cells" button as illustrated in the figure below:

![](images/check_env-1.png)


Finally, if your environment satisfies the requirements for the tutorials, the executed code cell will produce an output message similar to the one shown below:

![](images/check_env-2.png)


Although not required, we also recommend that you update the required Python packages to their latest versions to ensure best compatibility with the teaching material. Please upgrade already installed packages by executing

- `conda update [package-name]` 
- or `pip install [package-name] --upgrade`


Data Downloads
--------------

The data for this tutorial is not included in the repository.  We will be
using several data sets during the tutorial: most are built-in to
scikit-learn, which includes code that automatically downloads and caches these
data.

**Because the wireless network connections can often be spotty, 
it would be a good idea to download these
data sets before arriving at the workshop.
Please run ``python fetch_data.py`` to download all necessary data beforehand.**

The download size of the data files are approx. 280 MB, and after `fetch_data.py`
extracted the data on your disk, the ./notebook/dataset folder will take 480 MB
of your local solid state or hard drive.


Outline
=======

Day 1 Session
---------------

- 01 Introduction to machine learning with sample applications, Supervised and Unsupervised learning [[view](notebooks/01\ Introduction\ to\ Machine\ Learning.ipynb)]
- 02 Scientific Computing Tools for Python: NumPy, SciPy, and matplotlib [[view](notebooks/02\ Scientific\ Computing\ Tools\ in\ Python.ipynb)]
- 03 Data formats, preparation, and representation [[view](notebooks/03\ Data\ Representation\ for\ Machine\ Learning.ipynb)]
- 04 Supervised learning: Training and test data [[view](notebooks/04\ Training\ and\ Testing\ Data.ipynb)]
- 05 Supervised learning: Estimators for classification [[view](notebooks/05\ Supervised\ Learning\ -\ Classification.ipynb)]
- 06 Supervised learning: Estimators for regression analysis [[view](notebooks/06\ Supervised\ Learning\ -\ Regression.ipynb)]
- 07 Unsupervised learning: Unsupervised Transformers [[view](notebooks/07\ Unsupervised\ Learning\ -\ Transformations\ and\ Dimensionality\ Reduction.ipynb)]
- 08 Unsupervised learning: Clustering [[view](notebooks/08\ Unsupervised\ Learning\ -\ Clustering.ipynb)]
- 09 The scikit-learn estimator interface [[view](notebooks/09\ Review\ of\ Scikit-learn\ API.ipynb)]
- 10 Preparing a real-world dataset (titanic) [[view](notebooks/10\ Case\ Study\ -\ Titanic\ Survival.ipynb)]
- 11 Working with text data via the bag-of-words model [[view](notebooks/11\ Text\ Feature\ Extraction.ipynb)]
- 12 Application: IMDb Movie Review Sentiment Analysis [[view](notebooks/12\ Case\ Study\ -\ SMS\ Spam\ Detection.ipynb)]

Day 2 Session
-----------------

- 13 Cross-Validation [[view](notebooks/13\ Cross\ Validation.ipynb)]
- 14 Model complexity and grid search for adjusting hyperparameters [[view](notebooks/14\ Model\ Complexity\ and\ GridSearchCV.ipynb)]
- 15 Scikit-learn Pipelines [[view](notebooks/15\ Pipelining\ Estimators.ipynb)]
- 16 Supervised learning: Performance metrics for classification [[view](notebooks/16\ Performance\ metrics\ and\ Model\ Evaluation.ipynb)]
- 17 Supervised learning: Linear Models [[view](notebooks/17\ In\ Depth\ -\ Linear\ Models.ipynb)]
- 18 Supervised learning: Support Vector Machines [[view](notebooks/18\ In\ Depth\ -\ Support\ Vector\ Machines.ipynb)]
- 19 Supervised learning: Decision trees and random forests, and ensemble methods [[view](notebooks/19\ In\ Depth\ -\ Trees\ and\ Forests.ipynb)]
- 20 Supervised learning: Feature selection [[view](notebooks/20\ Feature\ Selection.ipynb)]
- 21 Unsupervised learning: Hierarchical and density-based clustering algorithms [[view](notebooks/21\ Unsupervised\ learning\ -\ Hierarchical\ and\ density-based\ clustering\ algorithms.ipynb)]
- 22 Unsupervised learning: Non-linear dimensionality reduction [[view](notebooks/22\ Unsupervised\ learning\ -\ Non-linear\ dimensionality\ reduction.ipynb)]
- 23 Automated machine learning [[view](notebooks/23\ Automated\ machine\ learning.ipynb)]
