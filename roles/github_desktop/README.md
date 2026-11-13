# Github Desktop

[GitHub Desktop](https://github.com/apps/desktop) is a free, open-source graphical application for Windows and macOS that simplifies working with Git and GitHub repositories without using the command line.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `github_desktop_state` | str | The desired deployment state of the GitHub Desktop Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `github_desktop_package` | str | The Flatpak application identifier for GitHub Desktop. | `"io.github.shiftey.Desktop"` |
| `github_desktop_remote_name` | str | The name of the remote repository hosting the GitHub Desktop Flatpak package. | `"flathub"` |

## Example Playbook Calls

**Install:**

``` shell
$ ansible-playbook jcook3701.flatpak.github_desktop.yml -K
```

**Uninstall:**

``` shell
$ ansible-playbook jcook3701.flatpak.github_desktop.yml -K -e "github_desktop_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
