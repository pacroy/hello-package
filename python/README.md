# hello

This is a hello world demo Python package.

## Install

```sh
pip install --index https://test.pypi.org/simple/ --upgrade pacroy-hello
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
   ```
3. Install build and publish tools.

   ```sh
   pip install --upgrade build
   pip install --upgrade twine
   ```

4. Build.

   ```sh
   python -m build
   ```

5. Publish.

   ```sh
   python -m twine upload --repository testpypi dist/*
   ```

   Enter username `__token__`
   Enter password with your [TestPyPi API token](https://test.pypi.org/manage/account/token/).

## References

- [Packaging Python Projects — Python Packaging User Guide](https://packaging.python.org/en/latest/tutorials/packaging-projects/)