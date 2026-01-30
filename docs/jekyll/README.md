# {{ site.title }}

[![License](https://img.shields.io/github/license/{{ site.github_username }}{{ site.baseurl }})](LICENSE.md)

**Author:** {{ site.author }}  
**Version:** {{ site.version }}  

## Overview

{{ site.description }}  

***

**CI/CD Check List:**

![changelog](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/changelog.yml/badge.svg)
![dependency-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/dependency-check.yml/badge.svg)
![format-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/format-check.yml/badge.svg)
![lint-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/lint-check.yml/badge.svg)
![security-audit](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/security-audit.yml/badge.svg)
![spellcheck](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/spellcheck.yml/badge.svg)
![tests](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/tests.yml/badge.svg)
![typecheck](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/typecheck.yml/badge.svg)
<!-- ![release](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/release.yml/badge.svg) -->

***

## Usage Examples

***

## Development Strategy

### 🐍️ Build environment (.venv)

``` shell
$ make install
```

### 🧬 Dependency Management (deptry)

```shell
$ make dependency-check
```

### 🛡️ Security Audit (pip-audit)

```shell
$ make security
```

### 🎨 Formatting (black)

```shell
$ make format-check
```

```shell
$ make format-fix
```

### 🔍 Linting (ansible-lint, ruff, tomllint, & yaml-lint)

``` shell
$ make lint-check
```

``` shell
$ make lint-fix
```

### 🎓 Spellchecking (codespell)

```shell
$ make spellcheck
```

### 🧠 Typechecking (mypy)

``` shell
$ make typecheck
```

### 🧪 Testing (pytest, galaxy-importer)

``` shell
$ make test
```

``` shell
$ make galaxy-import
```

### 🚀 Release (git tag)

```shell
$ make release
```

### ❓ Build Help

``` shell
$ make help
```

## Commit Help:

**Note:** Commits are required to be conventional git commit message.  This helps with the auto-generation of the changelog files and is enforced by pre-commit.  

**options (default):**

* docs
* chore
* feat
* fix
* refactor
* ci
* test
* perf
* revert
* build
* style

**example:**  

```shell
<type>[optional scope]: <description>

[optional body]

[optional footer(s)]
```

* ```<type>```: A required noun that describes the nature of the change.  
* ```[optional scope]```: An optional phrase within parentheses that specifies the part of the codebase being affected (e.g., fix(parser):).  
* ```<description>```: A required short, imperative-mood summary of the changes.  
* ```[optional body]```: A longer description providing additional context and "what and why" details.  
* ```[optional footer(s)]```: Used for adding meta-information, such as issue references (Fixes #123) or indicating breaking changes.  

***

## Requirements

**Python 3.11**  

```shell
$ sudo apt install python3.11
```

***

## Author's Notes

### TODO's

1. Documentation is currently getting wrong project_slug/name. ❌
    * Currently path for documentation is just the ```$(project_name)``` and not the ```$(namespace).$(project_name)```.
2. Finish ci/cd for changelog generation using antsichaut ❌
3. Decide if i should:  
    * Create ci/cd for documentation rather than using pre-commit

***
