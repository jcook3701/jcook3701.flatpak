# Code

[Visual Studio Code](https://flathub.org/en/apps/com.visualstudio.code) (commonly known as VS Code) is a free, lightweight, and extensible source-code editor developed by Microsoft. Available across Windows, macOS, Linux, and web browsers, it combines the simplicity of a fast text editor with powerful developer tools like debugging, version control, and AI assistance.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `code_state` | string | Desired lifecycle state of Visual Studio Code. Choices: `present`, `absent`, `teardown`. | `present` |
| `code_package` | string | Flatpak application ID for Visual Studio Code. | `com.visualstudio.code` |
| `code_remote_name` | string | Flatpak remote repository used to install Visual Studio Code. | `flathub` |

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and package management ecosystem.
