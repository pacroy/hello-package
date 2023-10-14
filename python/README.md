# hello

This is a hello world demo Python package.

## Install

```sh
pip install -i https://test.pypi.org/simple/ pacroy-hello==0.0.1
```

## Usage

```python
from pacroy_hello import hello
hello.hello()
```

## Build & Publish

1. Install [Python version manager (pyenv)](https://github.com/pyenv/pyenv#installation).
2. Install the latest python version 3.

   ```sh
   pyenv install --list
   pyenv install 3.10.11
   pyenv versions
   pyenv global 3.10.11
   pip install --upgrade pip
   pip install --upgrade build
   pip install --upgrade twine
   ```

3. Build.

   ```sh
   python -m build
   ```

4. Publish.

   ```sh
   python -m twine upload --repository testpypi dist/*
   ```

   Enter username `__token__`
   Enter password with your [TestPyPi API token](https://test.pypi.org/manage/account/token/).

### References

- [Packaging Python Projects — Python Packaging User Guide](https://packaging.python.org/en/latest/tutorials/packaging-projects/)