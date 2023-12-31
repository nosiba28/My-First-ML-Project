# MyML Project:
Project name: MyML

This project actually defines the ML project structure.

## Description
   1. create virtual environment:
       > conda create --name venv python=3.9
   2. activate the venv
       > conda activate venv 
   3. create a project folder
       > mkdir MyML
   4. do some following installation
   5. edit conf.py file: 
     >import os
     >import sys
     >sys.path.insert(0, os.path.abspath("../my_py_pkg/src"))
     >project = 'MyML'
     >copyright = '2023, Khandoker Nosiba Arifin'
     >author = 'Khandoker Nosiba Arifin'
     >release = '0.0.0.1'
     >extensions = [
    "sphinx.ext.viewcode",
    "sphinx.ext.todo",
    "sphinx.ext.autodoc"
     ]
     >templates_path = ['_templates']
   6. Add modules into the insert.rst
   7. do some following installation 3 & 4
   8. using cmd
    >cd docs
    >sphinx-quickstart
    >cd my-py-pkg
    >sphinx_apidoc -o ../docs src/
    >cd docs
    >make html
    9. If you want to show the html file then go to the --> docs>build>html>index.html the right click an copy the file and open it using the browser.
    10. then create setup.py and install the following
    11. then for build and upload package to the pypi.org and we must have an account to the pypi.org. note: package name must be unique otherwise we will get error.
   >> python setup.py sdist bdist_wheel
   >> twine upload dist/*
      > username: __token__
      > password: "your-api-token"
   


## Installation
   1. install conda(miniconda3)
   2. install make (for running make file)
   After installing make 
   > make --version
   > make install (for running the Makefile and installing the packages which are include into the requirements.txt)
   (we have to create docs folder where all the documentations of our project are being saved now we have to install these 3 & 4 no)
   3. pip install sphinx
   4. pip install sphinx-rtd-theme

   (for setup.py)
   5. pip install setuptools
   (for locally publish the package)
   6. pip install -e .
   7. pip install twine
   


## Contributors

## License
Go to the https://opensource.org/ > Licenses > popular/ strong Community> MIT License(copy & paste to the LICENSE file & edit the author name and copyright year)