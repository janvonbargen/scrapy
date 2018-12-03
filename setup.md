# Setup

```
virtualenv venv
```

# Package

```
source venv/bin/activate

# build distribution files
pip install setuptools wheel
python setup.py sdist bdist_wheel

# upload to local pypi
pip install twine

twine upload --repository-url http://127.0.0.1/ dist/*
# username/password: pypiuser/pypipasswd (see pypi.md)
```
