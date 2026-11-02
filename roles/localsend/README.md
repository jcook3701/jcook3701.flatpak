# Localsend

[LocalSend](https://github.com/localsend/localsend) is a cross-platform app that enables secure communication between devices using a REST API and HTTPS encryption. Unlike other messaging apps that rely on external servers, LocalSend doesn't require an internet connection or third-party servers, making it a fast and reliable solution for local communication.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `localsend_state` | str | The desired deployment state of the LocalSend Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `localsend_package` | str | The Flatpak application identifier for LocalSend. | `"org.localsend.localsend_app"` |
| `localsend_remote_name` | str | The name of the remote repository hosting the LocalSend Flatpak package. | `"flathub"` |

## Example Playbook Calls

Install **Localsend** package from flathub.

``` shell
$ ansible-playbook jcook3701.flatpak.localsend.yml -K
```

Uninstall **Localsend** package from flathub.

``` shell
$ ansible-playbook jcook3701.flatpak.localsend.yml -K -e "localsend_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
