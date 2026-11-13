# Discord

[Discord](https://discord.com/) is a free voice, video, and text communication service used by tens of millions of people to talk and hang out with their communities and friends. It organizes conversations into private or public servers, where users can join voice channels, share screens, text in dedicated channels, and integrate automated tools and bots to manage community workflows.

## Role Variables

| Variable | Type | Description / Choices | Default |
| :--- | :--- | :--- | :--- |
| `discord_state` | str | The desired deployment state of the Discord Flatpak package.<br>**Choices:** `present`, `absent` | `"present"` |
| `discord_package` | str | The Flatpak application identifier for Discord. | `"org.discordapp.Discord"` |
| `discord_remote_name` | str | The name of the remote repository hosting the Discord Flatpak package. | `"flathub"` |

## Example Playbook Calls

Install **Discord** Flatpak Application.  

``` shell
$ ansible-playbook jcook3701.flatpak.discord.yml -K
```

Uninstall **Discord** Flatpak Application.  

``` shell
$ ansible-playbook jcook3701.flatpak.discord.yml -K -e "discord_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
