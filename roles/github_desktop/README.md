# Github Desktop

**Install:**
``` shell
$ ansible-playbook jcook3701.flatpak.github-desktop.yml -K
```

**Uninstall:**
``` shell
$ ansible-playbook jcook3701.flatpak.github-desktop.yml -K -e "github_desktop_state=absent"
```
