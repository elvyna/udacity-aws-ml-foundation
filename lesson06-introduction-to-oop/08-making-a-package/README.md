## Instructions

On your local computer, you need to create a folder called `3a-python-package`. Inside this folder, you need to create a few folders and files:

- A setup.py file, which is required in order to use pip install.
- A subfolder called distributions, which is the name of the Python package.
- Inside the distributions folder, you need:
  - The Gaussiandistribution.py file (provided).
  - The Generaldistribution.py file (provided).
  - The __init__.py file (you need to create this file).

Once everything is set up, in order to actually create the package, use your terminal window to navigate into the 3a_python_package folder.

Enter the following:
```
cd 3a-python-package

pip install . ## this will find the `setup.py` and run the installation
```

Then, you can test it in the Python interpreter:
```
from distributions import Gaussian

gaussian_one = Gaussian(25, 2)
gaussian_one.mean
gaussian_one + gaussian_one
```

Note: in the Python package, we put `.` in front of the imported module, e.g., `from .general_distribution import Distribution`.
