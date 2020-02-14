# Development process

Welcome…

## Test suite

Requirements:

- [pyenv](https://github.com/pyenv/pyenv)
- [tox](https://tox.readthedocs.io)
- [vale](https://errata-ai.gitbook.io/vale)
- [node](https://nodejs.org)
- [sed](https://www.gnu.org/software/sed)

MacOS X contributors need to install gnu-sed

```bash
brew install gnu-sed
```

then **you have to add\modify to your PATH like this 'PATH="/usr/local/opt/gnu-sed/libexec/gnubin:\$PATH"' from your ~/.bashrc or ~/.zshrc**

Running test suite:

```bash
tox
```

After the test suite finished successful and if you use a PyCharm you should setup `{YOU PROJECT ROOT}.tox/.package/bin/python3.8` as a project interpreter

Install needed npms

```bash
npm install
```

Code coverage…

## Documentation

We use:

- [mkdocs](https://www.mkdocs.org)
- [doctest](https://docs.python.org/3/library/doctest.html)

Running live-reloading server:

```bash
tox -e mkdocs -- serve
```

## Release

We use:

- [semantic-release](https://semantic-release.gitbook.io/semantic-release)
- [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog)

Commit changes:

```bash
npx commit
```
