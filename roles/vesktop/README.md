# Vesktop

[Vesktop](https://vesktop.dev/) is a customizable and privacy friendly Discord desktop app!

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `vesktop_state` | string | Desired lifecycle state of Vesktop. Choices: `present`, `absent`, `teardown`. | `present` |
| `vesktop_package` | string | Flatpak application ID for Vesktop. | `flathub dev.vencord.Vesktop` |
| `vesktop_remote_name` | string | Flatpak remote repository used to install Vesktop. | `flathub` |

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
