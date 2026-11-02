# Bottles

[Bottles](https://github.com/bottlesdevs/Bottles) abstracts the complexity of Wine configurations into a clean, elegant interface. Focus on your applications, not the configuration.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `bottles_state` | str | The desired deployment state of the Bottles Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `bottles_package` | str | The Flatpak application identifier for Bottles. | `"com.usebottles.bottles"` |
| `bottles_remote_name` | str | The name of the remote repository hosting the Bottles Flatpak package. | `"flathub"` |

## Example Playbook Calls

Install **Bottles** package from flathub.

``` shell
$ ansible-playbook jcook3701.flatpak.bottles.yml -K
```

Uninstall **Bottles** Flatpak Application.  

``` shell
$ ansible-playbook jcook3701.flatpak.bottles.yml -K -e "bottles_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
