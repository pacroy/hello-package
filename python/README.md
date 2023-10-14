# hello

This is a hello world demo Python package.

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
   ```

3. Build.

   ```sh
   python -m build
   ```

### References

- [Packaging Python Projects — Python Packaging User Guide](https://packaging.python.org/en/latest/tutorials/packaging-projects/)