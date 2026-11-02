# Flatseal

[Flatseal](https://flathub.org/en/apps/com.github.tchx84.Flatseal) is a graphical utility for Linux that lets you review and modify permissions for your Flatpak applications.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `flatseal_state` | str | The desired deployment state of the Flatseal Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `flatseal_package` | str | The Flatpak application identifier for Flatseal. | `"com.github.tchx84.Flatseal"` |
| `flatseal_remote_name` | str | The name of the remote repository hosting the Flatseal Flatpak package. | `"flathub"` |

## Example Playbook Calls

Install **Flatseal** Flatpak Application.  

``` shell
$ ansible-playbook jcook3701.flatpak.flatseal.yml -K
```

Uninstall **Flatseal** Flatpak Application.  

``` shell
$ ansible-playbook jcook3701.flatpak.flatseal.yml -K -e "flatseal_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
