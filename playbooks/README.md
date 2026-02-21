# jcook3701.flatpak Galaxy Repository

## Authenticator

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.authenticator.yml -K

```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.authenticator.yml -K -e "authenticator_state=absent"
```

## Discord

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.discord.yml -K

```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.discord.yml -K -e "discord_state=absent"
```

## Flatseal

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.flatseal.yml -K

```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.flatseal.yml -K -e "flatseal_state=absent"
```

## Github-Desktop

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.github-desktop.yml -K

```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.github-desktop.yml -K -e "github_desktop_state=absent"
```

## Warehouse

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.warehouse.yml -K

```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.warehouse.yml -K -e "warehouse_state=absent"
```
