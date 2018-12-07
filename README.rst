
======
wavePy
======


`wavePy <https://github.com/aps-xsd-opt-group/wavepy>`_ is Python library for data analyses of coherence and wavefront measurements at syncrotron beamlines. Currently it covers: single grating imaging, speckle tracking, scan of Talbot peaks for coherence.

Documentation
-------------
* https://wavepy.readthedocs.org

Credits
-------

We kindly request that you cite the following `articles <https://wavepy.readthedocs.io/en/latest/source/credits.html#citations>`_ 
if you use wavePy.

* List here the features.

Contribute
----------

* Documentation: https://github.com/aps-xsd-opt-group/wavepy/tree/master/doc
* Issue Tracker: https://github.com/aps-xsd-opt-group/wavepy/issues
* Source Code: https://github.com/aps-xsd-opt-group/wavepy

==========================
Prerequisites
==========================

The following libraries should be installed in your system:

- FFTW3, see: http://www.fftw.org/download.html
- Xraylib, see: https://github.com/tschoonj/xraylib/wiki/Installation-instructions
- DXchange, see: https://dxchange.readthedocs.io/en/latest/source/install.html

==========================
Installation
==========================

>>> python3 -m pip install wavepy



==========================
Installation as Developer
==========================



Syncing with git
----------------

.. NOTE:: You need to have ``git`` installed


Clone
-----

>>> git clone https://github.com/aps-xsd-opt-group/wavepy



Update your local installation
------------------------------

>>> git pull


To make git to store your credentials
-------------------------------------

>>> git config credential.helper store




Solving dependencies with conda
-------------------------------

.. NOTE:: You need to have ``anaconda`` or ``miniconda`` installed


Creating conda enviroment
-------------------------

>>> conda create -n ENV_NAME python=3.5 numpy=1.11  scipy=0.17 matplotlib=1.5 spyder=2.3.9 --yes

.. WARNING:: edit ``ENV_NAME``



Solving dependencies
--------------------


Activate the enviroment:

>>> source activate ENV_NAME


.. WARNING:: edit ``ENV_NAME``


>>> conda install scikit-image=0.12 --yes
>>> conda install -c dgursoy dxchange --yes

>>> pip install cffi
>>> pip install unwrap
>>> pip install tqdm
>>> pip install termcolor
>>> pip install easygui_qt

.. NOTE:: ``unwrap`` needs ``cffi``, ``tqdm`` is used for progress bar



Adding Recomended packages
--------------------------

>>> conda install -c dgursoy xraylib




Additional Settings
-------------------

``easygui_qt`` conflicts with the Qt backend of
``matplotlib``. The workaround 
is to change the backend to TkAgg. This can be in the *matplotlibrc* file 
(instructions
`here <http://matplotlib.org/users/customizing.html#customizing-matplotlib>`_).
In Spyder this is done in Tools->Preferences->Console->External Modules,
where we set GUI backend to
TkAgg
