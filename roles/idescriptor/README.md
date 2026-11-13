# iDescriptor

iDescriptor is a free, open-source, and cross-platform desktop management tool for iOS devices (iPhones and iPads). Built with a Rust backend and Qt/QML UI, it serves as an alternative to iTunes for Windows, macOS, and Linux.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `idescriptor_state` | str | The desired deployment state of the iDescriptor Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `idescriptor_package` | str | The Flatpak application identifier for iDescriptor. | `"io.github.idescriptor.iDescriptor"` |
| `idescriptor_remote_name` | str | The name of the remote repository hosting the iDescriptor Flatpak package. | `"flathub"` |

## Example Playbook Calls

**Install:**

``` shell
$ ansible-playbook jcook3701.flatpak.idescriptor.yml -K
```

**Uninstall:**

``` shell
$ ansible-playbook jcook3701.flatpak.idescriptor.yml -K -e "idescriptor_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
