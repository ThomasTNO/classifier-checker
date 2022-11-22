# Classifier-checker

Classifier-checker validates configured classifiers for you!

## Install

```console
$ pip install classifier-checker
```

## Usage

```console
$ classifier-checker --help
usage: classifier-checker [-h] [--strict] [--ignore-private] [--trove] [-a ACCEPT] [-d DENY] [-af ACCEPT_FILE] [-df DENY_FILE] [--verbose] package

Classifier-checker v0.1.2.
Classifier-checker validates configured classifiers for you!

positional arguments:
  package               Installed package to validate

optional arguments:
  -h, --help            show this help message and exit
  --strict              Enables strict mode, classifiers should be exactly equal to accepted classifiers
  --ignore-private      Ignore all classifiers that start with "Private ::"
  --trove               Ensure that classifiers are in line with trove-classifiers, the canonical source for classifiers on PyPI
  -a ACCEPT, --accept ACCEPT
                        Accepted classifier(s) (comma-separated)
  -d DENY, --deny DENY  Denied classifier(s) (comma-separated)
  -af ACCEPT_FILE, --accept-file ACCEPT_FILE
                        Path to file containing accepted classifier(s) (new line-separated)
  -df DENY_FILE, --deny-file DENY_FILE
                        Path to file containing denied classifier(s) (new line-separated)
  --verbose             Enable verbose logging

Licensed under MIT, 2022 Thomas Rooijakkers
```