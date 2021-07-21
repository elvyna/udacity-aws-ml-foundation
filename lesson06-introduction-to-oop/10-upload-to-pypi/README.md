## Instructions

In the Supporting materials section of this page, there is a zip file called `5-exercise-upload-to-pypi.zip` . Download and unzip this file.

The Python package is located in the folder `5_exercise_upload_to_pypi`.

You need to create three files:

- setup.cfg
- README.md
- license.txt

You also need to create accounts for the pypi test repository and pypi repository.

Don't forget to keep your passwords; you'll need to type them into the command line.

Once you have all the files set up correctly, you can use the following commands on the command line. **You need to make the name of the package unique**, so change the name of the package from distributions to something else. That means changing the information in `setup.py` and the folder name.

In the terminal, make sure you are in the `5_exercise_upload_to_pypi` directory. If not, navigate there by entering the following at the command line:

```
cd 5_exercise_upload_to_pypi

python setup.py sdist

pip install twine

```

## Commands to upload to the PyPi test repository

```
twine upload --repository-url https://test.pypi.org/legacy/ dist/*

pip install --index-url https://test.pypi.org/simple/ distributions
```

### Command to upload to the PyPi repository

```
twine upload dist/*

pip install distributions
```
