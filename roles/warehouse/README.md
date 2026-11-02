# Warehouse

[Warehouse](https://github.com/flattool/warehouse) is a versatile toolbox and provides a simple UI to control complex Flatpak options, all without resorting to the command line.

## Role Variables

## Example Playbook Calls

Install **Warehouse** Flatpak Application.

``` shell
$ ansible-playbook jcook3701.flatpak.warehouse.yml -K
```

Uninstall **Warehouse** Flatpak Application.

``` shell
$ ansible-playbook jcook3701.flatpak.warehouse.yml -K -e "warehouse_state=absent"
```

## Author Information

Maintained by **Jared Cook** as part of the core infrastructure and container management ecosystem.
