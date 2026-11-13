# Authenticator

[Authenticator](https://gitlab.gnome.org/World/Authenticator) is an open-source, time-based two-factor authentication (2FA) client specifically designed for the Linux desktop, utilizing modern GTK4 and libadwaita design standards.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `authenticator_state` | str | The desired deployment state of the Authenticator Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `authenticator_package` | str | The Flatpak application identifier for Authenticator. | `"com.belmoussaoui.Authenticator"` |
| `authenticator_remote_name` | str | The name of the remote repository hosting the Authenticator Flatpak package. | `"flathub"` |

## Example Playbook Calls

**Install:** Flatpak Authenticator Application.

``` shell
$ ansible-playbook jcook3701.flatpak.authenticator.yml -K
```

**Uninstall:** Flatpak Authenticator Application.

``` shell
$ ansible-playbook jcook3701.flatpak.authenticator.yml -K -e "authenticator_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
