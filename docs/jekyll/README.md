# {{ site.title }}

[![License](https://img.shields.io/github/license/{{ site.github_username }}{{ site.baseurl }})](LICENSE.md)

**Author:** {{ site.author }}  
**Version:** {{ site.version }}  

## Overview

{{ site.description }}  

***

**CI/CD Check List:**

* ![changelog](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/changelog.yml/badge.svg)
* ![dependency-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/dependency-check.yml/badge.svg)
* ![format-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/format-check.yml/badge.svg)
* ![lint-check](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/lint-check.yml/badge.svg)
* ![security-audit](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/security-audit.yml/badge.svg)
* ![spellcheck](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/spellcheck.yml/badge.svg)
* ![tests](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/tests.yml/badge.svg)
* ![typecheck](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/typecheck.yml/badge.svg)
<!-- ![release](https://github.com/jcook3701/jcook3701.flatpak/actions/workflows/release.yml/badge.svg) -->

***

## Usage Examples

***

## 🌱 Getting Started

* [Requirements]({{ site.github_io_url }}/manual/setup-guide/requirements)
* [Installation guide]({{ site.github_io_url }}/manual/introduction/installation-guide)  

## 📚 Documentation

The {{ site.title }} documentation is available at [docs]({{ site.github_io_url }}).  

## 🤝 Contributing

If you're interested in contributing to the {{ site.title }} project:  

* Start by reading the [contributing guide]({{ site.github_io_url }}/manual/developer-resources/contribute).  
* Learn how to setup your local environment, in our [developer guide]({{ site.github_io_url }}/manual/contribute/developer-guide).  
* Look through our [style guide]({{ site.github_io_url }}/manual/contribute/style-guides/index).  

## 🍹 Authors Notes

## ⚖️ License

{{ site.copyright }}  

This project is licensed under the **{{ site.license }} License**.  
See the [LICENSE]({{ site.repo_blob }}/LICENSE.md) file for the full license text.  

SPDX-License-Identifier: {{ site.license }}  

<!--
### TODO's

1. Documentation is currently getting wrong project_slug/name. ❌
    * Currently path for documentation is just the ```$(project_name)``` and not the ```$(namespace).$(project_name)```.
2. Finish ci/cd for changelog generation using antsichaut ❌
3. Decide if i should:  
    * Create ci/cd for documentation rather than using pre-commit

-->
