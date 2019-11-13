# Google Style Pre-Commit Hook

A handy [pre-commit](http://pre-commit.com/) hook which will run Google's java
code style formatter for you on your code!

## Usage

Add to your **.pre-commit-hooks.yaml** file:
```
repos:
- repo: https://github.com/antonrud/google-style-precommit-hook
  rev: ed51ff6120772ad9d234cc7ab3331e32e5231a2c
  hooks:
    - id: google-style-java
```

*Note*: this file stores Google's code style formatter jar in a `.cache/`
directory so that it doesn't need to be re-downloaded each time.  You will
probably want to add `.cache/` to the `.gitignore` file of the project which
uses this hook.


### Acknowledgement
This project is originated from repository: [maltzj/google-style-precommit-hook](https://github.com/maltzj/google-style-precommit-hook) *(not being actively maintained)*
